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
        font-size: 0.8em;}
    .contact {margin: 0rem 1rem;}
    .contact .text {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.1em;
        font-size: 1.1rem;
        margin: 2rem 1rem 1rem 1rem;
        text-align: center;}
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
        padding-left: 0.5rem;}
    input:focus {
        border-bottom:#253439 0.25rem solid;
        outline:none;
        transition: 1s;}
    textarea:focus {
        border-bottom:#253439 0.25rem solid;
        outline:none;}

    .field textarea {
        resize:vertical;
        height: 5rem;
        min-height: 3rem;}
    .container1 .button {
        border: none;
        background-color:#101F24;
        color: white;
        cursor: pointer;
        padding: 0.5rem 1.8rem;
        text-align: center;
        border-radius: 0.5rem;
        font-size: 0.8rem;
        font-family: 'Open Sans', sans-serif;}
    .container1 .button:hover {
        background-color:#B29E84;
        color:#101F24;}
    .info {margin: 2rem 0rem;}
    .container2 {
        display:grid;
        grid-template-columns: 1.5rem auto 1fr;
        align-items:center;
        margin: 1rem 0rem;}
    .container2 .icon {
        color:#101F24;
        font-size: 1rem;
        align-self: center;}
    .contact .undertitle {
        font-family: 'Coco-Gothic';
        letter-spacing: 0.1rem;
        font-size: 0.8rem;
        text-align: left;
        margin-left: 0.3rem;
        font-weight: bold;}
    .contact .undertext {
        font-family: 'Open Sans', sans-serif;
        letter-spacing: 0.1rem;
        font-size: 0.8rem;
        font-weight: lighter;
        text-align: left;
        margin-left: 0.3rem;
    }

    @media only screen and (min-width: 640px) {
        h4, input, textarea {font-size: 0.9em;}
        .text {font-size: 1em;}
        .contact {margin: 0rem 10% 2rem 10%;}
        .container {margin:0rem;}
        .container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            column-gap: 1.5rem;}
        .container1 .button {
            padding: 0.5rem 1.9rem;
            font-size: 0.9rem;}
        .info {margin: 0rem;}
        .container2 {
            display:grid;
            grid-template-columns: 1.5rem auto 1fr;}
        .container2 .icon {font-size: 1rem;}
        .contact .undertitle {
            font-size: 0.8rem;
            margin-left: 0.3rem;
            margin-top: 0.1rem;}
        .contact .undertext {
            font-size: 0.8rem;
            margin-left: 0.3rem;}
        }
    
    @media only screen and (min-width: 940px) {
        h4, input, textarea {font-size: 1em;}
        .contact .text {font-size: 1.2em;}
        .contact {margin: 0rem 14% 2rem 14%;}
        .container {column-gap: 2rem;}
        .container1 .button {
            padding: 0.5rem 1.9rem;
            font-size: 1rem;}
        .container2 .icon {font-size: 1.1rem;}
        .contact .undertitle {font-size: 0.9rem;}
        .contact .undertext {font-size: 0.9rem;}
        }
    @media only screen and (min-width: 1200px) {
        h4, input, textarea {font-size: 1.1em;}
        .contact .text {font-size: 1.3em;
            margin: 2rem 1rem;}
        .contact {margin: 0rem 17% 2rem 17%;}
        .field input, .field textarea {margin-bottom: 0.7rem;}
        .container {column-gap: 3rem;}
        .container1 .button {
            padding: 0.6rem 2rem;
            font-size: 1.2rem;}
        .container2 .icon {font-size: 1.2rem;}
        .contact .undertitle {font-size: 1rem;
            margin-left: 0.7rem;}
        .contact .undertext {font-size: 1rem;}
        }
    @media only screen and (min-width: 1600px) {
        h4, input, textarea {font-size: 1.2em;}
        .field input, .field textarea {height: 3rem;}
        .field textarea {
            height: 6rem;
            min-height: 6rem;}
        .contact .text {font-size: 1.6em;
            margin: 3rem 1rem;}
        .contact {margin: 0rem 20% 2rem 20%;}
        .field input, .field textarea {margin-bottom: 0.9rem;}
        .container {column-gap: 4rem;}
        .container1 .button {
            padding: 1rem 2.3rem;
            font-size: 1.4rem;}
        .container2 .icon {font-size: 1.4rem;}
        .contact .undertitle {font-size: 1.3rem;
            margin-left: 1rem;
            margin-top: 0.3rem;}
        .contact .undertext {font-size: 1.3rem;
            margin-left: 0.7rem;}
        }
</style>