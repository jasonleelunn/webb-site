<script>
	import '../app.css';
	import Header from './Header.svelte';
	import Footer from './Footer.svelte';
</script>

<Header />
<slot />
<Footer />

<style lang="postcss">
	:global(html) {
		background-color: theme(colors.gray.800);
	}
</style>
