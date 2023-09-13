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
	}
	.nav-list {
		width: 100%;
		display: flex;
		list-style-type: none;
		padding-left: 0;
		--_gap: 2rem;
		text-align: center;
	}
	li {
		padding-inline:calc(var(--_gap)/2);
		transition: all 200ms linear;
		position: relative;
	}
	li > a {
		text-decoration: none;
		color: var(--nav-footer);
		transition: color 200ms linear;
	}
	nav ul li::after{
		content: "";
		position: absolute;
		height: 2px;
		background-color: #303030;
		width:100%;
		bottom: -0.5rem;
		left: 0;
		scale: 0 1;
		transition: 250ms all;
	}
	li:hover::after{
		scale: 1 1;
	}
	
	/* li:hover {
		background-color: #999999;
	}
	a:hover {
		color: #f6f6f6;
	} */
	@media all and (min-width: 1600px) {
		header {
			font-size: var(--font-size-md);
		}
	}
</style>
