<script lang="ts">
	import { onMount } from 'svelte';

	let scrolled: boolean = false;

	onMount(() => {
		window.onscroll = () => {
			scrollFunction();
		};
	});

	// When the user scrolls down 20px from the top of the document, show the button

	function scrollFunction() {
        const scroll = window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop
		if (scroll > 20) {
			scrolled = true;
		} else {
			scrolled = false;
		}
	}

	// When the user clicks on the button, scroll to the top of the document
	function topFunction() {
		document.body.scrollTop = 0; // For Safari
		document.documentElement.scrollTop = 0; // For Chrome, Firefox, IE and Opera
	}
</script>

<button
	on:click={() => topFunction()}
	class:invisible={!scrolled}
	id="myBtn"
	title="Go to top"
	class="fas fa-angle-up"
    ></button>

<style>
	#myBtn {
		position: fixed;
		bottom: 1rem;
		right: 1rem;
		z-index: 99;
		border: none;
		outline: none;
		background-color: #b29e84;
		color: white;
		cursor: pointer;
		padding: 0.8rem;
		border-radius: 0.5rem;
		font-size: 0.8rem;
	}
	#myBtn:hover {
		background-color: #555;
	}

	@media only screen and (min-width: 640px) {
		#myBtn {
			bottom: 2rem;
			right: 2rem;
		}
	}
	@media only screen and (min-width: 940px) {
		#myBtn {
			bottom: 2.3rem;
			right: 2.3rem;
			font-size: 0.9rem;
		}
	}
	@media only screen and (min-width: 1200px) {
		#myBtn {
			bottom: 2.5rem;
			right: 2.5rem;
			padding: 0.9rem;
			font-size: 0.9rem;
		}
	}
	@media only screen and (min-width: 1600px) {
		#myBtn {
			bottom: 3.1rem;
			right: 3.1rem;
			padding: 1rem;
			font-size: 1.8rem;
		}
	}
</style>
