<script lang="ts">
	import Nav from '$lib/components/Nav.svelte';
	import { Card, GradientButton } from 'flowbite-svelte';
</script>

<Nav />

<main class="grid place-content-center">
	<div class="mt-48 flex place-self-center text-6xl">
		<section class="title mr-4 text-white">
			<div class="slide first"><div>Design</div></div>
			<div class="slide second"><div>Develop</div></div>
			<div class="slide third"><div>Deploy</div></div>
		</section>
		<div>with Maycoon!</div>
	</div>

	<div class="mt-12 flex place-content-center">
		<GradientButton
			class="m-10 w-60 p-1"
			href="https://maycoon-ui.github.io/guide"
			outline
			color="purpleToBlue"><h1 class="text-2xl">Getting Started</h1></GradientButton
		>

		<GradientButton
			class="m-10 w-60 p-1"
			href="https://www.github.com/maycoon-ui/maycoon"
			target="_blank"
			outline
			color="purpleToBlue"><h1 class="text-2xl">GitHub</h1></GradientButton
		>
	</div>

	<div class="cards mt-24 flex">
		<Card class="mr-16 text-black">
			<h5 class="mb-2 text-2xl font-bold">Beautiful</h5>
			<p class="text-xl leading-tight">
				Utilize a large collection of fast, well-designed & beautiful built-in Widgets to design the
				perfect User Interface.
			</p>
		</Card>
		<Card class="mr-16 text-black">
			<h5 class="mb-2 text-2xl font-bold">Plug'n'Play</h5>
			<p class="text-xl leading-tight">
				Simply add Maycoon to your Rust Project and start playing around. No extra dependencies
				needed.
			</p>
		</Card>
		<Card class="text-black">
			<h5 class="mb-2 text-2xl font-bold">Powered by Performance</h5>
			<p class="text-xl leading-tight">
				Maycoon uses the GPU for fast 2D Rendering and the CPU for parallel Task Execution and fast
				App Logic.
			</p>
		</Card>
	</div>
</main>

<style lang="scss">
	.cards {
		animation: move-in 1s 1;
	}

	@keyframes move-in {
		0% {
			transform: translateY(-100vh);
		}
	}

	.title {
		overflow: hidden;
		height: 6.75rem;
	}

	.title > .slide > div {
		padding: 0.25rem 0.75rem;
		margin-bottom: 3rem;
	}

	.title .slide:first-child {
		animation: text-animation 8s infinite;
	}

	.slide div {
		border-radius: 15px;
		background: linear-gradient(-30deg, rgb(13, 131, 241), rgb(211, 15, 211));
	}

	@keyframes text-animation {
		0% {
			margin-top: 0rem;
		}
		10% {
			margin-top: 0rem;
		}
		20% {
			margin-top: -7.25rem;
		}
		30% {
			margin-top: -7.25rem;
		}
		40% {
			margin-top: -14.5rem;
		}
		60% {
			margin-top: -14.5rem;
		}
		70% {
			margin-top: -7.25rem;
		}
		80% {
			margin-top: -7.25rem;
		}
		90% {
			margin-top: 0rem;
		}
		100% {
			margin-top: 0rem;
		}
	}
</style>
