<script>
    import Ingredients from "./components/Ingredients.svelte";
    import Instructions from "./components/Instructions.svelte";
import Intro from "./components/Intro.svelte";
    import Nutrition from "./components/Nutrition.svelte";


</script>

<svelte:head>
	<title>Recipe Page</title>
	<html lang="en" />
</svelte:head>

<main>
	<div class="components-container">
		<Intro />
		<div>
			<Ingredients />
			<Instructions />
			<Nutrition />
		</div>
	</div>
</main>

<style>
	.components-container > div{
		padding: 1.5em;
	}

	@media (min-width:40em){
		main{
			margin-block: 7em;
		}
		.components-container{
			background: var(--neu-white);
			border-radius: 20px;
			padding: 3em;
			max-width: 48em;
			margin-inline: auto;
		}
	}
</style>