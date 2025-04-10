<!-- src/lib/About.svelte -->
<script lang="ts">
    //
</script>

<!-- view -->
<div class="flex flex-col items-center max-w-[720px] p-[24px]">
    <span class="text-[26px] font-bold">👋 Hi, I'm Cobin.</span>
    <div class="flex flex-row w-full justify-between">
        <div class="flex flex-col text-center mx-4">
            <picture class="m-2">
                <source
                    class="mx-auto my-4 rounded-lg w-32 h-32"
                    srcset="/a/me.webp"
                    type="image/webp"
                />
                <img
                    class="mx-auto my-4 rounded-lg w-32 h-32"
                    src="/a/me.png"
                    alt="me"
                    title=""
                    style=""
                />
            </picture>
            <span class="whitespace-nowrap text-[var(--text-color2)]"
                >Systems Engineering</span
            >
            <span class="whitespace-nowrap text-[var(--text-color2)]"
                >Scalable Automation</span
            >
        </div>
        <div class="flex flex-col mx-4 max-w-[460px]">
            <span class="my-8 text-[var(--text-color2)]">
                I'm a systems generalist with a strong focus on Linux,
                high-performance, low-latency infrastructure. I'm passionate
                about building robust, automated, and scalable environments
                using open-source technologies. <br />
                At my core I am a Linux Enthusiast.</span
            >
            <span class="text-[var(--text-color2)]">What drives me:</span>
            <ul class="list-none mb-4">
                <li>
                    <span>
                        Scalable architecture, strong typing, and
                        well-engineered automation pipelines. I believe in
                        repeatability, resilience, and observability.
                    </span>
                </li>
            </ul>
            <span class="text-[var(--text-color2)]"
                >Here are a few things I work with:</span
            >
            <ul class="list-disc">
                <li>
                    Compute and Infrastructure: Cloud (AWS/Azure), Kubernetes,
                    Bare-metal Provisioning (OutofBand/PXE), Linux
                    (RHEL/Debian), Containers (Docker/Podman), Infrastructure as
                    Code (Terraform)
                </li>
                <li>
                    Automation & Tooling: CI/CD Pipelines, Gitops, Scripting
                    (bash/python), systemd, Ansible
                </li>
                <li>
                    Frontend Development: node, typescript, html/css (svelte)
                </li>
                <li>
                    Backend Development: golang, python, rest, databases
                    (postgres/mysql)
                </li>
                <li>And:
                    security and compliance frameworks,
                    identity and access control,
                    kernel tuning, monitoring systems
                </li>
            </ul>
            <span class="text-[var(--text-color2)]"
                >You can contact me by emailing:</span
            >
            <span class="font-bold text-[var(--text-color2)]"
                >hi [at] cobin [dot] io</span
            >
        </div>
    </div>
</div>

<style>
    /*  */
</style>
