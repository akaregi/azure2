<script lang="ts" context="module">
    export const load = async ({ page }) => ({
        props: {
            key: page.path,
        },
    });
</script>

<script lang="ts">
    import "../css/reset.css";
    import "../css/app.css";

    import Footer from "$lib/layout/Footer.svelte";
    import Menu from "$lib/layout/Menu.svelte";
    import PageTransition from "$lib/components/PageTransition.svelte";

    export let key: string;
</script>

<div class="wrapper">
    <div class="left">
        <Menu />
    </div>

    <div class="right">
        <main>
            <PageTransition refresh={key}>
                <slot />
            </PageTransition>
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
