<script>
    import Navbar from "../components/Navbar.svelte"
    import Footer from "../components/Footer.svelte"
</script>

<Navbar/>

<section id="home">
    <div class="home">
        <div class="home-content">
            <div class="home-title">
                <h1>Välkommen!</h1>
            </div>
            <div class="home-text">
                <p>Hej och välkommen till min webbsida! Jag heter Yuliya och jag är en
                    
                    <!-- <a class="typewrite" data-period="2000" data-type='[ "front-end utvecklare.", "inredare.", "designer." ]'>
                        <span class="wrap"></span>
                    </a> -->

                <p>Här kan du hitta information om mina kompetenser och erfarenheter, 
                    samt kolla min portfolio och läsa lite om mig själv.</p>
                <p>Hör gärna av dig om du har några frågor eller funderingar!</p>
            </div>
            <div class="programming">
                <img src="/HTML.png" alt="HTML5 logotyp"/>
                <img src="/CSS.png" alt="CSS3 logotyp"/>
                <img src="/Svelte.png" alt="Svelte logotyp"/>
                <img src="/JS.png" alt="Javascript logotyp"/>
                <img src="/Typescript.png" alt="Typescript logotyp"/>
            </div>                
            <div class="contact-info">
                <p>Email: yuliya.swe@gmail.com</p>
                <p>Mobilnummer: +46 728 790 804</p>
            </div>
        </div>
        <div class="home-photo">
            <img src="/Yuliyaphoto.svg" alt="En bild på Yuliya.">
        </div>
    </div>
</section>

<style>
    .programming {
        width: 2.5em;
        display: flex;
        flex-direction: row;
    }
</style>

<Footer/>