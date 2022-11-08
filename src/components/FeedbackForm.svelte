<script>
  import Card from "./Card.svelte";
  import Button from "./Button.svelte";

  let text = ''
  let btnDesabled = true
</script>

<Card>
<header>
  <h2>How would you rate our service with us?</h2>
</header>

<form>
  <!-- Rating Select -->
  <div class="input-group">
    <input type="text" bind:value={text} placeholder="Tell us something that keeps you coming back">
    <Button disabled={btnDesabled} type="submit">Send</Button>
  </div>
</form>
</Card>

<style>
  .input-group{

  }

</style>