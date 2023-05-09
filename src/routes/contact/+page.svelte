<script>
	import { fly } from 'svelte/transition';
</script>

<section
	id="about"
	in:fly={{ y: 50, duration: 500, delay: 500 }}
	out:fly={{ duration: 500, delay: 500 }}
>
	<div class="container">
		<div class="yo-img">
			<img src="./photo3.png" alt="profilePhoto" />
		</div>
		<div class="about-me">
			<p>
				Hey, I'm Martin. I'm Frontend developer
				<br />
				I am passionate about programming, I love finding new methods to solve problems that come my
				way.
				<br />
				These are the technologies that I use daily to program
			</p>
		</div>
	</div>

	<div class="icons">
		<div class="icon-container">
			<img
				src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg"
				alt="logo"
			/>
			<span>HTML</span>
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
				src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg"
				alt="logo"
			/>
			<span>BOOTSTRAP</span>
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
	</div>
	<div class="cv">
		<button type="button"><a href="./cv.pdf" download>Download CV</a></button>
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
	.container {
		width: 100%;
		display: flex;
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
		justify-content: center;
		align-items: center;
		width: 100%;
		text-align: center;
		font-size: var(--font-size-base);
		font-weight: 500;
		letter-spacing: 0.1rem;
		word-spacing: 0.1rem;
		padding-bottom: 2rem;
	}
	.about-me > p {
		padding: 0rem 2.5rem;
	}
	.icons {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
		gap: 1rem 2rem;
		margin-top: 5rem;
	}
	.icon-container {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.icon-container > span {
		visibility: hidden;
		opacity: 0;
		transition: all 500ms linear;
		font-weight: bold;
		transform: scale(0);
	}
	.icons > .icon-container > img {
		margin: 1rem 1rem;
		transition: all 250ms linear;
		overflow: hidden;
		padding: 1rem;
		border-radius: 1rem;
	}
	.icons > .icon-container > img:hover {
		transform: scale(1.05);
	}
	.icon-container:hover span {
		transform: scale(1);
		visibility: visible;
		opacity: 1;
	}
	.cv{
		margin-top: 3rem;
		display: flex;
		justify-content: center;
		align-items: center;
	}
	.cv > button{
    padding: 1rem; 
    color: #202020;
    background-color: inherit;
    letter-spacing: 0.1rem;
    cursor: pointer;
    -webkit-box-shadow: 0px 0px 24px 11px rgba(80, 80, 80, 0.42);
    -moz-box-shadow: 0px 0px 24px 11px rgba(80, 80, 80, 0.42);
    box-shadow: 0px 0px 24px 11px rgba(80, 80, 80, 0.42);
    font-weight: lighter;
    transition: all 500ms linear;
	font-size: var(--font-size-base);
	font-weight: 700;
	}
  .cv> button:hover{
    background:rgb(51, 51, 51);
    color: white;
    transition: all 100ms;
  }
  a{
	text-decoration: none;
	color: #202020;
  }
	@media all and (max-width: 650px) {
		.container {
			flex-direction: column;
		}
	}
</style>
