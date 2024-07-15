<script lang="ts">
	import { page } from '$app/stores';
	import { GradientButton } from 'flowbite-svelte';
</script>

<main class="grid place-content-center">
	<svg class="animate-text" viewBox="0 0 1200 300">
		<symbol id="s-text">
			<text text-anchor="middle" x="50%" y="80%">{$page.status}: {$page.error?.message}</text>
		</symbol>

		<g class="g-ants">
			<use xlink:href="#s-text" class="text-copy"></use>
			<use xlink:href="#s-text" class="text-copy"></use>
			<use xlink:href="#s-text" class="text-copy"></use>
			<use xlink:href="#s-text" class="text-copy"></use>
			<use xlink:href="#s-text" class="text-copy"></use>
			<use xlink:href="#s-text" class="text-copy"></use>
			<use xlink:href="#s-text" class="text-copy"></use>
		</g>
	</svg>

	<div class="mt-2 text-center text-4xl">
		{#if $page.status === 400}
			I'd rather prefer good requests.
		{:else if $page.status === 401}
			Unauthorized Request... yikes!
		{:else if $page.status === 403}
			You are not allowed to pass!
		{:else if $page.status === 404}
			Minor spelling mistake?
		{:else if $page.status === 405}
			I need a valid method please!
		{:else if $page.status === 406}
			UNACCEPTABLE!
		{:else if $page.status === 408}
			Sorrry, but the servers seem to be slower than snails!
		{:else if $page.status === 410}
			I call this page gonzo, because... it's gone!
		{:else if $page.status === 413}
			We need more support heroes to move that payload!
		{:else if $page.status === 414}
			Yo URL's so fat, it can turn an iPhone into an iPad by sitting on it.
		{:else if $page.status === 418}
			I'm a f*cking Teapot you idiot!
		{:else if $page.status === 429}
			The amount of requests overcome the amount of fat people jokes...
		{:else if $page.status === 431}
			Yo Header's so big, people shout Taxi when it wears yellow.
		{:else if $page.status === 451}
			Your government or something censored this page. Not Cool! #fckCensorship
		{:else if $page.status === 500}
			Wait... did you try to divide by zero?
		{:else if $page.status === 501}
			I'm either still living in the stone age or you just can't type.
		{:else if $page.status === 502}
			Your gateway is so bad, it may be responsible for climate change.
		{:else if $page.status === 505}
			That HTTP version ain't supported here, pal!
		{:else if $page.status === 508}
			Are you kidding me?
		{:else}
			Someone messed up...
		{/if}
	</div>

	<GradientButton class="mt-12 w-fit place-self-center" outline color="purpleToPink" href="../">
		<div class="text-2xl">Back to Home</div>
	</GradientButton>
</main>

<style lang="scss">
	.animate-text {
		font-size: 5.5rem;
		width: 1200px;
		height: 300px;
	}

	.text-copy {
		fill: none;
		stroke: white;
		stroke-dasharray: 6% 29%;
		stroke-width: 5px;
		stroke-dashoffset: 0%;
		animation: stroke-offset 5.5s infinite linear;
	}

	.text-copy:nth-child(1) {
		stroke: #4d163d;
		animation-delay: -1;
	}

	.text-copy:nth-child(2) {
		stroke: #840037;
		animation-delay: -2s;
	}

	.text-copy:nth-child(3) {
		stroke: #bd0034;
		animation-delay: -3s;
	}

	.text-copy:nth-child(4) {
		stroke: #bd0034;
		animation-delay: -4s;
	}

	.text-copy:nth-child(5) {
		stroke: #fdb731;
		animation-delay: -5s;
	}

	.text-copy:nth-child(6) {
		stroke: #f8a916;
		animation-delay: -6s;
	}

	.text-copy:nth-child(7) {
		stroke: #c00c0c;
		animation-delay: -7s;
	}

	@keyframes stroke-offset {
		100% {
			stroke-dashoffset: -35%;
		}
	}
</style>
