<script>
  import Inner from "./Inner.svelte";
  export let name;
  let count = 0;

  function handle(event) {
    alert("yo");
  }
</script>

<style>
  h1 {
    color: purple;
  }
</style>

<h1>Hello {name}!</h1>

<Inner on:message={handle} />
