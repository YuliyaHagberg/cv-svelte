<button on:click={() => topFunction()} id="myBtn" title="Go to top" class="fas fa-angle-up"></button>

<script lang="ts">
import { onMount } from "svelte";

    let mybutton:any;

    onMount(() => {
        mybutton = document.getElementById("myBtn");
        window.onscroll = function() {scrollFunction()};
    })

    // When the user scrolls down 20px from the top of the document, show the button

    function scrollFunction() {
        if (typeof mybutton !== null)
        if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
            mybutton.style.display = "block";
        } else {
            mybutton.style.display = "none";
        }
    }

    // When the user clicks on the button, scroll to the top of the document
    function topFunction() {
        document.body.scrollTop = 0; // For Safari
        document.documentElement.scrollTop = 0; // For Chrome, Firefox, IE and Opera
    }
</script>

<style>
    #myBtn {
        display: none;
        position: fixed;
        bottom: 1rem;
        right: 1rem;
        z-index: 99;
        border: none;
        outline: none;
        background-color: #B29E84;
        color: white;
        cursor: pointer;
        padding: 0.8rem;
        border-radius: 0.5rem;
        font-size: 0.8rem;
    }
    
    #myBtn:hover {
        background-color: #555;
    }
</style>