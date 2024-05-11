<script lang="ts">
	import Nav from '$lib/components/Nav.svelte';
	import { Card } from 'flowbite-svelte';
</script>

<Nav />
<main class="grid place-content-center">
	<div class="title flex justify-center text-6xl">
		About
		<div class="gradient-title text-white">Maycoon</div>
	</div>

	<div class="cards mt-20 flex">
		<Card class="mr-16 text-black">
			<h5 class="mb-2 text-xl font-bold">What is Maycoon?</h5>
			<p class="text-xl leading-tight">
				Maycoon is a modern framework for developing cross-platform Apps with beautiful UI and fast
				app logic. It is written in Rust and utilizes the GPU for optimal drawing operations.
			</p>
		</Card>
		<Card class="mr-16 text-black">
			<h5 class="mb-2 text-xl font-bold">What can I develop Apps for?</h5>
			<p class="text-xl leading-tight">
				Right now, we only support Desktop platforms (macOS, linux, Windows and maybe more), but
				there are thoughts about making Maycoon Apps portable to the Web or other platforms.
			</p>
		</Card>
		<Card class="text-black">
			<h5 class="mb-2 text-xl font-bold">Why use Rust?</h5>
			<p class="text-xl leading-tight">
				Maycoon is coded in Rust for optimal performance. While not ideal for UI work, Rust is
				perfect for performance and efficient memory efficiency. We also think about making bindings
				to other languages like Python or C/C++.
			</p>
		</Card>
	</div>

	<div class="cards mt-20 flex">
		<Card class="mr-16 text-black">
			<h5 class="mb-2 text-xl font-bold">Is this production ready?</h5>
			<p class="text-xl leading-tight">
				Maycoon is still in its Beta Phase and won't get to its first real release soon, so it's
				definetely not production ready and breaking changes may occur at any moment. You may want
				to use this for experiments, but not for 'real' ready-to-ship Apps.
			</p>
		</Card>
		<Card class="mr-16 text-black">
			<h5 class="mb-2 text-xl font-bold">What are alternatives?</h5>
			<p class="text-xl leading-tight">
				There are some nice UI frameworks to develop fast Apps in Rust. Notably
				<a href="https://github.com/emilk/egui" target="_blank">egui</a> or
				<a href="https://github.com/iced-rs/iced" target="_blank">iced</a>. If you want some
				Non-Rust alternatives, then you may be interested in
				<a href="https://www.qt.io" target="_blank">Qt</a> for C++, Python and other languages or
				<a href="https://flutter.dev" target="_blank">Flutter</a> for the Dart language.
			</p>
		</Card>
		<Card class="text-black">
			<h5 class="mb-2 text-xl font-bold">When is this going to get production-ready?</h5>
			<p class="text-xl leading-tight">
				We don't have a real ETA for the 1.0.0 Release, but you can always check out our
				<a href="https://github.com/maycoon-ui/maycoon" target="_blank">Git Repo</a> for the latest commits.
				If you want development to speed up, you can always contribute with code or just by giving us
				feedback on the latest changes.
			</p>
		</Card>
	</div>

	<div class="cards mb-32 mt-20 flex">
		<Card class="mr-16 text-black">
			<h5 class="mb-2 text-xl font-bold">Who develops Maycoon?</h5>
			<p class="text-xl leading-tight">
				Maycoon is mainly developed by <a href="https://drafteddev.github.io" target="_blank"
					>Mikail Plotzky</a
				> and any Maycoon contributors. Feel free to join us on our journey and add your awesome code!
			</p>
		</Card>
		<Card class="mr-16 text-black">
			<h5 class="mb-2 text-xl font-bold">How does Maycoon work under the hood?</h5>
			<p class="text-xl leading-tight">
				We use modern technology such as <a
					href="https://github.com/femtovg/femtovg"
					target="_blank">Modern GPU-powered Vector Graphics</a
				>, async task execution and the <a href="https://rust-lang.org" target="_blank">Rust</a> Programming
				language.
			</p>
		</Card>
		<Card class="text-black">
			<h5 class="mb-2 text-xl font-bold">Is Maycoon free-to-use?</h5>
			<p class="text-xl leading-tight">
				Maycoon is dual licensed under the MIT and Apache 2.0 License which makes it free to use for
				everyone. There is no price for awesome UIs. Just try it!
			</p>
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
