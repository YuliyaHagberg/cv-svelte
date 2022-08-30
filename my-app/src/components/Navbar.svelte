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
        border-radius: 0.28rem;
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
            gap: 0em;
            grid-template-columns: 0.9fr 1.1fr 1fr 1.1fr 0.9fr;
            grid-row: 1;
            height: 4.2em;}
        .mainnav {align-self: center;}
        .mainnav ul li a{padding: 0.5rem 0.7rem;}
        .navbar .logo {grid-column: 3 / 4;
            grid-row: 1 / 2;
            align-self: center;}
        .logo img {width: 6.5rem; grid-row: 1;}
        .social {font-size: 0.9rem;
            grid-column: 1 / 2;
            grid-row: 1 / 2;
            align-self: center;}
        .social a {margin: 0rem 0.15rem;}
        .form-select {
            grid-column: 5 / 6;
            font-size: 0.9rem;
            align-self: center;}
        .navbar .mainnav .left {grid-column: 2 / 3; justify-content: space-evenly;}
        .navbar .mainnav .right {grid-column: 4 / 5; justify-content: space-evenly;}
    }
    @media only screen and (min-width: 860px) {
        .social {font-size: 1rem;}
        .form-select {font-size: 1rem;}
        .navbar .left, .right {
            display: flex;
            gap: 1rem;
            justify-content: center;
        }
    }
    @media only screen and (min-width: 1200px) {
        .social {font-size: 1.1rem;}
        .form-select {font-size: 1.1rem;}
        .navbar .left, .right {gap: 1.1rem;}
        .navbar ul li {font-size: 1.1rem;}
    }
    @media only screen and (min-width: 1600px) {
        .social {font-size: 1.4rem;}
        .form-select {font-size: 1.4rem;}
        .navbar .left, .right {gap: 1.4rem;}
        .navbar ul li {font-size: 1.4rem;}
        .navbar {height: 5em;}
        .logo img {width: 8rem;}
    }
</style> 