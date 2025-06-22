<script>
	import { onMount } from 'svelte';
	
	let isVisible = false;
	
	onMount(() => {
		const handleScroll = () => {
			isVisible = window.scrollY > 100;
		};
		
		window.addEventListener('scroll', handleScroll);
		
		return () => {
			window.removeEventListener('scroll', handleScroll);
		};
	});
	
	function scrollToSection(sectionId) {
		const element = document.getElementById(sectionId);
		if (element) {
			element.scrollIntoView({ behavior: 'smooth' });
		}
	}
</script>

<nav class="navbar" class:visible={isVisible}>
	<div class="nav-container">
		<img src="/logos/MARBALABS/Logo Files/For Web/svg/White logo - no background.svg" alt="MarbaLabs" class="nav-logo">
		<ul class="nav-links">
			<li><button on:click={() => scrollToSection('home')}>Home</button></li>
			<li><button on:click={() => scrollToSection('about')}>About</button></li>
			<li><button on:click={() => scrollToSection('projects')}>Projects</button></li>
			<li><button on:click={() => scrollToSection('contact')}>Contact</button></li>
		</ul>
	</div>
</nav>

<style>
	.navbar {
		position: fixed;
		top: 0;
		width: 100%;
		background: rgba(0, 0, 0, 0.9);
		backdrop-filter: blur(10px);
		z-index: 1000;
		padding: 15px 0;
		transition: all 0.3s ease;
		transform: translateY(-100%);
	}

	.navbar.visible {
		transform: translateY(0);
	}

	.nav-container {
		max-width: 1200px;
		margin: 0 auto;
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 0 20px;
	}

	.nav-logo {
		height: 35px;
	}

	.nav-links {
		display: flex;
		list-style: none;
		gap: 30px;
		margin: 0;
		padding: 0;
	}

	.nav-links button {
		background: none;
		border: none;
		color: white;
		font-weight: 500;
		cursor: pointer;
		transition: color 0.3s ease;
		font-size: 1rem;
		padding: 5px 10px;
	}

	.nav-links button:hover {
		color: #ff8000;
	}

	@media (max-width: 768px) {
		.nav-links {
			display: none;
		}
	}
</style> 