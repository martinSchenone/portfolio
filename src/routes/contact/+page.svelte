<script>
	const profilePic = '/photo3.png/';
	import { fly } from 'svelte/transition';
</script>

<section
	id="about"
	in:fly={{ y: 50, duration: 500, delay: 500 }}
	out:fly={{ duration: 500, delay: 500 }}
>
	<div class="container">
		<div class="yo-img">
			<img src={profilePic} alt="profilePhoto" />
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
      <span>SVELTE</span>
		</div>
	</div>
</section>

<!-- todo:poner una foto mia en el contact -->
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
  .icon-container{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .icon-container > span{
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
  .icon-container:hover span{
    transform: scale(1);
    visibility: visible;
    opacity: 1;
  }
	@media all and (max-width: 650px) {
		.container {
			flex-direction: column;
		}
	}
</style>
