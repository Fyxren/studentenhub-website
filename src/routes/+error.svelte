<script>
    import { page } from "$app/stores";
    import Footer from "../lib/components/Footer.svelte";
</script>

<div
    class="flex flex-col h-screen max-h-screen bg-gradient-to-br from-[#001930] to-[#003F6C] text-[#C9E5FF]"
>
    <main
        class="flex flex-col items-center justify-center h-screen"
    >
        <h1 class="text-6xl font-bold tracking-widest">{$page.status}</h1>
        <p class="mt-2 text-3xl font-semibold">{$page.error.message}</p>

        <a
            class="btn btn-ghost btn-wide bg-[#fda515]/80 hover:bg-[#fda515]/70 font-semibold tracking-wider mt-10"
            href="/"
        >
            Back to home
        </a>
    </main>

    <Footer />
</div>
