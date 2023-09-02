<script>
	import Header from "./Header.svelte"
	import Footer from "./Footer.svelte"
	import Navigation from "./Navigation.svelte"
</script>

<svelte:head>
	<title>Slowpals</title>
</svelte:head>

<div class="layout">
	
	<Header />
	
	<Navigation />
	
	<main>
		<slot />
	</main>
	
	<Footer />
	
</div>

<style>
	
	:global(html, body){
		margin: 0;
		padding: 0;
	}
	
	:global(*){
		box-sizing: border-box;
	}
	
	.layout{
		background-color: aqua;
		min-height: 100vh;
		display: grid;
		grid-template-rows: auto auto 1fr auto;
		padding: 0.5em 1em;
	}
	
	main{
		max-width: 800px;
		margin: 0 auto;
	}
	
</style>