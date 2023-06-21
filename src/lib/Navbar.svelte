<script>
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
	import Fa from 'svelte-fa';
	import { faClock, faHouse, faNoteSticky, faCog } from '@fortawesome/free-solid-svg-icons';
	import { DarkMode } from 'flowbite-svelte';
</script>

<div class="relative min-w-full">
<DarkMode initialTheme="dark" class="hidden"/>
	<Navbar
	navClass="px-2 sm:px-4 py-2.5 z-20 top-0 left-0 border-b"
	let:hidden
	let:toggle
>
	<NavBrand href="/">
		<Fa icon={faClock} class="text-xl mx-2" />
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white"
			>OpenTimeTracker</span
		>
	</NavBrand>
	<NavHamburger on:click={toggle} />
	<NavUl {hidden}>
		<NavLi href="/" active={true} class="flex flex-row items-center">
			<Fa icon={faHouse} class="mr-2" />
			Home
		</NavLi>
		<NavLi href="/card" class="flex flex-row items-center">
			<Fa icon={faClock} class="mr-2" />
			Time Card
		</NavLi>
		<NavLi href="/sheets" class="flex flex-row items-center"
			><Fa icon={faNoteSticky} class="mr-2" />Time Sheets</NavLi
		>
		<NavLi href="/settings" class="flex flex-row items-center">
			<Fa icon={faCog} class="mr-2" />
			Settings
		</NavLi>
	</NavUl>
</Navbar>
</div>
