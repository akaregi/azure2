<script type="ts">
    export let title: string;
</script>

<h1>{title}</h1>

<style>
    h1::after {
        white-space: pre;
        content: "\A----";
    }

    h1 {
        margin-bottom: 3rem;
    }

    @media screen and (max-width: 768px) {
        h1 {
            margin-bottom: 1rem;
        }
    }
</style>
