<script>
  import FeedbackItem from "./FeedbackItem.svelte";

  export let feedback = []

  console.log(feedback)
</script>

<!-- foreach svelte -->
{#each feedback as fb (fb.id)}
  <FeedbackItem item={fb}/>
{/each}
