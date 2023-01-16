<script>
	import Thing from "./Thing.svelte";
	import MouseMove from "./MouseMove.svelte";
	import MouseMoveInline from "./MouseMoveInline.svelte";
	import HelloWorld from "./HelloWorld.svelte";
	import IfCondition from "./IfCondition.svelte";
	import IfElseCondition from "./IfElseCondition.svelte";
	import IfElseIfCondition from "./IfElseIfCondition.svelte";
  	import EachBlocks from "./EachBlocks.svelte";
  	import DynamicAttr from "./DynamicAttr.svelte";
  	import Styling from "./Styling.svelte";
  	import HtmlTags from "./HtmlTags.svelte";
  import Assignments from "./Assignments.svelte";
  import Declarations from "./Declarations.svelte";
  import Statements from "./Statements.svelte";
	// ---------------------------------------

	// ----------------------------------

	// ----------------------------------

	// --------------------------------------------

	let things = [
		{id: 1, name: 'apple'},
		{id: 2, name: 'banana'},
		{id: 3, name: 'carrot'},
		{id: 4, name: 'doughnut'},
		{id: 5, name: 'egg'}
	];

	function handleClick() {
		things = things.slice(1)
	}

	// -----------------------------------------------

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

<button on:click={handleClick}>
	Remove first thing
</button>

{#each things as thing (thing.id) }
	<Thing name={thing.name}/>
{/each}

<hr>

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

<HelloWorld />
<DynamicAttr />
<Styling />
<HtmlTags />
<Assignments />
<hr>
<Declarations />
<hr>
<Statements />
<hr>
<IfCondition />
<IfElseCondition />
<IfElseIfCondition />
<EachBlocks />
<MouseMove />
<MouseMoveInline />