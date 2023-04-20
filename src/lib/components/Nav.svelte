
<header>
    <div class="nav-cont">
        <nav class="nav">
            <ul class="nav-list">
                <li><a href="/">Home</a></li>
                <li><a href="/projects">Projects</a></li>
                <li><a href="/contact">About me</a></li>
            </ul>
        </nav>
    </div>
   
</header>


<style>
    header{
        border-bottom: 1.5px solid #bababa;
        width: 90%;
        display: flex;
        align-items: center;
        justify-content: center;
        max-width: 1200px;
        margin-inline: auto;
    }
   
    .nav-list{
        width: 100%;
        display: flex;
        list-style-type: none;
        padding-left: 0;
        gap: 1rem;
    
    }
    li{
        transition:all 200ms linear;
        padding: 0.1rem 0.3rem;
    }
    li>a{
        text-decoration: none;
        color: var(--nav-footer);
        transition: color 200ms linear;

    }
    li:hover{
        background-color: #999999;
    }
    a:hover{
        color: #f1f1f1;
    }
    @media all and (min-width:1600px){
        header{
            font-size: var(--font-size-md);
        }
  }
</style>