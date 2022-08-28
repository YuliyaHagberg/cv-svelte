<script lang="ts">
    import Navbar from "../components/Navbar.svelte"
    import Footer from "../components/Footer.svelte"
    import Button from "../components/Button.svelte"

    let show = false;
    let source:string;
    const imageClick = (src:string) => {
        source = src;
        show = !show;
    }
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
        <img id="portfolio-img" on:click={()=>imageClick("/Beautyka.png")} src="/Beautyka.png" alt="två kvinnor ler. över dem står texten boka din glykolsyra peeling idag">
        <img id="portfolio-img" on:click={()=>imageClick("/DERMACEUTIC.png")} src="/DERMACEUTIC.png" alt="en kvinna rensar sitt ansikte. flera proukter från ett märke är placerade runt henne.">
        <img id="portfolio-img" on:click={()=>imageClick("/Facebook.png")} src="/Facebook.png" alt="produkter och ingredienser på en rosa bakgrund">
        <img id="portfolio-img" on:click={()=>imageClick("/KemiskPeeling.svg")} src="/KemiskPeeling.svg" alt="infografik om olika kemiska peelingar">
        <img id="portfolio-img" on:click={()=>imageClick("/Instagram.svg")} src="/Instagram.svg" alt="ny video, instagram inlägg">
        <img id="portfolio-img" on:click={()=>imageClick("/PElogga.svg")} src="/PElogga.svg" alt="Progressiva ekonomer logga">
        <img id="portfolio-img" on:click={()=>imageClick("/3Dstore.svg")} src="/3Dstore.svg" alt="modell av en affär i 3D">
        <img id="portfolio-img" on:click={()=>imageClick("/3d1.svg")} src="/3d1.svg" alt="positionsmarkör i 3D">
        <img id="portfolio-img" on:click={()=>imageClick("/3d2.svg")} src="/3d2.svg" alt="statiskikstaplar i 3D">
        <img id="portfolio-img" on:click={()=>imageClick("/3d3.svg")} src="/3d3.svg" alt="graf i 3D">
        <img id="portfolio-img" on:click={()=>imageClick("/2d.svg")} src="/2d.svg" alt="minisymboler i 2D">
        <!--<img id="long-pic" src="/Dermalogica.svg" alt="">
            <img id="long-pic" src="/PElogolong.svg" alt="">-->
    </div>
    <div class="modul" class:invisible={!show}>
        <div class="absolute top-0 right-0 m-4 p-1 rounded-full" on:click={() => show = !show}><i class="fa-solid fa-xmark"></i></div>
        <img id="portfolio-img" src={source} alt="">
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
        cursor: pointer;
    }

    img:hover {
        filter:brightness(0.8);
    }

    .modul {
        position: fixed;
        top: calc(50% - 25rem / 2);
        left: calc(50% - 25rem / 2);
        z-index: 999999;
    }

    .modul div {
        background-color: #B29E84;
    }

    .modul div:hover {
        background-color: #253439;
        transition: 1s;
    }

    .modul img {
        z-index: 999999;
        width: 25rem;
        height: 25rem;
    }
</style>
