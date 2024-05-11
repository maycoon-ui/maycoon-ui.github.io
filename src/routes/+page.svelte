<script lang="ts">
	import Nav from '$lib/components/Nav.svelte';
	import { Card } from 'flowbite-svelte';
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

	<div class="cards mt-72 flex">
		<Card class="mr-16 text-black">
			<h5 class="mb-2 text-2xl font-bold">Beautiful</h5>
			<p class="text-xl leading-tight">
				Use a palette of well-designed and beautiful built-in Widgets to design your dream UI.
			</p>
		</Card>
		<Card class="mr-16 text-black">
			<h5 class="mb-2 text-2xl font-bold">Plug'n'Play</h5>
			<p class="text-xl leading-tight">
				Add Maycoon to your Cargo Project and start playing around without extra dependencies.
			</p>
		</Card>
		<Card class="text-black">
			<h5 class="mb-2 text-2xl font-bold">Powered by Performance</h5>
			<p class="text-xl leading-tight">
				Maycoon utilized the GPU and parallel task execution to make your App lightning fast.
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
