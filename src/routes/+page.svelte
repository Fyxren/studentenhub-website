<script>
    import Footer from "../lib/components/Footer.svelte";

    let list = [
        "Een plek voor al je vragen",
        "Voor ieder vak een eigen kanaal & rol",
        "Open voor suggesties en ideeën",
        "Behulpzaam-rol wanneer verdiend",
    ];
</script>

<div
    class="flex flex-col h-screen max-h-screen overflow-hidden bg-gradient-to-br from-[#001930] to-[#003F6C] text-[#C9E5FF] px-5"
>
    <main
        class="flex flex-col items-center justify-center h-screen max-h-screen text-center"
    >
        <h1 class="mt-10 text-3xl font-bold md:mt-0 md:text-6xl">
            📚 • Studentenhub
        </h1>
        <p class="mt-5 text-lg italic md:mt-10 md:text-xl">
            Dé Discord server voor scholieren en studenten!
        </p>

        <div class="grid gap-3 mt-5 md:gap-5 md:mt-20 md:grid-cols-2">
            {#each list as item}
                <div
                    class="w-full px-10 py-2 text-center rounded-lg bg-white/5"
                >
                    {item}
                </div>
            {/each}
        </div>

        <a
            class="btn btn-ghost btn-wide bg-[#fda515]/80 hover:bg-[#fda515]/70 font-semibold tracking-wider mt-5 md:mt-10"
            href="https://discord.com/invite/YtXxyCtfwv"
            target="_blank">Join de server</a
        >
    </main>

    <Footer />
</div>
