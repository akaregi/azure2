<script lang="ts">
  export let title: string;
</script>

<h1 class="header">{title}</h1>

<style>
  .header {
    margin-bottom: 3rem;
  }

  .header::after {
    white-space: pre;
    content: "\A----";
  }

  @media screen and (max-width: 768px) {
    .header {
      margin-bottom: 1rem;
    }
  }
</style>
