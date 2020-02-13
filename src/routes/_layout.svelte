<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<style>
	main {
		position: relative;
		background-color: white;
		padding: .5em;
		margin: 0 .5rem .5rem;
		box-sizing: border-box;
		min-height: 100vh;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	@media (min-width: 480px) {
		main {
			margin: 0 1.5rem 1.5rem;
		}
	}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>