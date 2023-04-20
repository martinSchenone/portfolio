<footer id="contact">
	<div class="contactMe">
		<a class="contact1" href="/">Home</a>
		<a class="contact1" href="/projects">Projects</a>
		<a class="contact1" href="/contact">About Me</a>
	</div>
	<div class="contactMe">
		<a class="icon" href="https://wa.me/5492324685227" target="_blank">
			<span class="span-icon" id="wpp-i">
				<i class="fa-brands fa-whatsapp"/>
			</span>
		</a>
		<a class="icon" href="https://www.linkedin.com/in/martin-schenone-578241236/" target="_blank"
			><span class="span-icon" id="linkedin-i">
				<i class="fa-brands fa-linkedin-in"/>
			</span>
			</a>
		<a class="icon" href="https://github.com/martinSchenone" target="_blank">
			<span class="span-icon" id="github-i">
				<i class="fa-brands fa-github" />
			</span>
		</a>
		<a class="icon" href="mailto:martinsche2010@gmail.com" target="_blank">
			<span class="span-icon" id="mail-i">
				<i class="fa-regular fa-envelope"></i>
			</span>
		</a>
	</div>
</footer>

<!-- todo: cambiar los id de referencia hacia las rutas nuevas que tengo que crear -->
<!-- todo:crear animacion cuando le damos hover a los enlaces de redes sociales para que aparezca su icono al lado con transition -->
<style>
	footer {
		margin-top: 5rem;
		border-top: 1.5px solid #bababa;
		width: 90%;
		display: flex;
		justify-content: space-between;
		align-items: center;
		font-size: var(--font-size-base);
		color: var(--nav-footer);
		max-width: 1200px;
		margin-inline: auto;
		padding: 2rem 1rem;
	}

	.contactMe {
		display: flex;
		justify-content: center;
		align-items: center;
	}
	
	a {
		font-weight: 300;
		padding: 0.2rem 0.2rem;
		color: var(--nav-footer);
		font-weight: 400;
		text-decoration: none;
		transition: all 200ms linear;
		margin: 0rem 0.3rem;
	}
	.icon {
		padding: 0rem 0.5rem;
	}
	.contact1:hover {
		background: #999999;
		color: #f1f1f1;
	}
	.span-icon{
		color: #00000;
	}
	#wpp-i:hover{
		color:#25D366;
	}
	#github-i:hover{
		color:#adadad ;
	}
	#linkedin-i:hover{
		color:#0072b1 ;
	}
	#mail-i:hover{
		color:#c71610 ;
	}
	@media all and (max-width: 576px) {
		footer {
			flex-direction: column;
			text-align: center;
			justify-content: center;
			align-items: center;
		}
		.contactMe {
			margin-bottom: 1rem;
			text-align: center;
			font-size: var(--font-size-base);
			justify-content: center;
			align-items: center;
		}
	}
	@media all and (min-width:1600px){
        footer{
            font-size: var(--font-size-md);
        }
  }
</style>
