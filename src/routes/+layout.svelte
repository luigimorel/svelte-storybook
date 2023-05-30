<script>
	import Footer from '../lib/components/Footer.svelte';
	import Hero from '../lib/components/Hero.svelte';
	import Navbar from '../lib/components/Navbar.svelte';
	import Services from '../lib/components/Services.svelte';
	import './../styles/app.css';
</script>

<slot />
<div class=" bg-red-400">
	<Navbar />
	<Hero />
	<Services />
	<Footer />
</div>
