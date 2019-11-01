<script>
  import { createEventDispatcher } from "svelte";
  const dispatch = new createEventDispatcher();

  function messager() {
    console.log("got here");
    dispatch('message',{
        text:'yo21'
    });
  }
</script>

<button on:click={messager}>Click!</button>
