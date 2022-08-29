<script>
    import Navbar from "../components/Navbar.svelte"
    import Footer from "../components/Footer.svelte"
    import Button from "../components/Button.svelte"
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
                    
                <!-- svelte-ignore a11y-missing-attribute -->
                <a class="typewrite" data-period="2000" data-type='[ "front-end utvecklare.", "inredare.", "designer." ]'>
                    <span class="wrap"></span>
                </a>
                    
                <script>
                    var TxtType = function(el, toRotate, period) {
                        this.toRotate = toRotate;
                        this.el = el;
                        this.loopNum = 0;
                        this.period = parseInt(period, 10) || 2000;
                        this.txt = '';
                        this.tick();
                        this.isDeleting = false;
                    };

                    TxtType.prototype.tick = function() {
                        var i = this.loopNum % this.toRotate.length;
                        var fullTxt = this.toRotate[i];

                        if (this.isDeleting) {
                        this.txt = fullTxt.substring(0, this.txt.length - 1);
                        } else {
                        this.txt = fullTxt.substring(0, this.txt.length + 1);
                        }

                        this.el.innerHTML = '<span class="wrap">'+this.txt+'</span>';

                        var that = this;
                        var delta = 200 - Math.random() * 100;

                        if (this.isDeleting) { delta /= 2; }

                        if (!this.isDeleting && this.txt === fullTxt) {
                        delta = this.period;
                        this.isDeleting = true;
                        } else if (this.isDeleting && this.txt === '') {
                        this.isDeleting = false;
                        this.loopNum++;
                        delta = 500;
                        }

                        setTimeout(function() {
                        that.tick();
                        }, delta);
                    };

                    window.onload = function() {
                        var elements = document.getElementsByClassName('typewrite');
                        for (var i=0; i<elements.length; i++) {
                            var toRotate = elements[i].getAttribute('data-type');
                            var period = elements[i].getAttribute('data-period');
                            if (toRotate) {
                            new TxtType(elements[i], JSON.parse(toRotate), period);
                            }
                        }
                        // INJECT CSS
                        var css = document.createElement("style");
                        css.type = "text/css";
                        css.innerHTML = ".typewrite > .wrap { border-right: 0.08em solid #fff}";
                        document.body.appendChild(css);
                    };
                </script>

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
    <Button/>
</section>

<Footer/>

<style>
    #home {
        background-color: #253439;
        color: white;
        padding: 2rem 10%;
    }

    .home .home-title {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.09rem;
        font-size: 1.5rem;
        margin: 0.5rem 0rem;
        font-weight: bold;
    }

    .home .home-text {
        font-family: 'Open Sans', sans-serif;
        font-size: 0.8rem;
        letter-spacing: 0.08rem;
        line-height: 1.2rem;
    }

    .home-text p {
        margin: 1rem 0rem;
    }

    .home .home-content .contact-info {
        font-family: 'Open Sans', sans-serif;
        font-size: 0.7rem;
        letter-spacing: 0.08rem;
        line-height: 1.2rem;
    }
    
    .home-photo {
        margin: 1rem 0rem;
    }

    .programming {
        width: 2.5rem;
        height: 2.5rem;
        display: flex;
        flex-direction: row;
        gap: 0.5rem;
        margin: 1.3rem 0rem;
    }

    .typewrite {
        color: white;
        font-family: 'Open Sans', sans-serif;
        font-weight: light;
        font-size: small;
        text-decoration: none;
        position: relative;
    }

    @media only screen and (min-width: 680px) {
        #home {padding: 2rem 10%;}
        .home {display:grid; grid-template-columns: 2fr 1fr; column-gap: 2rem;}
        .home-photo {width: 15rem;}
        .typewrite {font-size: 0.8rem;}
    }
    @media only screen and (min-width: 940px) {
        #home {padding: 3rem 15%;}
        .home {column-gap: 2.3rem;}
        .home .home-title {font-size: 1.5rem;}
        .home .home-text {font-size: 0.9rem;}
        .home-text p {line-height: 1.5rem;}
        .home .home-content .contact-info {font-size: 0.8rem;}
        .home-photo {width: 16rem;}
        .typewrite {font-size: 0.9rem;}
    }
    @media only screen and (min-width: 1200px) {
        #home {padding: 3rem 17%;}
        .home {column-gap: 3rem;}
        .home .home-title {font-size: 1.8rem;}
        .home .home-text {font-size: 1rem;}
        .home-photo {width: 18rem;}
        .home .home-content .contact-info {font-size: 0.9rem;}
        .typewrite {font-size: 1rem;}
    }
    @media only screen and (min-width: 1600px) {
        #home {padding: 4rem 20%;}
        .home .home-title {font-size: 2.5rem;}
        .home .home-text {font-size: 1.4rem; margin: 1rem 0rem;}
        .home-text p {line-height: 2.2rem; margin: 1rem 0rem;}
        .home-photo {width: 21rem;}
        .home .home-content .contact-info {font-size: 1.2rem;  line-height: 2rem;}
        .typewrite {font-size: 1.4rem;}
        .programming {
            width: 3.5rem;
            height: 3.5rem;
            gap: 1rem;
            margin: 1.7rem 0rem;}
    }
</style>