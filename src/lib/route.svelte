<!-- src/lib/route.svelte -->
<script lang="ts" module>
    import { writable } from "svelte/store";
    export const route = writable(getCurrentRoute());
    function getCurrentRoute(): string {
        const hash = window.location.hash;
        return hash.startsWith("#!") ? hash.slice(2) : "";
    }
    window.addEventListener("hashchange", () => {
        route.set(getCurrentRoute());
    });
    export function navigate(path: string) {
        window.location.hash = `#!${path}`;
    }
</script>
