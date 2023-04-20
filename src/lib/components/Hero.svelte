<section id="home">
  <div class="hero-container">
    <h1>Hello,I'm Martin.</h1>
    <h2>A Frontend Developer</h2>
    <p>I'm interested in the development and improvement of websites, with a minimalist design perspective.</p>
    <span><a style="all:unset" href="/projects">PROJECTS</a></span>
  </div>
</section>
<!-- todo: Poner una imagen mia ya sea o diseño creado por ia de fondo en la izq o derecha -->

<style>
  section {
    display: flex;
    justify-content: center;
    align-items: center;
    color: #000000;
    width: 90%;
    height: 90vh;
    font-weight: bold;
    max-width: 1200px;
    margin-inline: auto;
  }
  h1{
    font-weight: bold;
    font-size: var(--font-size-lg);
  }
  h2{
    font-weight: 300;
    font-size: var(--font-size-md);
  }
  .hero-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .hero-container > p {
    font-size: var(--font-size-base);
    font-weight: 300;
    padding:0rem 3rem;
  }
  .hero-container > span {
    margin-top: 1rem;
    padding: 1rem; 
    color: #202020;
    background-color: inherit;
    letter-spacing: 0.3rem;
    cursor: pointer;
    -webkit-box-shadow: 0px 0px 24px 11px rgba(80, 80, 80, 0.42);
    -moz-box-shadow: 0px 0px 24px 11px rgba(80, 80, 80, 0.42);
    box-shadow: 0px 0px 24px 11px rgba(80, 80, 80, 0.42);
    font-weight: lighter;
    transition: all 500ms linear;
  }
  .hero-container> span:hover{
    background:rgb(51, 51, 51);
    color: white;
    transition: all 100ms;
  }
  p,
  h2,
  h1 {
    text-align: center;
  }

  @media all and (min-width:1600px){
    h1{
      font-size: var(--font-size-xl);
    }
    h2{
      font-size: var(--font-size-lg);
    }
    .hero-container > p{
      font-size: var(--font-size-md);
    }
    .hero-container > span{
      font-size: var(--font-size-md);
    }
  }
</style>
