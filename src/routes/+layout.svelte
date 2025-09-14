<script lang="ts">
	import '../app.css';

	let { children } = $props();

		import Header from '$lib/components/layoutComponents/Header.svelte';

</script>


<Header />
{@render children()}
