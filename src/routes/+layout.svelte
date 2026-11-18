<script lang="ts">
	import './layout.css';
	import favicon from '#lib/assets/HB3 favicon.svg';
	import type { LayoutProps } from './$types';
	import Header from './components/Header.svelte';

	let { children }: LayoutProps = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}

<Header />