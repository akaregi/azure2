<script lang="ts">
  let isOpen = false;
</script>

<nav>
  <h1 class="menu-header"><a data-sveltekit-preload-data="hover" href="/">AZURE.ICU</a></h1>

  <button class="menu-button" on:click={() => (isOpen = !isOpen)}> MENU (TOUCH HERE) </button>

  <ul class="menu-items {isOpen ? 'menu-open' : ''}">
    <li class="menu-item"><a data-sveltekit-preload-data="hover" href="/">/index</a></li>
    <li class="menu-item"><a data-sveltekit-preload-data="hover" href="/works">/works</a></li>
    <li class="menu-item"><a data-sveltekit-preload-data="hover" href="/scaffolding">/posts</a></li>
    <li class="menu-item"><a data-sveltekit-preload-data="hover" href="/scaffolding">/photos</a></li>
    <li class="menu-item"><a data-sveltekit-preload-data="hover" href="/scaffolding">/misc</a></li>
  </ul>
</nav>

<style>
  a {
    color: var(--grey);
  }

  .menu-header {
    margin-bottom: 3rem;
    color: var(--grey);
  }

  .menu-button {
    display: none;
  }

  .menu-items {
    margin: 0;
  }

  .menu-item {
    margin-bottom: 1rem;
  }

  .menu-item::before {
    content: "";
    margin: 0;
  }

  @media screen and (max-width: 768px) {
    .menu-header {
      display: none;
    }

    .menu-button {
      display: block;
      margin-bottom: 1rem;
    }

    .menu-items {
      display: none;

      margin-bottom: 3rem;
    }

    .menu-items.menu-open {
      display: block;
    }
  }
</style>
