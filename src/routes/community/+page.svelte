<script>
	import Nav from '$lib/components/Nav.svelte';
	import { Card } from 'flowbite-svelte';
</script>

<Nav></Nav>

<Nav />
<main class="grid place-content-center">
	<div class="title flex justify-center text-6xl">
		Welcome to
		<div class="gradient-title text-white">Maycoon</div>
	</div>

	<div class="cards mt-20 flex">
		<Card class="mr-16 text-black" href="https://github.com/maycoon-ui/maycoon" target="_blank">
			<h5 class="mb-2 text-xl font-bold">GitHub</h5>
			<p class="text-xl leading-tight">
				Watch for the newest changes, open an issue, suggest something or even contribute with your
				own code!
			</p>
		</Card>
		<Card class="mr-16 text-black">
			<h5 class="mb-2 text-xl font-bold">Discord</h5>
			<p class="text-xl leading-tight">
				Have a quick question or just want to chat about Maycoon? Then join our Discord Server!
			</p>
		</Card>
		<Card class="text-black">
			<h5 class="mb-2 text-xl font-bold">More???</h5>
			<p class="text-xl leading-tight">???</p>
		</Card>
	</div>
</main>

<style lang="scss">
	.title {
		margin-top: 8rem;
	}

	.gradient-title {
		margin-left: 1.5rem;
		margin-top: -0.5rem;
		padding: 0.5rem;
		border-radius: 15px;
		background: linear-gradient(-30deg, rgb(13, 131, 241), rgb(211, 15, 211));
	}
</style>
