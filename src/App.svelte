<script lang="ts">
  let name: string = "Svelte";

  let count: number = 0;

  let double: number;
  $: double = count * 2;

  let fAdd = () => count++;
</script>

<main>
  <h1>Hello {name}!</h1>

  <button on:click={fAdd} id="counter">
    {count}
  </button>
</main>
