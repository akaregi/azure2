<script lang="ts">
    export let title: string;
</script>

<section>
    <h2>{title}</h2>
    <div class="content">
        <slot />
    </div>
</section>

<style>
    h2 {
        margin-bottom: 1rem;
        font-size: 1.5rem;
    }

    h2::before {
        content: "## ";
    }

    .content {
        margin-left: 2rem;
        margin-bottom: 3rem;
    }

    @media screen and (max-width: 768px) {
        .content {
            margin-left: 0.5rem;
        }
    }
</style>
