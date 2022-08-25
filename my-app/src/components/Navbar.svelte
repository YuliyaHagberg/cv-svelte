    <nav class="navbar">
        <div class="mainnav">
            <ul class="left">
                <li><a href="utbildning">Utbildning</a></li>
                <li><a href="erfarenhet">Erfarenhet</a></li>
            </ul>
        </div>
        <div class="logo">
            <a href="/"><img src="/yhlogo.svg" alt="Yuliya Hagberg" class="logo"/></a>
        </div>
        <div class="mainnav">
            <ul class="right">
                <li><a href="portfolio">Portfolio</a></li>
                <li><a href="about">Om mig</a></li>
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

    .mainnav {
        align-self: end;
    }

    .mainnav ul li a:hover{
        transition: 1s;
        background-color: #EFE7DD;
        border-radius: 0.3rem;
        padding: 0.3rem 0.7rem;
    }

    .navbar .logo {
        grid-row: 1 / 3;
        grid-column: 2 / 3;
        justify-self: center;
    }

    .logo img {
        width: 7rem;
        margin: 0rem;
    }

    .social {
        font-size: 0.8rem;
        color: #B29E84;
    }

    .navbar .social a:hover {
        color: #253439;
        transition: 1s;
    }

    .form-select {
        grid-column: 3 / 4;
        font-size: 0.8rem;
        border: none;
        color: #B29E84;
        cursor: pointer;
    }
</style>
    