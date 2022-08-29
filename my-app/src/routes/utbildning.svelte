<script>
    import Navbar from "../components/Navbar.svelte"
    import Footer from "../components/Footer.svelte"
    import Button from "../components/Button.svelte"
</script>

<Navbar/>

<section class="utbildning">
    <div class="flex-container">
        <div class="aside">
            <a href="https://www.ltu.se/" target="_blank"><img class="logos" src="/LTU.svg" alt="LTUs logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Digital tjänsteutveckling, </em></a>
            <a id="date1" class="text3">Augusti 2022 - Juni 2025</a>
            <p class="text1">Luleå tekniska universitet</p>
            <p class="text2">Digital tjänste<wbr/>utveckling är ett växande och innovativt område. Digitala tjänste<wbr/>utvecklare jobbar med design av allt från idé och prototyp till 
                färdig tjänst som ofta är webbaserad. Under utbildningen får man lära sig om interaktions<wbr/>design, UX och webb<wbr/>utveckling centralt. Här lär man sig även digitala 
                strategier och affärs<wbr/>modeller, samt hur IKT påverkas av individ, organisation och samhälle.</p>
        </div>
    </div>

    <div class="flex-container">
        <div class="aside">
            <a href="https://www.codecademy.com/" target="_blank"><img class="logos" src="/Code.svg" alt="Codecademys logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Front-end Engineer, </em></a>
            <a id="date1" class="text3">December 2021 - Augusti 2022</a>
            <p class="text1">Codecademy</p>
            <p class="text2">På Codecademy har jag lärt mig programmeringens principer, HTML, CSS, Javascript, Node.js, API-hantering, säkerhet, att arbeta med github, med mera. 
                Codecademy har även inspirerat mig att läsa vidare själv när det gäller mer avancerade saker och om nyare industri<wbr/>standarder så som Svelte och Typescript.
            </p>
        </div>
    </div>

    <div class="flex-container">
        <div class="aside">
            <a href="https://www.kth.se/" target="_blank"><img class="logos" src="/KTH.svg" alt="KTHs logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Civilingenjör i samhälls<wbr/>byggnad, </em></a>
            <a id="date1" class="text3">Augusti 2021 - Juni 2022</a>
            <p class="text1">Kungliga Tekniska högskolan</p>
            <p class="text2">Här lärde jag mig om samhälls<wbr/>byggnads<wbr/>processen, numeriska metoder, programmering i matlab, linjär algebra och analys.
                Jag bytte program efter ett år för att jag är mer intresserad av datateknik och design.
            </p>
        </div>
    </div>

    <div class="flex-container">
        <div class="aside">
            <a href="https://www.inredningskurser.se/" target="_blank"><img class="logos" src="/Inredning.svg" alt="Inredningskursernas logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Inredare, Homestaging<wbr/>konsult & Inrednings<wbr/>stylist, </em></a>
            <a id="date2" class="text3">Oktober 2021 - nu</a>
            <p class="text1">Inredningskurser Sverige</p>
            <p class="text2">I denna yrkes<wbr/>utbildning har jag fått kompetenser från färgsättning, ljussättning, 
                möblering, och kunskaper i hur man praktiskt arbetar som inredare & hur man skapar sin egen verksamhet. 
                Vi har bland annat arbetat med fiktiva kunder, kollage, moodboards, färgsättningar, kundanalys.</p>
        </div>
    </div>

    <div class="flex-container">
        <div class="aside">
            <a href="https://kungsholmensgymnasium.stockholm/" target="_blank"><img class="logos" src="/KG.svg" alt="Gymnasiets logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Naturvetenskaps<wbr/>programmet, </em></a>
            <a id="date3" class="text3">Augusti 2018 - Juni 2021</a>
            <p class="text1">Kungsholmens gymnasium</p>
            <p class="text2">Här utvecklade jag ett vetenskapligt förhållnings<wbr/>sätt 
                och lärde mig att se olika fenomen i ett helhets<wbr/>perspektiv samt hur man arbetar bra i ett team.</p>
        </div>
    </div>

    <div class="flex-container">
        <div class="aside">
            <a href="https://www.dalecarnegie.se/" target="_blank"><img class="logos" src="/Dale.svg" alt="Dale Carnegies logotyp"></a>
        </div>
        <div class="main">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a class="title"><em>Generation.Next, </em></a>
            <a id="date4" class="text3">November 2018 - Maj 2019</a>
            <p class="text1">Dale Carnegie</p>
            <p class="text2">Generation.Next är ledarskaps<wbr/>träningen för unga vuxna som vill lära sig 
                färdigheter som varar livet ut. I denna kurs får man kunskaper och tränar sig på teamwork, 
                ledarskap, social förmåga, kommunikation, attityd samt hantera stress och oro. Man får 
                konkreta verktyg för hur man hanterar prestations<wbr/>ångest och stress, förbereder och håller 
                presentationer och tal, sätter rimliga och nåbara målsättningar, säljer in dina åsikter, 
                samt viktigast av allt, hur man skapar, behåller och förbättrar relationer med vänner, 
                lärare, familj och arbetsgivare.</p>
        </div>
    </div>
<Button/>
</section>

<Footer/>

<style>
    .utbildning {
        color: white;
        background-color: #253439;
        padding: 1rem 0rem 3rem 0rem;
    }

    .title {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.1rem;
        font-size: 1rem;
        line-height: 0.1rem;
    }

    .text1 {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.09rem;
        font-size: 0.8rem;
        padding: 0.6rem 0rem;
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
        width: 2.7rem;
        height: 2.7rem;
    }

    .flex-container {
        display: grid;
        grid-template-columns: 12.5% auto;
        padding: 1rem;
        column-gap: 1rem;
    }

    @media only screen and (min-width: 640px) {
        .utbildning {padding: 1.5rem 15% 3rem 10%;}
        .title {font-size: 1.2rem;}
        .text1 {
            font-size: 1rem;
            padding: 0.5rem 0rem;}
        .text2 {font-size: 0.9rem;}
        .text3 {font-size: 0.9rem;}
        .aside {
            width: 4rem;
            height: 4rem;}
    }
    @media only screen and (min-width: 940px) {
        .utbildning {padding: 2rem 18% 3rem 10%;}
        .title {font-size: 1.3rem;}
        .text1 {font-size: 1rem;}
        .text2 {font-size: 1rem;}
        .text3 {font-size: 1rem;}
        .aside {
            width: 5rem;
            height: 5rem;}
    }
    @media only screen and (min-width: 1200px) {
        .utbildning {padding: 3rem 20% 4rem 13%;}
        .title {font-size: 1.5rem;}
        .text1 {font-size: 1.1rem;}
        .text2 {font-size: 1.1rem;}
        .text3 {font-size: 1.1rem;}
        .aside {
            width: 6rem;
            height: 6rem;}
    }
    @media only screen and (min-width: 1600px) {
        .utbildning {padding: 3rem 23% 4rem 15%;}
        .flex-container {padding: 2rem 0rem;}
        .title {font-size: 1.7rem;}
        .text1 {font-size: 1.4rem;}
        .text2 {font-size: 1.4rem;}
        .text3 {font-size: 1.4rem;}
        .aside {
            width: 7rem;
            height: 7rem;}
    }
</style>