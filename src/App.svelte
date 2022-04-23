<script>
	import LeftSide from "./components/LeftSide.svelte";

	export let name;
</script>

<main>
	<LeftSide></LeftSide>
</main>

<style>
	*{
        background-image: url('/img/beams.jpg');
    }
	main {
		text-align: left;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
		background-image: url("/img/beams.jpg");
		background-repeat: no-repeat;
		background-size: cover;
		object-fit: fill;
		overflow: auto;
		color: rgb(68, 51, 51);
	}

	@media (min-width: 140px) {
		main {
			max-width: none;
		}
	}
</style>