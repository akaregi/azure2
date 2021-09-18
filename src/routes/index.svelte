<script context="module" lang="ts">
    export const prerender = true;
</script>

<script lang="ts">
    import Header from "$lib/Header.svelte";
    import Section from "$lib/Section.svelte";
</script>

<svelte:head>
    <title>Welcome to azure.icu</title>
</svelte:head>

<Header title="Welcome to azure.icu" />

<Section title="Who am I?">
    <p>
        I'm akarregi, as known as regi. I live somewhere in Japan, very near to
        Tokyo.
    </p>

    <p>
        I'm a kind of hobby linguist, hobby programmer. But I spend much time
        gaming. It's so terriyfing...
    </p>
</Section>

<Section title="My Projects">
    <p>Some projects belong to me.</p>

    <ul>
        <li>
            <a href="https://social.azure.icu">The Red Resolution</a> for Pleroma.
        </li>
        <li>
            <a href="https://book.azure.icu/">The Red Book</a> for documentation.
        </li>
        <li>
            <a href="https://static.azure.icu/">The Red Vault</a> for archives.
        </li>
    </ul>

    <p>
        The Red Resolution(TRR) is my own Pleroma instance. I'm the principal of
        TRR. TRR is a single-user instance, so anyone other than me may not
        join. Follow my account if you make the instance relationship.
    </p>

    <p>
        The special project named “INDARIN PARIA”(former to “raipara-rei ryky”;
        r3) is in progress. Indarin Paria is a constructed language I make. Its
        comprehensive book will be open to the public in the future. Now this
        conlang is closed-beta.
    </p>
</Section>

<Section title="Contact">
    <p>I have various accounts for messaging. Active social networks are:</p>

    <ul>
        <li>Pleroma (@red_resolution@social.azure.icu) for primary.</li>
        <li>Twitter (@nanigashi_777) for secondary. I check it also.</li>
        <li>Discord for real-time messaging. Active if I'm awake.</li>
    </ul>

    <p>I use Telegram, Matrix, IRC optionally.</p>

    <p>If you prefer, there're PGP keys to send some messages securely.</p>

    <ul>
        <li>
            <a href="https://static.azure.icu/keys/AC04_7EE8_B935_A2E0.asc">
                AC04 7EE8 B935 A2E0
            </a>
            as akg.tachibana(at)gmail.com
        </li>
        <li>
            <a href="https://static.azure.icu/keys/65BA_1CD4_CFA7_7FD3.asc">
                65BA 1CD4 CFA7 7FD3
            </a>
            as verdigris(at)azure.icu
        </li>
    </ul>
</Section>
