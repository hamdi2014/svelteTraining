<script>
    async function getRandomNumber() {
		const res = await fetch(`https://svelte.dev/tutorial/random-number`);
		const text = await res.text();
		console.log(text)
		if (res.ok) {
			return text;
		} else {
			throw new Error(text)
		}
	}
	
	let promise = getRandomNumber();

	function hndlClk() {
		promise = getRandomNumber();
	}
</script>

<button on:click={hndlClk}>
	generate random number
</button>

<!-- replace this element -->
{#await promise}
	<p>...waiting</p>
{:then number}
	<p>The number is {number}</p>
{:catch error}
	<p style="color: red;">{error.message}</p>
{/await}