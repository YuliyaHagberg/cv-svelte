<script lang="ts">
    import Navbar from "../components/Navbar.svelte"
    import Footer from "../components/Footer.svelte"
    import Button from "../components/Button.svelte"
</script>

<Navbar/>

<section class="portfolio">
    <div class="container3">        
        <div href="#" class="flex-item" style="background-image: url(/Inredning.svg)"></div>
        <div href="#beautyka" class="flex-item" style="background-image: url(/Beautyka.svg)"></div>
        <div href="#PE" class="flex-item" style="background-image: url(/PE.svg)"></div>
        <div href="#datana" class="flex-item" style="background-image: url(/Datana.svg)"></div>
    </div>
    <h1 class="title">Saker jag har gjort</h1>
    <div class="container4">   
        <img id="portfolio-img-1" src="/Beautyka.png" alt="två kvinnor ler. över dem står texten boka din glykolsyra peeling idag">
        <img id="portfolio-img-2" src="/DERMACEUTIC.png" alt="en kvinna rensar sitt ansikte. flera proukter från ett märke är placerade runt henne.">
        <img id="portfolio-img-3" src="/Facebook.png" alt="produkter och ingredienser på en rosa bakgrund">
        <img id="portfolio-img-4" src="/KemiskPeeling.svg" alt="infografik om olika kemiska peelingar">
        <img id="portfolio-img-5" src="/Instagram.svg" alt="ny video, instagram inlägg">
        <img id="portfolio-img-6" src="/PElogga.svg" alt="Progressiva ekonomer logga">
        <img id="portfolio-img-7" src="/3Dstore.svg" alt="modell av en affär i 3D">
        <img id="portfolio-img-8" src="/3d1.svg" alt="positionsmarkör i 3D">
        <img id="portfolio-img-9" src="/3d2.svg" alt="statiskikstaplar i 3D">
        <img id="portfolio-img-10" src="/3d3.svg" alt="graf i 3D">
        <img id="portfolio-img-11" src="/2d.svg" alt="minisymboler i 2D">
        <!--
            <img id="long-pic" src="/Dermalogica.svg" alt="">
            <img id="long-pic" src="/PElogolong.svg" alt="">
        -->
    </div>
<Button/>
</section>

<Footer/>

<style>
    .portfolio {
        color: white;
        padding-bottom: 5rem;
        padding-top: 1rem;
        background-color: #253439;
    }

    .title {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.1em;
        font-size: 1rem;
        text-align: center;
        padding-top: 1em;
    }

    .container3 {
        display: flex;
        flex-direction: row;
        gap: 0.8rem;
        justify-content: center;
        flex-wrap: wrap;
        padding: 0.5rem;
    }

    .flex-item {
        width: 4rem;
        height: 4rem;
        background-size: cover;
        background-position: center;
        opacity: 70%;
    }

    .flex-item:hover {
        opacity:100%;
    }

    .container4 {
        display: flex;
        flex-direction: row;
        justify-content: center;
        flex-wrap: wrap;
    }

    img {
        width: 8rem;
        height: 8rem;
        margin: 0.5rem;
    }

</style>