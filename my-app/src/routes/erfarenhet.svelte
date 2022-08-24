<script>
    import Navbar from "../components/Navbar.svelte"
    import Footer from "../components/Footer.svelte"
    import Button from "../components/Button.svelte"
</script>

<Navbar/>

<section class="erfarenhet">
    <div class="flex-container">
        <div class="aside">
            <a href="https://github.com/gofven" target="_blank"><img class="logos" src="/Flowback.svg" alt="Flowbacks logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Designkonsult och utvecklare, </em></a>
            <a id="date1" class="text3">Januari 2022 - nu</a>
            <p class="text1">Flowback</p>
            <p class="text2">Jag var rådgivare gällande designen som togs fram i Figma och 
                har hjälpt till med utveckling. Projektet är en demokrati-plattform vars källkod är öppen.</p>
        </div>
    </div>

    <div class="flex-container">
        <div class="aside">
            <a href="https://digitaldemokrati.se/" target="_blank"><img class="logos" src="/DD.svg" alt="Föreningens logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Grafisk designkonsult, </em></a>
            <a id="date1" class="text3">Mars 2022</a>
            <p class="text1">Föreningen för Digital demokrati</p>
            <p class="text2">Jag gjorde en presentation efter kundens önskemål och lite annat grafiskt material.</p>
        </div>
    </div>

    <div class="flex-container">
        <div class="aside">
            <a href="https://progressiva-ekonomer.se/" target="_blank"><img class="logos" src="/PE.svg" alt="Progressiva Ekonomers logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Digital Designer, </em></a>
            <a id="date1" class="text3">Juni - Juli 2022</a>
            <p class="text1">Progressiva Ekonomer</p>
            <p class="text2">Jag skapade en logga i olika varianter åt en ideell förening. 
                Loggan var anpassad efter kundens önskemål.</p>
        </div>
    </div>

    <div class="flex-container">
        <div class="aside">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a><img class="logos" src="/Beautyka.svg" alt="Beautykas logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Art Director, </em></a>
            <a id="date2" class="text3">April 2018 - Maj 2022</a>
            <p class="text1">Beautyka</p>
            <p class="text2">Jag ansvarade för content bestående av text, bilder, filmer, och 
                skapade visuellt material med hjälp av Canva.</p>
        </div>
    </div>

    <div class="flex-container">
        <div class="aside">
            <a href="https://www.datana.se/" target="_blank"><img class="logos" src="/Datana.svg" alt="Datans logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Grafisk designkonsult, </em></a>
            <a id="date3" class="text3">Oktober 2021</a>
            <p class="text1">Datana</p>
            <p class="text2">Jag gjorde en PowerPoint efter kundens önskemål. I den använde jag grafiska 3D
                detaljer som jag skapade själv i Affinity Designer.</p>
        </div>
    </div>

    <div class="flex-container">
        <div class="aside">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a><img class="logos" src="/appen-logo.svg" alt="Appens logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Transkriberare, </em></a>
            <a id="date4" class="text3">April 2022 - nu</a>
            <p class="text1">Appen</p>
            <p class="text2">Jobbet gick ut på att transkribera diverse ljudfiler.</p>
        </div>
    </div>
<Button/>
</section>

<Footer/>

<style>
    .erfarenhet {
        color: white;
        background-color: #253439;
        padding: 1rem 0rem 3rem 0rem;
    }

    .title {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.1rem;
        font-size: 1.2rem;
        line-height: 0.1rem;
    }

    .text1 {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.09rem;
        font-size: 1rem;
        padding: 0.5rem 0rem;
    }

    .text2 {
        font-family: 'Open Sans', sans-serif;
        letter-spacing: 0.07rem;
        font-size: 0.8rem;
    }

    .text3 {
        font-family: 'Open Sans', sans-serif;
        letter-spacing: 0.07rem;
        font-size: 0.8rem;
        text-align: right;
        white-space: nowrap;
    }

    .aside {
        width: 3rem;
        height: 3rem;
    }

    .flex-container {
        display: grid;
        grid-template-columns: 3rem auto;
        padding: 1rem;
        column-gap: 1rem;
    }
</style>