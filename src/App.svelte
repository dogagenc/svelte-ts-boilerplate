<script lang="ts">
  import Component from './Component.svelte';

  let name = 'world';
  let fullName;
  $: fullName = `${name} !`;
</script>

<main>
  <h1>
    <Component name={fullName} />
  </h1>
</main>
