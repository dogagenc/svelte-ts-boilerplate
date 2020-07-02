<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: red;
  }
</style>

<script lang="ts">
  export let name: string;

  import Component from './Component.svelte';

  let myName = 'doga';
  let mySurname = 'genc';
  let fullName: string;
  $: fullName = `${myName} ${mySurname}`;
</script>

<main>
  <h1>Hello {name}!</h1>
  <Component name={fullName} count={4} />
</main>
