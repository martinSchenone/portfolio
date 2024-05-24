<section id="home">
	<div class="hero-container">
		<div class="name_surname">
			<h1 id="title_name">Martin Schenone</h1>
			<h2 id="description">Front End Developer</h2>
		</div>
		<div class="interests">
			<h3>
				Interested in the development and focused on improvement of websites, design with a
				minimalist style.
			</h3>
		</div>
		<div class="projects">
			<button class=""><a style="all:unset" href="#projectos">PROJECTS</a></button>
		</div>
	</div>
</section>

<style>
	section {
		display: flex;
		justify-content: center;
		align-items: center;
		color: #252525;
		width: 90%;
		height: 100dvh;
		font-weight: bold;
		max-width: 1200px;
		margin-inline: auto;
		border-bottom: 1.5px solid #bababa;
		animation: 0.5s showHero ease-out both;
	}

	@keyframes showHero {
		0% {
			transform: translateY(0);
		}
		100% {
			transform: translateY(-20px);
		}
	}
	.name_surname {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		font-size: var(--font-size-md);
	}
	h1 {
		margin-bottom: 0;
	}
	.interests {
		text-align: center;
		max-width: 600px;
	}
	#description {
		align-self: flex-start;
		font-style: italic;
		padding-top: 0;
		margin-top: 0;
		font-size: 13px;
	}
	#title_name {
		letter-spacing: -2px;
	}
	.hero-container {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 3rem;
	}
	.interests > h4 {
		font-weight: 400;
		line-height: 1.3;
	}
	.projects > button {
		all: unset;
		padding: 1rem;
		color: #252525;
		background-color: inherit;
		letter-spacing: -0.15px;
		cursor: pointer;
		-webkit-box-shadow: 0px 0px 20px 3px rgba(80, 80, 80, 0.42);
		-moz-box-shadow: 0px 0px 20px 3px rgba(80, 80, 80, 0.42);
		box-shadow: 0px 0px 20px 3px rgba(80, 80, 80, 0.42);
		background: #c9d6ff; /* fallback for old browsers */
		background: -webkit-linear-gradient(
			to bottom,
			#e2e2e2,
			#c9d6ff
		); /* Chrome 10-25, Safari 5.1-6 */
		background: linear-gradient(
			to bottom,
			#e2e2e2,
			#c9d6ff
		); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
		font-weight: 500;
		transition: all 250ms linear;
		opacity: 70%;
	}
	.projects > button:hover {
		opacity: 100%;
	}
	.projects > button:active {
		scale: 95%;
	}
	@media all and (min-width: 568px) {
		.name_surname {
			font-size: var(--font-size-lg);
		}
	}
	@media all and (min-width: 720px) {
		.name_surname {
			font-size: var(--font-size-xl);
		}
	}
</style>
