<h1 class="text-3xl font-bold mb-4">
    Declutter your Data Pipeline
</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<script> 
let x = 0;
	let y = 0;
	
	function yPlusAValue(value) {
		return value + y;
	}
	
	$: total = yPlusAValue(x);
</script> 
Total: {total}
<button on:click={() => x++}>
	Increment X
</button>

<button on:click={() => y++}>
	Increment Y
</button>

<style>
	p {
		color: rgb(0, 128, 90);
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}

    button {background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;

    }
</style>
