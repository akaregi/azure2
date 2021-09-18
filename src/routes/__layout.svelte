<script lang="ts">
    import "../css/reset.css";
    import "../css/app.css";

    import Footer from "$lib/Footer.svelte";
    import Menu from "$lib/Menu.svelte";
</script>

<div class="wrapper">
    <div class="left">
        <Menu />
    </div>

    <div class="right">
        <main>
            <slot />
        </main>

        <Footer />
    </div>
</div>

<style>
    .wrapper {
        display: grid;
        grid-template-areas: "left right";
        grid-template-columns: 1fr 4fr;
    }

    @media screen and (max-width: 768px) {
        .wrapper {
            grid-template-areas: "left" "right";
            grid-template-columns: 1fr;
        }
    }

    .left {
        grid-area: left;
    }

    .right {
        grid-area: right;
    }
</style>
