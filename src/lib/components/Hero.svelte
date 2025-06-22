<script>
	export let scrollToProjects = () => {};
</script>

<section class="hero" id="home">
	<div class="hero-content">
		<img src="/logos/MARBALABS/Logo Files/For Web/svg/White logo - no background.svg" alt="MarbaLabs" class="logo">
		<h1>Marba Labs</h1>
		<p>A collective of artists, developers, and designers bringing extraordinary ideas to life</p>
		<button on:click={scrollToProjects} class="cta-button">View Our Work</button>
	</div>
</section>

<style>
	.hero {
		height: 100vh;
		background: linear-gradient(135deg, #ff8000 0%, #ff6b35 100%);
		display: flex;
		align-items: center;
		justify-content: center;
		position: relative;
		overflow: hidden;
	}

	.hero::before {
		content: '';
		position: absolute;
		top: 0;
		left: 0;
		right: 0;
		bottom: 0;
		background: url('/logos/orange-transformed.png') no-repeat center center;
		background-size: cover;
		opacity: 0.1;
		z-index: 1;
	}

	.hero-content {
		text-align: center;
		color: white;
		z-index: 2;
		position: relative;
		max-width: 800px;
		padding: 0 20px;
	}

	.logo {
		height: 120px;
		margin-bottom: 30px;
		filter: drop-shadow(0 4px 8px rgba(0,0,0,0.2));
	}

	.hero h1 {
		font-size: 3.5rem;
		font-weight: 700;
		margin-bottom: 20px;
		background: linear-gradient(45deg, #fff, #ffebb3);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
		background-clip: text;
	}

	.hero p {
		font-size: 1.3rem;
		font-weight: 300;
		margin-bottom: 40px;
		opacity: 0.95;
	}

	.cta-button {
		background: rgba(255, 255, 255, 0.2);
		color: white;
		padding: 15px 35px;
		border-radius: 50px;
		border: 2px solid rgba(255, 255, 255, 0.3);
		cursor: pointer;
		font-weight: 500;
		backdrop-filter: blur(10px);
		transition: all 0.3s ease;
		font-size: 1rem;
	}

	.cta-button:hover {
		background: rgba(255, 255, 255, 0.3);
		transform: translateY(-2px);
		box-shadow: 0 10px 20px rgba(0,0,0,0.2);
	}

	@media (max-width: 768px) {
		.hero h1 {
			font-size: 2.5rem;
		}

		.hero p {
			font-size: 1.1rem;
		}
	}
</style> 