<script>
	import FetchExample from './FetchExample.svelte'
	export let name
</script>

<main>
	<h1 class="text-3xl">Hello {name}!</h1>
	<h3 class="text-2xl"><span class="text-orange-600">Svelte</span> + <span class="text-teal-500">Tailwind</span></h3>
	<p>
		Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
		how to build Svelte apps.
	</p>

	<FetchExample />
</main>

<style>
</style>
