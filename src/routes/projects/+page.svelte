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
		border: 1px solid #ddd;
		display: inline-block;
		padding: 0.35rem 1rem;
		transition: all 250ms linear;
		font-weight: lighter;
		cursor: pointer;
	}
	.view-project:hover {
		background-color: #ccc;
		color: #101010;
	}
	.projectCard:hover {
		background-color: #505050;
background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='407' height='407' viewBox='0 0 800 800'%3E%3Cg fill='none' stroke='%23BABABA' stroke-width='1'%3E%3Cpath d='M769 229L1037 260.9M927 880L731 737 520 660 309 538 40 599 295 764 126.5 879.5 40 599-197 493 102 382-31 229 126.5 79.5-69-63'/%3E%3Cpath d='M-31 229L237 261 390 382 603 493 308.5 537.5 101.5 381.5M370 905L295 764'/%3E%3Cpath d='M520 660L578 842 731 737 840 599 603 493 520 660 295 764 309 538 390 382 539 269 769 229 577.5 41.5 370 105 295 -36 126.5 79.5 237 261 102 382 40 599 -69 737 127 880'/%3E%3Cpath d='M520-140L578.5 42.5 731-63M603 493L539 269 237 261 370 105M902 382L539 269M390 382L102 382'/%3E%3Cpath d='M-222 42L126.5 79.5 370 105 539 269 577.5 41.5 927 80 769 229 902 382 603 493 731 737M295-36L577.5 41.5M578 842L295 764M40-201L127 80M102 382L-261 269'/%3E%3C/g%3E%3Cg fill='%23BABABA'%3E%3Ccircle cx='769' cy='229' r='5'/%3E%3Ccircle cx='539' cy='269' r='5'/%3E%3Ccircle cx='603' cy='493' r='5'/%3E%3Ccircle cx='731' cy='737' r='5'/%3E%3Ccircle cx='520' cy='660' r='5'/%3E%3Ccircle cx='309' cy='538' r='5'/%3E%3Ccircle cx='295' cy='764' r='5'/%3E%3Ccircle cx='40' cy='599' r='5'/%3E%3Ccircle cx='102' cy='382' r='5'/%3E%3Ccircle cx='127' cy='80' r='5'/%3E%3Ccircle cx='370' cy='105' r='5'/%3E%3Ccircle cx='578' cy='42' r='5'/%3E%3Ccircle cx='237' cy='261' r='5'/%3E%3Ccircle cx='390' cy='382' r='5'/%3E%3C/g%3E%3C/svg%3E");
color:#f1f1f1;


		transform: translate(0, -0.75rem);
	}
</style>
