<script>
	import Button from "./UI/Button.svelte";
	import Card from "./UI/Card.svelte";

	let name: string = "svelte";
	let counter: number = 0;
</script>

<main>
	<Card>
		<span slot="title">Hi from {name}.</span>
		<Button on:click={() => (counter = counter + 1)}
			>I was clicked {counter} times!</Button
		>
	</Card>
</main>

<style lang="scss">
	:global {
		* {
			font-family: Verdana, Geneva, Tahoma, sans-serif;
		}

		body {
			background: #ececde;
			height: 100vh;
		}

		main {
			margin-top: 10rem;
			display: flex;
			justify-content: center;
			align-items: center;
		}
	}
</style>
