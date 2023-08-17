<header>
	<nav class="nav">
		<ul class="nav-list">
			<li><a href="#home">Home</a></li>
			<li><a href="#projectos">Projects</a></li>
			<li><a href="#contact">About me</a></li>
		</ul>
	</nav>
</header>

<style>
	header {
		border-bottom: 1.5px solid #bababa;
		width: 90%;
		display: flex;
		align-items: center;
		justify-content: center;
		max-width: 1200px;
		margin-inline: auto;
	}
	.nav {
		width: 100%;
	}
	.nav-list {
		width: 100%;
		display: flex;
		justify-content: space-evenly;
		list-style-type: none;
		padding-left: 0;
		gap: 1rem;
		text-align: center;
	}
	li {
		padding: 0.5rem;
		transition: all 200ms linear;
	}
	li > a {
		text-decoration: none;
		color: var(--nav-footer);
		transition: color 200ms linear;
	}
	li:hover {
		background-color: #999999;
	}
	a:hover {
		color: #f6f6f6;
	}
	@media all and (min-width: 1600px) {
		header {
			font-size: var(--font-size-md);
		}
	}
</style>
