<script context="module" lang="ts">
  export const prerender = true;
</script>

<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Section from "$lib/components/Section.svelte";
</script>

<svelte:head>
  <title>Welcome to azure.icu</title>
</svelte:head>

<Header title="Welcome to azure.icu" />

<Section heading="2" title="Who am I?">
  <p>I'm akarregi, as known as nanigashi. I live somewhere in Japan, very near to Tokyo.</p>

  <p>I'm a kind of hobby linguist, hobby programmer. But I spend much time gaming. It's so terriyfing...</p>
</Section>

<Section heading="2" title="Contact">
  <p>I have various accounts for messaging. Active social networks are:</p>

  <ul>
    <li>Twitter (@nanigashi_777) for primary..</li>
    <li>ActivityPub(@nanigashi@council.azure.icu) for secondary.</li>
    <li>Discord for real-time messaging. Active if I'm awake.</li>
  </ul>

  <p>If you prefer, there're PGP keys to send some messages securely.</p>

  <ul>
    <li>
      <a href="https://static.azure.icu/keys/AC04_7EE8_B935_A2E0.asc"> AC04 7EE8 B935 A2E0 </a>
      as akg.tachibana(at)gmail.com
    </li>
    <li>
      <a href="https://static.azure.icu/keys/65BA_1CD4_CFA7_7FD3.asc"> 65BA 1CD4 CFA7 7FD3 </a>
      as verdigris(at)azure.icu
    </li>
  </ul>
</Section>
