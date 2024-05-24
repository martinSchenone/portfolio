<script>
	const projectsMap = [
		{
			cardTitle: 'ECOMMERCE' || '',
			cardDescription: 'Clothing website, with local storage and more.' || '',
			href:"https://msecommerce.netlify.app"
		},
		{
			cardTitle: 'Bufalo Burgers' || '',
			cardDescription:
				'Website for a hamburger restaurant, with the intention of attracting customers, showing a service and reaching new areas and/or people.' ||
				'',
				href:"https://bufaloburgers.netlify.app"
		},
		{
			cardTitle: 'AnimeX' || '',
			cardDescription: 'Anime site created with sveltekit using Jikan API.' || '',
			href:"https://my-anime-app.netlify.app"
		},
		{
			cardTitle: 'World Search' || '',
			cardDescription: 'World search Frontend mentor challenge,created with svelte.' || '',
			href:"https://worldsearchapp.netlify.app"
		},
		{
			cardTitle: 'Rick and morty' || '',
			cardDescription: 'Website consuming rick and morty API.' || '',
			href:"https://rickmorty-universe.netlify.app"
		}
	];
</script>

<section class="projects" id="projectos">
	<div class="section-info">
		<h1 class="section-title">Projects</h1>
		<p>Here Are Some Things I’ve Built</p>
	</div>
	{#each projectsMap as project}
		<div class="projectCard">
			<div class="cardText">
				<h1 class="cardTitle">{project.cardTitle}</h1>
				<p class="cardDescription">{project.cardDescription}</p>
				<div class="view-project">
					<button>
						<a href={project.href} target="_blank"> View project </a>
					</button>
				</div>
			</div>
		</div>
	{/each}
</section>

<style>
	.projects {
		margin: 5rem 0rem;
		width: 90%;
		max-width: 1200px;
		margin-inline: auto;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 2rem;
		border-bottom: 1.5px solid #bababa;
		padding-bottom: 5rem;
	}
	.section-title {
		font-size: clamp(2rem, 8vw + 1rem, 3.5rem);
		text-align: center;
		letter-spacing: -2px;
	}
	.projectCard {
		width: min(1200px, 60%);
		padding: 1.5rem;
		transition: all 350ms linear;
		margin: 1rem 0rem;
		cursor: default;
		border: 1px solid #ccc;
	}
	.cardTitle {
		font-weight: bold;
		align-self: flex-start;
		font-size: var(--font-size-lg);
	}
	.cardText {
		font-size: var(--font-size-sm);
		letter-spacing: 1.15px;
		line-height: 1.4;
		font-weight: 600;
	}

	.cardDescription {
		font-weight: 600;
	}
	.view-project > button,
	a {
		all: unset;
	}
	.view-project {
		opacity: 0;
		visibility: hidden;
		font-size: var(--font-size-base);
	}
	a {
		font-weight: 400;
	}

	.view-project {
		border: 1px solid #efefef;
		display: inline-block;
		padding: 0.35rem 1rem;
		transition: all 350ms linear;
		font-weight: lighter;
		cursor: pointer;
		background-color: #efefef;
		color: #252525;
	}
	.view-project:hover {
		color: #101010;
		background-color: #efefef;
	}
	.projectCard:hover {
		background-color: #232323e1;
		background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='407' height='407' viewBox='0 0 800 800'%3E%3Cg fill='none' stroke='%23BABABA' stroke-width='1'%3E%3Cpath d='M769 229L1037 260.9M927 880L731 737 520 660 309 538 40 599 295 764 126.5 879.5 40 599-197 493 102 382-31 229 126.5 79.5-69-63'/%3E%3Cpath d='M-31 229L237 261 390 382 603 493 308.5 537.5 101.5 381.5M370 905L295 764'/%3E%3Cpath d='M520 660L578 842 731 737 840 599 603 493 520 660 295 764 309 538 390 382 539 269 769 229 577.5 41.5 370 105 295 -36 126.5 79.5 237 261 102 382 40 599 -69 737 127 880'/%3E%3Cpath d='M520-140L578.5 42.5 731-63M603 493L539 269 237 261 370 105M902 382L539 269M390 382L102 382'/%3E%3Cpath d='M-222 42L126.5 79.5 370 105 539 269 577.5 41.5 927 80 769 229 902 382 603 493 731 737M295-36L577.5 41.5M578 842L295 764M40-201L127 80M102 382L-261 269'/%3E%3C/g%3E%3Cg fill='%23BABABA'%3E%3Ccircle cx='769' cy='229' r='5'/%3E%3Ccircle cx='539' cy='269' r='5'/%3E%3Ccircle cx='603' cy='493' r='5'/%3E%3Ccircle cx='731' cy='737' r='5'/%3E%3Ccircle cx='520' cy='660' r='5'/%3E%3Ccircle cx='309' cy='538' r='5'/%3E%3Ccircle cx='295' cy='764' r='5'/%3E%3Ccircle cx='40' cy='599' r='5'/%3E%3Ccircle cx='102' cy='382' r='5'/%3E%3Ccircle cx='127' cy='80' r='5'/%3E%3Ccircle cx='370' cy='105' r='5'/%3E%3Ccircle cx='578' cy='42' r='5'/%3E%3Ccircle cx='237' cy='261' r='5'/%3E%3Ccircle cx='390' cy='382' r='5'/%3E%3C/g%3E%3C/svg%3E");
		color: #f1f1f1;
		transform: translate(0, -0.5rem);
	}
	.projectCard:hover .view-project {
		opacity: 1;
		visibility: visible;
	}
</style>
