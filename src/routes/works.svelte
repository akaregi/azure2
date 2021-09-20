<script context="module" lang="ts">
    import Header from '$lib/components/Header.svelte'
    import Section from '$lib/components/Section.svelte'

    export const prerender = true
</script>

<svelte:head>
    <title>Works</title>
</svelte:head>

<Header title="Works" />

<Section heading="2" title="The Red Project">
    <p>Some plans belong to this project.</p>

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
        <li>Indarin Paria</li>
    </ul>
</Section>

<Section heading="3" title="The Red Resolution">
    <p>
        The Red Resolution(TRR) is my own Pleroma instance. I'm the principal of
        TRR. TRR is a single-user instance, so anyone other than me may not
        join. Follow my account if you make the instance relationship.
    </p>
</Section>

<Section heading="3" title="Indarin Paria">
    <p>
        The special project named “INDARIN PARIA”(former to “raipara-rei ryky”;
        r3) is in progress. Indarin Paria is a constructed language I make. Its
        comprehensive book will be open to the public in the future. Now this
        conlang is closed-beta.
    </p>
</Section>

<h2>The Fedyya Project</h2>

<Section heading="3" title="fedyya LUNARIS">
    <p>
        <a href="https://lunaris.azure.icu/">fedyya LUNARIS</a> is a set of my Hymmnos(conlang
        of Ar Tonelico) creations. You may use all of them by CC-BY 4.0 license.
    </p>
</Section>

<h2>Serious projects</h2>

<Section heading="3" title="Lianiis Min's site">
    <p>
        I built a site for <a href="https://www.lianiis.com/">Lianiis Min</a
        >(conlang) what what was made by my friend. For making this site, I gave
        my friend technical advice, for instance, collecting words and compiled
        them in the searchable dictionary.
    </p>
</Section>

<h2>Other works</h2>

<Section heading="3" title="Emoji Builder">
    <p>
        <a href="https://emoji-builder.azure.icu/">The Emoji Builder</a> is
        complicated to explain. This site is for making a sentence with Emoji
        expression. This is published on
        <a href="https://github.com/akaregi/emoji-builder">GitHub</a>.
    </p>
</Section>

<Section heading="3" title="The Iyo Shrine">
    <p>
        <a href="https://omikuji.azure.icu/">The Iyo Shrine</a>(JA: 伊予神社) is
        a virtual shrine that you can pick some Omikujis(like a fortune cookie).
        I license this as AGPL-3.0 so you can get source codes on
        <a href="https://github.com/akaregi/Omikuji-Machine">GitHub</a>. New
        result candidates are welcome. If you desire, please make a PR at
        GitHub.
    </p>
</Section>
