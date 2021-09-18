<script lang="ts">
    let isOpen = false;
</script>

<nav>
    <h2 class="wide"><a sveltekit:prefetch href="/">AZURE.ICU</a></h2>

    <h2 class="narrow" on:click={() => (isOpen = !isOpen)}>
        MENU (TOUCH HERE)
    </h2>

    <ul
        class="menu-items {isOpen ? 'open' : ''}"
        on:click={() => (isOpen = !isOpen)}
    >
        <li><a sveltekit:prefetch href="/">/index</a></li>
        <li><a sveltekit:prefetch href="/scaffolding">/posts</a></li>
        <li><a sveltekit:prefetch href="/scaffolding">/photos</a></li>
        <li><a sveltekit:prefetch href="/scaffolding">/misc</a></li>
        <li>
            <a href="https://twitter.com/nanigashi_777">Twitter</a>
        </li>
        <li>
            <a href="https://social.azure.icu/red_resolution"> Pleroma </a>
        </li>
    </ul>
</nav>

<style>
    h2 {
        margin-bottom: 3rem;
        color: var(--grey);
    }

    h2::after {
        white-space: pre;
        content: "\A----";
    }

    ul {
        margin: 0;
    }

    li {
        margin-bottom: 1rem;
    }

    li::before {
        content: "";
        margin: 0;
    }

    a {
        color: var(--grey);
    }

    .narrow {
        display: none;
    }

    @media screen and (max-width: 768px) {
        h2 {
            margin-bottom: 1rem;
        }

        .wide {
            display: none;
        }

        .narrow {
            display: block;
        }

        .menu-items {
            display: none;

            margin-bottom: 3rem;
        }

        .menu-items.open {
            display: block;
        }
    }
</style>
