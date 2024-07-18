<script lang="ts">
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
</script>

<Navbar class="fixed w-full border-b-4">
	<NavBrand href="/">
		<img src="favicon.png" class="h-12" alt="Maycoon Logo" />
		<span class="pl-10 text-2xl">Maycoon</span>
	</NavBrand>
	<NavHamburger />
	<NavUl>
		<NavLi href="/" class="text-2xl">Home</NavLi>
		<NavLi href="/about" class="text-2xl">About</NavLi>
		<NavLi href="https://maycoon-ui.github.io/guide" class="text-2xl">Guide</NavLi>
		<NavLi href="https://docs.rs/maycoon" target="_blank" class="text-2xl">Docs</NavLi>
		<NavLi href="/community" class="text-2xl">Community</NavLi>
	</NavUl>
</Navbar>
