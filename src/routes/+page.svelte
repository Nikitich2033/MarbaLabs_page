<script>
	import Navbar from '$lib/components/Navbar.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import About from '$lib/components/About.svelte';
	import Projects from '$lib/components/Projects.svelte';
	import Contact from '$lib/components/Contact.svelte';
	import Footer from '$lib/components/Footer.svelte';

	function scrollToProjects() {
		const element = document.getElementById('projects');
		if (element) {
			element.scrollIntoView({ behavior: 'smooth' });
		}
	}
</script>

<svelte:head>
	<title>Marba Labs - Creative Digital Solutions</title>
	<meta name="description" content="A collective of artists, developers, and designers based in Marbella and London, bringing extraordinary ideas to life through blockchain and digital experiences." />
</svelte:head>

<Navbar />
<Hero {scrollToProjects} />
<About />
<Projects />
<Contact />
<Footer />

<style>
	:global(*) {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	:global(body) {
		font-family: 'Inter', sans-serif;
		line-height: 1.6;
		color: #333;
		overflow-x: hidden;
	}

	:global(html) {
		scroll-behavior: smooth;
	}
</style>
