<script>
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
	import Fa from 'svelte-fa';
	import { faClock } from '@fortawesome/free-solid-svg-icons';
</script>

<div class="relative px-8">
	<Navbar
		navClass="px-2 sm:px-4 py-2.5 absolute w-full z-20 top-0 left-0 border-b"
		let:hidden
		let:toggle
	>
		<NavBrand href="/">
			<Fa icon={faClock} class="text-xl mr-2" />
			<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white"
				>OpenTimeTracker</span
			>
		</NavBrand>
		<NavHamburger on:click={toggle} />
		<NavUl {hidden}>
			<NavLi href="/" active={true}>Home</NavLi>
			<NavLi href="/card">Time Card</NavLi>
			<NavLi href="/sheets">Time Sheets</NavLi>
			<NavLi href="/settings">Settings</NavLi>
		</NavUl>
	</Navbar>
</div>
