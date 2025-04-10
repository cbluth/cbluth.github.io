<script module lang="ts">
    let i = 0;
    const themes = ["dark", "light", "midnight", "solarized"];
    type Theme = (typeof themes)[number];
    export function setTheme(theme: Theme) {
        localStorage.setItem("theme", theme);
        document.documentElement.setAttribute("theme", theme)
        i = themes.indexOf(theme)
    }
    export function getTheme(): Theme {
        const theme = localStorage.getItem("theme") as Theme;
        if (themes.includes(theme as Theme)) {
            return theme as Theme;
        }
        return "dark";
    }
    export function next(): Theme {
        i = (i + 1) % themes.length;
        const theme = themes[i];
        setTheme(theme);
        return theme
    }
    export function initTheme() {
        setTheme(getTheme())
    }
</script>

<script lang="ts">
    let theme: Theme = $state("dark");
    const icons: Record<Theme, string> = {
        dark: "🌚",
        light: "🌞",
        midnight: "🌌",
        solarized: "🌇",
    };
    function rotate() {
        theme = next();
    }
    $effect(() => {
        initTheme();
        theme = getTheme();
    })
</script>

<div class="flex m-1 items-center justify-center h-[50px] w-[50px]">
    <button
    onclick={rotate}
    class="
        text-2xl p-2 rounded-full
        transition-transform duration-500
        hover:scale-120 active:rotate-180 cursor-pointer
    "
    >
        {icons[theme]}
    </button>
</div>

<style lang="postcss">
    @reference "tailwindcss";
</style>

