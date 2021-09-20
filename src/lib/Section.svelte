<script lang="ts">
    export let title: string;
    export let heading: "1" | "2" | "3" | "4" | "5" | "6";
</script>

<section>
    {#if heading === "1"}
        <h1>{title}</h1>
    {:else if heading === "2"}
        <h2>{title}</h2>
    {:else if heading === "3"}
        <h3>{title}</h3>
    {:else if heading === "4"}
        <h4>{title}</h4>
    {:else if heading === "5"}
        <h5>{title}</h5>
    {:else if heading === "6"}
        <h6>{title}</h6>
    {/if}

    <div class="content">
        <slot />
    </div>
</section>

<style>
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
