<!-- src/App.svelte -->
<script lang="ts">
    import Nav from "./lib/Nav.svelte";
    import Main from "./lib/Main.svelte";
    import About from "./lib/About.svelte";
    import Footer from "./lib/Footer.svelte";
    import { route } from "./lib/route.svelte";
    let view = $state("");
    $effect(() => {
        const unsubscribe = route.subscribe((v) => {
            view = v;
        });
        return unsubscribe;
    });
</script>

<div class="flex flex-col h-screen w-full">
    <Nav />
    <main
        class="flex flex-col flex-grow items-center justify-center w-full mx-auto px-4"
    >
        {#if view === ""}
            <Main />
        {:else if view === "/about"}
            <About />
        {:else if view === "/blog"}
            <h1 class="text-center mt-10 text-2xl">Blog</h1>
        {:else}
            <h1 class="text-center mt-10 text-2xl">404 - not found</h1>
        {/if}
    </main>
    <Footer />
</div>

<style lang="postcss">
    @reference "tailwindcss";
</style>
