<script>
    import Navbar from "../components/Navbar.svelte"
    import Footer from "../components/Footer.svelte"
    import Button from "../components/ToTopButton.svelte"
    import '../components/styles.css'
</script>

<Navbar/>

<div class="filosofi">
    <p class="title">Min filosofi</p>
    <p class="text">Design handlar om att fånga känslor, värderingar, och skönhet på ett sätt som är så praktiskt
         och optimal med avseende på målgruppen som möjligt. Varje arbete jag gör börjar med en 
         målgruppsanalys, vad associerar de olika symboler till? Hur blir designen tillgänlig och 
         vacker för dem? Det ska finnas ett naturligt flöde så att målgruppen enkelt dansar sig fram
          till målet.</p>

    <p class="middle"><em>Människor förstår saker och ting i narrativ, vilket blir något att undersöka 
        från fall till fall. Hur kan designen berätta rätt berättelse?</em></p>

    <p class="text">Bra design går ut på att svara på diverse frågor, bland annat: vilken funktion spelar designens
         element? Vilken struktur har de mellan sig? Vilken stil har de? Vad innebär de för målgruppen?
          Vilken process är den bästa för att skapa designen? Detta svarar jag på tillsammans med 
          kunden till den grad som kunden önskar. Jag skapar själv alltid prototyper först för att
           testa idéerna, och itererar nya inom de rätta begränsningarna.</p>

    <p class="text">Det finns många metoder jag använder mig av: att tänka baklänges från målet till början, 
        att tänka mig vad som inte skulle passa för att visualisera motsatsen, att ta in någon 
        annans perspektiv givet att arbetet inte är sekretessbelagt, att undersöka vetenskapliga artiklar 
        om fonters psykologiska effekter, att undersöka själv gentemot målgruppen, med mera.</p>

    <p class="text">Jag arbetar med text, bilder, inredning, och interaktivitet, samt att få dessa konstformer 
        att vara i harmoni.</p>

    <p class="title2">Rationalitet</p>
    <p class="text">Smarta och innovativa lösningar är de bästa vägarna fram för elegans. Det är viktigt att 
        experimentera med hypoteser och kunna vara måttligt själv-kritisk, flexibel och ödmjuk. 
        Detta innebär också att brister ska hanteras så bra som det går. Vetenskapliga belägg är 
        viktiga som grund.</p>

    <p class="title2">Samvetsgrannhet och produktivitet</p>
    <p class="text">Jag bryter ner planer i mindre delar, och utvärderar kontinuerligt hur arbetet går 
        och hur det kan förbättras. Jag använder mig av <em>Get Things Done</em>, antecknar smart, och visar upp 
        de möjliga bra alternativ som jag kommer fram till om du som kund önskar att samskapa designen.</p>

    <p class="title2">Mål- och teamfokus</p>
    <p class="text">Jag fokuserar på att få fram bästa möjliga resultat. Att samskapa efter en gemensam 
        vision med dig och ditt projekt genom att lära känna din verksamhet till den grad du önskar. 
        Tillsammans så skapar vi en röd tråd som leder oss ut ur labyrinten av otydlighet och 
        abstraktion, till professionella konkreta designer och sidor.</p>

    <p class="title2">Fortsättningsvis</p>
    <p class="text">Jag gör alltid mitt bästa, älskar livet, och är rolig ibland! Det som är tråkigt 
        kan oftast bli roligt genom att byta perspektiv! Några intressen jag har förutom design och 
        utveckling är att spela sällskasspel, att resa, och att äta glass. Min vision är att skapa en 
        vackrare, mer tillgänglig och funktionell värld - tillsammans skapar vi just den framtiden!</p>
</div>

<Button/>

<style>
    .filosofi {
        color: white;
        justify-content: left;
        background-color: #253439;
        padding: 1.5rem;
    }

    .filosofi .title {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.09rem;
        font-size: 1.2rem;
    }

    .filosofi .title2 {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.09rem;
        font-size: 1rem;
        padding: 1rem 0rem 0rem 0rem;
    }

    .filosofi .text {
        font-family: 'Open Sans', sans-serif;
        letter-spacing: 0.09rem;
        font-size: 0.7rem;
        text-align: left;
    }

    .filosofi .middle {
        font-family: 'Coco-Gothic', bold;
        font-weight: bolder;
        letter-spacing: 0.09rem;
        font-size: 0.8rem;
        text-align: center;
        padding: 1rem 10%;
    }
    @media only screen and (min-width: 640px) {
        .filosofi {padding: 2.5rem 20% 3rem 10%;}
        .filosofi .title {font-size: 1.3rem;}
        .filosofi .title2 {
            font-size: 1rem;
            padding: 1.1rem 0rem 0rem 0rem;}
        .filosofi .text {font-size: 0.7rem;}
        .filosofi .middle {font-size: 0.8rem; padding: 1.5rem 15%;}
    }
    @media only screen and (min-width: 940px) {
        .filosofi {padding: 2rem 25% 3rem 13%;}
        .filosofi .title {font-size: 1.5rem;}
        .filosofi .title2 {
            font-size: 1.3rem;
            padding: 1.2rem 0rem 0rem 0rem;}
        .filosofi .text {font-size: 0.8rem;}
        .filosofi .middle {font-size: 0.9rem; padding: 1.7rem 15%;}
    }
    @media only screen and (min-width: 1200px) {
        .filosofi {padding: 3rem 30% 3rem 15%;}
        .filosofi .title {font-size: 1.7rem;}
        .filosofi .title2 {
            font-size: 1.5rem;
            padding: 1.4rem 0rem 0.3rem 0rem;}
        .filosofi .text {font-size: 1rem;}
        .filosofi .middle {font-size: 1.1rem; padding: 1.7rem 15%;}
    }
    @media only screen and (min-width: 1600px) {
        .filosofi {padding: 4rem 35% 6rem 18%;}
        .filosofi .title {font-size: 2rem;}
        .filosofi .title2 {
            font-size: 1.8rem;
            padding: 1.8rem 0rem 0.3rem 0rem;}
        .filosofi .text {font-size: 1.2rem;}
        .filosofi .middle {font-size: 1.3rem; padding: 1.7rem 15%;}
    }
</style>

<Footer/>