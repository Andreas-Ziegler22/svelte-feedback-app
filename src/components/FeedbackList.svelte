<script>
  import {FeedbackStore} from '../store'
  import {fade, scale} from 'svelte/transition'
  import FeedbackItem from "./FeedbackItem.svelte";

  let feedback = []

  
</script>

<!-- foreach svelte -->
{#each $FeedbackStore as fb (fb.id)}
<div in:scale out:fade="{{ duration: 500}}">
  <FeedbackItem item={fb}/>
</div>
{/each}
