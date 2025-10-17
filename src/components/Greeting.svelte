<script>
  const { messages } = $props();

  let greeting = $state(messages[0]);
  
  const random = () => {
    return messages[(Math.floor(Math.random() * messages.length))];
  }

</script>

<div>
  <h3>{greeting}! Thank you for visiting!</h3>
  <button onclick={() => greeting = random()}>
    New Greeting
  </button>
</div>