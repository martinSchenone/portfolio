<script>
	import { fly } from 'svelte/transition';
</script>

<div in:fly={{ y: 50, duration: 500, delay: 500 }} out:fly={{ duration: 500, delay: 500 }}>
	<section class="projects">
		<div class="section-info">
			<h1 class="section-title">Projects</h1>
			<p>Here are some of my projects that I have worked on.</p>
		</div>
		<div class="projectCard">
			<div class="cardText">
				<h1 class="cardTitle">AnimeX</h1>
				<p class="cardDescription">Anime site created with sveltekit using Jikan API.</p>
				<div class="view-project">
					<button>
						<a href="https://my-anime-app.netlify.app/anime" target="_blank"> View project </a>
					</button>
				</div>
			</div>
		</div>
		<div class="projectCard">
			<div class="cardText">
				<h1 class="cardTitle">World Search</h1>
				<p class="cardDescription">World search Frontend mentor challenge,created with svelte.</p>
				<div class="view-project">
					<button><a href="https://worldsearchapp.netlify.app" target="_blank">View Project</a></button>
				</div>
			</div>
		</div>
		<div class="projectCard">
			<div class="cardText">
				<h1 class="cardTitle">Rick and morty</h1>
				<p class="cardDescription">Website consuming rick and morty API</p>
				<div class="view-project">
					<button>
						<a href="https://rickmorty-universe.netlify.app" target="_blank"> View project </a>
					</button>
				</div>
			</div>
		</div>
	</section>
</div>

<style>
	.section-title {
		font-size: clamp(2rem, 8vw + 1rem, 3.5rem);
		text-align: center;
	}
	.projects {
		margin-top: 5rem;
		width: 90%;
		max-width: 1200px;
		margin-inline: auto;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 4rem;
	}
	.projectCard {
		width: min(50%, 1200px);
		padding: 1.5rem;
		border-radius: 0.5rem;
		transition: all 250ms linear;
	}
	.cardText {
		font-size: var(--font-size-base);
		letter-spacing: 0.1rem;
	}
	.cardTitle {
		font-weight: bold;
		align-self: flex-start;
	}
	.cardDescription {
		font-weight: 400;
	}
	.view-project > button,
	a {
		all: unset;
	}
	.view-project {
		border: 1px solid #000;
		display: inline-block;
		border-radius: 1rem;
		padding: 0.35rem 1rem;
		transition: all 250ms linear;
		font-weight: lighter;
		cursor: pointer;
	}
	.view-project:hover {
		background-color: #cdbafa;
		border-color: #cdbafa;
	}
	.projectCard:hover {
		background: #d3cce3; /* fallback for old browsers */
		background: -webkit-linear-gradient(
			to right,
			#e9e4f0,
			#d3cce3
		); /* Chrome 10-25, Safari 5.1-6 */
		background: linear-gradient(
			to right,
			#e9e4f0,
			#d3cce3
		); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

		transform: translate(0, -0.75rem);
	}
</style>
