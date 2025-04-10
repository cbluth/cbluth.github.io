<!-- src/lib/Nav.svelte -->
<script lang="ts">
    import Theme from "./Theme.svelte";
    import { navigate } from "./route.svelte";
</script>

<!-- svelte-ignore a11y_no_static_element_interactions -->
<div
    class="
    flex flex-col sm:flex-row sm:h-[64px] sm:h-min-[64px]
    justify-around items-center
    w-full bg-[var(--bg-color2)]
    "
>
    <div class="flex">
        <!-- svelte-ignore a11y_click_events_have_key_events -->
        <span
            on:click={() => navigate("")}
            class="mx-[24px] text-[24px] font-bold select-none cursor-pointer"
            >Cobin.io</span
        >
    </div>
    <div class="flex">
        <Theme />
    </div>
    <div class="flex flex-row">
        <!-- svelte-ignore a11y_click_events_have_key_events -->
        <span
            on:click={() => navigate("")}
            class="mx-[12px] text-[16px] cursor-pointer">Home</span
        >
        <!-- svelte-ignore a11y_click_events_have_key_events -->
        <span
            on:click={() => navigate("/about")}
            class="mx-[12px] text-[16px] cursor-pointer">About</span
        >
        <!-- svelte-ignore a11y_click_events_have_key_events -->
        <span
            on:click={() => navigate("/blog")}
            class="mx-[12px] text-[16px] cursor-pointer">Blog</span
        >
    </div>
</div>

<style lang="postcss">
    @reference "tailwindcss";
</style>
