<script context="module">
	export const prerender = true;
	import Counter from '$lib/counter.svelte';
</script>

<svelte:head>
	<title>Hello, world!</title>
	<meta name="description" content="Tailwind SvelteKit TypeScript" />
</svelte:head>

<section class="flex flex-col justify-center items-center h-screen">

	<div class="flex">
		<img class="w-60" src='./images/batman_eyes.gif' alt="Batman">
		<img class="w-60" src='./images/batman_skipping.gif' alt="Batman">
	</div>

	<h1 class="w-fit font-bold text-6xl my-4">
		Svelte Boilerplate
	</h1>

	<h2 class="w-fit text-lg">
		Sveltekit, TypeScript and Tailwind
	</h2>

	<Counter />
</section>