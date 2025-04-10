<!-- src/lib/Main.svelte -->
<script lang="ts">
</script>

<div class="flex flex-col items-center max-w-[512px] w-[512px] p-[24px]">
    <span class="text-[26px] font-bold">👋 Hi, I'm Cobin.</span>
    <picture class="m-2">
        <source
            class="rounded-full w-[250px] h-[250px] m-2"
            srcset="/me.webp"
            type="image/webp"
        />
        <img
            class="rounded-full w-[250px] h-[250px] m-2"
            src="/me.png"
            alt="me"
            title=""
            style=""
        />
    </picture>
    <span class="text-[18px] text-[var(--text-color2)]"
        >communicator, collaborator, doer</span
    >
    <span class="text-[18px] whitespace-pre-wrap text-[var(--text-color2)]"
        >container evangelist, cloud thinker</span
    >
    <span class="text-[18px] whitespace-pre-wrap text-[var(--text-color2)]"
        >infrastructure solutioner, byte wizard</span
    >
    <span class="text-[18px] whitespace-pre-wrap text-[var(--text-color2)]"
        >fixer, tinkerer, internet plumber</span
    >
    <div class="flex flex-row">
        <!-- svelte-ignore a11y_consider_explicit_label -->
        <a
            href="https://github.com/cbluth"
            target="_blank"
            rel="noopener noreferrer me"
            title="Github"
            style="margin: 12px"
            ><svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
                class="p-[2px] w-[24px]"
                ><path
                    d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"
                ></path></svg
            ></a
        >
        <!-- svelte-ignore a11y_consider_explicit_label -->
        <a
            href="https://www.linkedin.com/in/cbluth/"
            target="_blank"
            rel="noopener noreferrer me"
            title="Linkedin"
            style="margin: 12px"
            ><svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
                class="p-[2px] w-[24px]"
                ><path
                    d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"
                ></path><rect x="2" y="9" width="4" height="12"></rect><circle
                    cx="4"
                    cy="4"
                    r="2"
                ></circle></svg
            ></a
        >
    </div>
</div>
