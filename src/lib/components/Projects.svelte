<script>
	const projects = [
		{
			title: "Birb NFT",
			description: "A unique NFT collection featuring adorable bird characters with rare traits and utilities. Built on cutting-edge blockchain technology with a focus on community and creativity.",
			url: "https://birb-nft.tech",
			class: "birb"
		},
		{
			title: "TonFlip",
			description: "An engaging gaming platform on the TON blockchain featuring coin flip mechanics and provably fair gameplay. Experience the thrill of decentralized gaming.",
			url: "https://tonflip.bot",
			class: "tonflip"
		}
	];
</script>

<section class="projects" id="projects">
	<div class="container">
		<h2 class="section-title">Our Projects</h2>
		<p class="section-subtitle">Innovative digital experiences that showcase our passion for creativity and technology</p>
		
		<div class="projects-grid">
			{#each projects as project}
				<div class="project-card">
					<div class="project-preview {project.class}"></div>
					<div class="project-info">
						<h3 class="project-title">{project.title}</h3>
						<p class="project-description">{project.description}</p>
						<a href={project.url} target="_blank" rel="noopener noreferrer" class="project-link">
							Visit {new URL(project.url).hostname}
						</a>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>

<style>
	.projects {
		padding: 100px 20px;
		background: white;
	}

	.container {
		max-width: 1200px;
		margin: 0 auto;
	}

	.section-title {
		font-size: 2.5rem;
		font-weight: 600;
		text-align: center;
		margin-bottom: 20px;
		color: #333;
	}

	.section-subtitle {
		font-size: 1.1rem;
		text-align: center;
		color: #666;
		margin-bottom: 60px;
		max-width: 600px;
		margin-left: auto;
		margin-right: auto;
	}

	.projects-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
		gap: 40px;
		margin-top: 60px;
	}

	.project-card {
		background: white;
		border-radius: 20px;
		overflow: hidden;
		box-shadow: 0 10px 30px rgba(0,0,0,0.1);
		transition: all 0.3s ease;
		border: 1px solid #eee;
	}

	.project-card:hover {
		transform: translateY(-10px);
		box-shadow: 0 20px 40px rgba(0,0,0,0.15);
	}

	.project-preview {
		height: 250px;
		background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
		position: relative;
		overflow: hidden;
	}

	.project-preview.birb {
		background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
	}

	.project-preview.tonflip {
		background: linear-gradient(135deg, #fa709a 0%, #fee140 100%);
	}

	.project-preview::before {
		content: '';
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		width: 80px;
		height: 80px;
		background: rgba(255,255,255,0.2);
		border-radius: 50%;
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.project-info {
		padding: 30px;
	}

	.project-title {
		font-size: 1.5rem;
		font-weight: 600;
		margin-bottom: 15px;
		color: #333;
	}

	.project-description {
		color: #666;
		margin-bottom: 25px;
		line-height: 1.6;
	}

	.project-link {
		display: inline-block;
		background: #ff8000;
		color: white;
		padding: 12px 25px;
		border-radius: 25px;
		text-decoration: none;
		font-weight: 500;
		transition: all 0.3s ease;
	}

	.project-link:hover {
		background: #e67300;
		transform: translateY(-2px);
	}

	@media (max-width: 768px) {
		.projects-grid {
			grid-template-columns: 1fr;
		}

		.section-title {
			font-size: 2rem;
		}
	}
</style> 