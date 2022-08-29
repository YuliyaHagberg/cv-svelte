    <nav class="navbar">
        <div class="mainnav">
            <ul class="left">
                <li><a href="portfolio">Portfolio</a></li>
                <li><a href="about">Om mig</a></li>
            </ul>
        </div>
        <div class="logo">
            <a href="/"><img src="/yhlogo.svg" alt="Yuliya Hagberg" class="logo"/></a>
        </div>
        <div class="mainnav">
            <ul class="right">
                <li><a href="utbildning">Utbildning</a></li>
                <li><a href="erfarenhet">Erfarenhet</a></li>
            </ul>
        </div>
        <div class="social">
            <a href="mailto:yuliya.swe@gmail.com"><i class="fa-solid fa-envelope fa-lg"></i></a>
            <a href="https://linkedin.com/in/yuliyahagberg/" target="_blank"><i class="fa-brands fa-linkedin fa-lg"></i></a>
            <a href="https://github.com/YuliyaHagberg" target="_blank"><i class="fa-brands fa-github fa-lg"></i></a>
        </div>
        <div class="form-select">
            <select id="language" class="form-select" name="language"> 
                <option>SE</option>
                <!-- <option>EN</option>
                <option>UA</option>
                <option>RU</option> -->
            </select>
        </div>
    </nav>

<style>
    .navbar {
        gap: 0.2em;
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        height: 5em;
        font-family:'Coco-Gothic', light;
        text-align: center;
    }
    .mainnav {align-self: end;}
    .mainnav ul li a:hover{
        transition: 0.8s;
        background-color: #EFE7DD;
        border-radius: 0.3rem;
    }
    .navbar .logo {
        grid-row: 1 / 3;
        grid-column: 2 / 3;
        justify-self: center;
    }
    .logo img {width: 7rem; margin: 0rem;}
    .social {font-size: 0.8rem; color: #B29E84;}
    .navbar .social a:hover {color: #253439; transition: 1s;}
    .form-select {
        grid-column: 3 / 4;
        font-size: 0.8rem;
        border: none;
        color: #B29E84;
        cursor: pointer;
    }

    @media only screen and (min-width: 640px) {
        .navbar {
            gap: 0.2em;
            grid-template-columns: repeat(5, 1fr);
            grid-row: 1;
            height: 4.2em;}
        .mainnav ul li a:hover{
            border-radius: 0.25rem;
            padding: 0.4rem 0.7rem;
        }
        .mainnav {align-self: center;}
        .navbar .logo {grid-column: 3 / 4;
            grid-row: 1 / 2;
            align-self: center;}
        .logo img {width: 6.5rem;
            grid-row: 1;}
        .social {font-size: 0.9rem;
            grid-column: 1 / 2;
            grid-row: 1 / 2;
            align-self: center;}
        .form-select {
            grid-column: 5 / 6;
            font-size: 0.9rem;
            align-self: center;}
        .navbar .mainnav .left {grid-column: 2 / 3;}
        .navbar .mainnav .right {grid-column: 4 / 5;}
    }
    @media only screen and (min-width: 860px) {
        .social {font-size: 1rem;}
        .form-select {font-size: 1rem;}
        .navbar .left, .right {
            display: flex;
            gap: 2.5rem;
            justify-content: center;
        }
    }
    @media only screen and (min-width: 1200px) {}
    @media only screen and (min-width: 1600px) {}
</style> 