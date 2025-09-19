<script lang="ts">
	import '../app.css';

	let { children } = $props();

		import Header from '$lib/components/layoutComponents/Header.svelte';
	import Footer from '$lib/components/layoutComponents/Footer.svelte';

</script>

<svelte:head>
	<script src="https://kit.fontawesome.com/bb271890d7.js" crossorigin="anonymous"></script>

</svelte:head>


<Header />

{@render children()}

<Footer />
