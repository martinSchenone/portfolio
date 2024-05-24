<script>
	import Footer from '../lib/components/Footer.svelte';
	import Nav from '../lib/components/Nav.svelte';
</script>

<title>Martin Schenone / Portfolio</title>

<Nav />
<slot />
<Footer />

<style>
	@import url('https://fonts.googleapis.com/css2?family=Azeret+Mono:wght@100;200;300;400;500;600;700&display=swap');
	:global(*) {
		font-family: 'Azeret Mono', monospace;
	}
</style>
