<section id="contact">
	<div class="about_me_title">
		<h1>About Me</h1>
	</div>
	<div class="container">
		<div class="yo-img">
			<img src="./photo3.png" alt="profilePhoto" />
		</div>
		<div class="about-me">
			<p class="text">Hey, I'm Martin. Frontend developer</p>

			<p>
				Passionate about programming, I love finding new methods to solve the problems that come my
				way.
			</p>
			These are the technologies that I use daily to develop
			<p />
		</div>
	</div>

	<div class="icons">
		<div class="icon-container">
			<img
				src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg"
				alt="logo"
			/>
			<span class="span">HTML</span>
		</div>
		<div class="icon-container">
			<img
				src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg"
				alt="logo"
			/>
			<span>CSS</span>
		</div>

		<div class="icon-container">
			<img
				src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg"
				alt="logo"
			/>
			<span>JAVASCRIPT</span>
		</div>
		<div class="icon-container">
			<img
				src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg"
				alt="logo"
			/>
			<span>NODE JS</span>
		</div>
		<div class="icon-container">
			<img
				src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/svelte/svelte-original.svg"
				alt="logo"
			/>
			<span>SVELTEKIT</span>
		</div>
		<div class="icon-container">
			<img
				src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tailwindcss/tailwindcss-plain.svg"
				alt="logo"
			/>
			<span>TAILWIND</span>
		</div>
		<div class="icon-container">
			<img
				src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg"
				alt="logo"
			/>
			<span>REACT</span>
		</div>
	</div>
	<div class="cv">
		<button type="button"><a href="./cv12-12.pdf" download>Download CV</a></button>
	</div>
</section>

<style>
	section {
		width: 90%;
		margin-top: 8rem;
		margin-bottom: 5rem;
		color: var(--nav-footer);
		max-width: 1200px;
		margin-inline: auto;
	}
	.about_me_title {
		text-align: center;
		font-size: var(--font-size-lg);
		letter-spacing: -2px;
	}
	.container {
		width: 100%;
		display: flex;
		margin-top: 5rem;
	}
	.yo-img {
		display: flex;
		justify-content: center;
		align-items: center;
		width: 100%;
		padding-bottom: 2rem;
	}
	.yo-img > img {
		width: 250px;
		border-radius: 10rem;
		object-fit: cover;
	}

	.about-me {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		width: 100%;
		text-align: center;
		font-size: var(--font-size-base);
		font-weight: 500;
		letter-spacing: 0.15px;
		line-height: 1.3;
		padding-bottom: 2rem;
	}
	.about-me > p {
		padding: 0rem 2.5rem;
	}

	.icons {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
		margin-top: 5rem;
		gap: 3rem;
		padding: 0.5rem;
	}
	.icon-container {
		display: flex;
		flex-direction: column;
		justify-content: center;
		position: relative;
		align-items: center;
	}
	.icon-container > span {
		opacity: 0;
		visibility: hidden;
		width: 100%;
		height: 100%;
		display: flex;
		justify-content: center;
		align-items: center;
		transition: all 250ms 100ms linear;
		font-weight: bold;
		transform: scale(1);
		letter-spacing: -2px;
		position: absolute;
		font-size: 2rem;
		text-align: center;
		z-index: 0;
	}
	.icons > .icon-container > img {
		transition: all 250ms linear;
		overflow: hidden;
		padding: 1rem;
		height: 100%;
		cursor: pointer;
	}
	.icons > .icon-container > img:hover {
		transform: scale(105%);
		opacity: 10%;
	}
	img {
		width: 100%;
		height: 100%;
		z-index: 10;
	}
	.icon-container:hover span {
		transform: scale(1);
		visibility: visible;
		opacity: 1;
	}
	.cv {
		margin-top: 7rem;
		display: flex;
		justify-content: center;
		align-items: center;
	}
	.cv > button {
		border: none;
		padding: 0.9rem 0rem;
		color: #252525;
		cursor: pointer;
		background: #c9d6ff;
		background: -webkit-linear-gradient(to bottom, #e2e2e2, #c9d6ff);
		background: linear-gradient(to bottom, #e2e2e2, #c9d6ff);
		-webkit-box-shadow: 0px 0px 20px 3px rgba(80, 80, 80, 0.42);
		-moz-box-shadow: 0px 0px 20px 3px rgba(80, 80, 80, 0.42);
		box-shadow: 0px 0px 20px 3px rgba(80, 80, 80, 0.42);
		font-weight: lighter;
		transition: all 500ms linear;
		font-size: var(--font-size-base);
		font-weight: 500;
		opacity: 0.7;
	}
	a {
		padding: 0.9rem;
	}
	.cv > button:hover {
		opacity: 1;
	}
	.cv > button:active {
		scale: 95%;
	}
	a {
		letter-spacing: -0.15px;
		text-decoration: none;
		font-weight: 700;
		color: #252525;
		transition: all 500ms linear;
	}

	@media all and (max-width: 650px) {
		.container {
			flex-direction: column;
		}
	}
</style>
