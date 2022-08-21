<section class="contact" id="contact">
    <div class="text">Kontakta mig</div>
    <div class="container">
        <div class="container1">
            <form action="https://formsubmit.co/b45e24c1740d2090c4e0bb243859eb84" method="POST">
                <div class="fields">
                    <div class="field name">
                        <input type="text" name="Name" placeholder="Namn" required>
                    </div>
                    <div class="field email">
                        <input type="email" name="Email" placeholder="Email" required>
                    </div>
                    <div class="field textarea">
                        <textarea type="text" name="Message" placeholder="Meddelande..." required></textarea>
                    </div>
                        <input type="submit" value="Skicka" class="button">
                </div>
            </form>
        </div>

        <div class="info">
            <div class="container2">
                <i class="fa-solid fa-user icon"></i>
                <h3 class="undertitle">Namn:</h3>
                <h4 class="undertext">Yuliya Hagberg</h4>
            </div>
            <div class="container2">
                <i class="fa-solid fa-location-dot icon"></i>
                <h3 class="undertitle">Plats:</h3>
                <h4 class="undertext">Stockholm, Sverige</h4>
            </div>
            <div class="container2">
                <i class="fa-solid fa-phone icon"></i>
                <h3 class="undertitle">Mobilnummer:</h3>
                <h4 class="undertext">+46 728 790 804</h4>
            </div>
            <div class="container2">
                <i class="fa-solid fa-envelope icon"></i>
                <h3 class="undertitle">Email:</h3>
                <h4 class="undertext">yuliya.swe@gmail.com</h4>
            </div>
        </div>
    </div>
</section>

<style>
    h4, input, textarea {
        font-family: 'Open Sans', sans-serif;
        font-size: 1em;
    }
    
    h3 {
        font-family: 'Coco-Gothic', light;
        font-size: 1em;
        font-weight: bold;
    }

    .text {
        font-family: 'Coco-Gothic', light;
        font-size: 1.5em;
    }

    .contact {
        margin-left: 1rem;
        margin-right: 1rem;
    }

    .contact .text {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.1em;
        font-size: x-large;
        margin: 2rem 1rem 1rem 1rem;
        text-align: center;
    }

    .field input, .field textarea {
        height: 2.5rem;
        width:100%;
        background-color:#f6f3ef;
        border-bottom:#B29E84 0.25rem solid;
        border-top:none;
        border-left:none;
        border-right:none;
        cursor: pointer;
        margin-bottom: 0.5rem;
        padding-left: 0.5rem;
    }

    input:focus {
        border-bottom:#253439 0.25rem solid;
        outline:none;
    }

    textarea:focus {
        border-bottom:#253439 0.25rem solid;
        outline:none;
    }

    .field textarea {
        resize:vertical;
        height: 5rem;
        min-height: 3rem;
    }

    .container1 .button {
        border: none;
        background-color:#101F24;
        color: white;
        cursor: pointer;
        padding: 0.6rem 2rem;
        text-align: center;
        border-radius: 0.5rem;
        font-size: 1rem;
        font-family: 'Open Sans', sans-serif;
    }

    .container1 .button:hover {
        background-color:#B29E84;
        color:#101F24;
    }

    .info {
        margin: 2rem 0rem;
    }

    .container2 {
        display:grid;
        grid-template-columns: 1.5rem auto 1fr;
        align-items:center;
        margin: 1rem 0rem;
    }

    .container2 .icon {
        color:#101F24;
        font-size: 1.2rem;
        align-self: center;
    }

    .contact .undertitle {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.1rem;
        font-size: 1rem;
        text-align: left;
        margin-left: 0.3rem;
    }

    .contact .undertext {
        font-family: 'Open Sans', sans-serif;
        letter-spacing: 0.1rem;
        font-size: 1rem;
        font-weight: lighter;
        text-align: left;
        margin-left: 0.3rem;
    }

</style>