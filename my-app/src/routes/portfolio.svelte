<script lang="ts">
	import Navbar from '../components/Navbar.svelte';
	import Footer from '../components/Footer.svelte';
	import Button from '../components/ToTopButton.svelte';

	let show = false;
	let source: string;
	const imageClick = (src: string) => {
		source = src;
		show = !show;
	};
</script>

<Navbar />

<section class="portfolio">
	<div class="container3">
		<div href="#" class="flex-item" style="background-image: url(/Inredning.svg)" />
		<div href="#beautyka" class="flex-item" style="background-image: url(/Beautyka.svg)" />
		<div href="#PE" class="flex-item" style="background-image: url(/PE.svg)" />
		<div href="#datana" class="flex-item" style="background-image: url(/Datana.svg)" />
	</div>
	<h1 class="title">Saker jag har gjort</h1>
	<div class="container4">
		<img
			id="portfolio-img"
			on:click={() => imageClick('/Beautyka.png')}
			src="/Beautyka.png"
			alt="två kvinnor ler. över dem står texten boka din glykolsyra peeling idag"
		/>
		<img
			id="portfolio-img"
			on:click={() => imageClick('/DERMACEUTIC.png')}
			src="/DERMACEUTIC.png"
			alt="en kvinna rensar sitt ansikte. flera proukter från ett märke är placerade runt henne."
		/>
		<img
			id="portfolio-img"
			on:click={() => imageClick('/Facebook.png')}
			src="/Facebook.png"
			alt="produkter och ingredienser på en rosa bakgrund"
		/>
		<img
			id="portfolio-img"
			on:click={() => imageClick('/KemiskPeeling.svg')}
			src="/KemiskPeeling.svg"
			alt="infografik om olika kemiska peelingar"
		/>
		<img
			id="portfolio-img"
			on:click={() => imageClick('/Instagram.svg')}
			src="/Instagram.svg"
			alt="ny video, instagram inlägg"
		/>
		<img
			id="portfolio-img"
			on:click={() => imageClick('/PElogga.svg')}
			src="/PElogga.svg"
			alt="Progressiva ekonomer logga"
		/>
		<img
			id="portfolio-img"
			on:click={() => imageClick('/3Dstore.svg')}
			src="/3Dstore.svg"
			alt="modell av en affär i 3D"
		/>
		<img
			id="portfolio-img"
			on:click={() => imageClick('/3d1.svg')}
			src="/3d1.svg"
			alt="positionsmarkör i 3D"
		/>
		<img
			id="portfolio-img"
			on:click={() => imageClick('/3d2.svg')}
			src="/3d2.svg"
			alt="statiskikstaplar i 3D"
		/>
		<img
			id="portfolio-img"
			on:click={() => imageClick('/3d3.svg')}
			src="/3d3.svg"
			alt="graf i 3D"
		/>
		<img
			id="portfolio-img"
			on:click={() => imageClick('/2d.svg')}
			src="/2d.svg"
			alt="minisymboler i 2D"
		/>
		<!--<img id="long-pic" src="/Dermalogica.svg" alt="">
            <img id="long-pic" src="/PElogolong.svg" alt="">-->
	</div>
	<div class="modul" class:invisible={!show}>
		<div class="absolute top-0 right-0 rounded-full" on:click={() => (show = !show)}>
			<i class="fa-solid fa-circle-xmark" />
		</div>
		<img id="portfolio-img" src={source} alt="" />
	</div>
	<Button />
</section>

<Footer />

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
		font-size: 0.9rem;
		text-align: center;
		padding-top: 1em;
	}
	.container3 {
		display: flex;
		flex-direction: row;
		gap: 0.5rem;
		justify-content: center;
		flex-wrap: wrap;
		padding: 0.5rem;
	}
	.flex-item {
		width: 3rem;
		height: 3rem;
		background-size: cover;
		background-position: center;
		opacity: 70%;
	}
	.flex-item:hover {
		opacity: 100%;
	}
	.container4 {
		display: flex;
		flex-direction: row;
		justify-content: center;
		flex-wrap: wrap;
	}
	img {
		width: 6rem;
		height: 6rem;
		margin: 0.5rem;
		cursor: pointer;
	}
	.container4 img:hover {
		filter: brightness(0.8);
	}
	.modul {
		position: fixed;
		top: calc(50% - 21rem / 2);
		left: calc(50% - 21rem / 2);
		z-index: 999999;
		padding: 1.5rem;
	}
	.modul div {
		color: #253439;
		font-size: 1.5rem;
		cursor: pointer;
	}
	.modul i {
		padding: 0.1rem;
		background-color: white;
		border-radius: 50%;
	}
	.modul img {
		z-index: 999999;
		width: 18rem;
		height: 18rem;
	}

	@media (min-width: 640px) {
		.portfolio {
			padding-top: 2rem;
		}
		.title {
			font-size: 1rem;
		}
		.flex-item {
			width: 3.5rem;
			height: 3.5rem;
		}
		img {
			width: 9rem;
			height: 9rem;
		}
		.modul {
			position: fixed;
			top: calc(50% - 23rem / 2);
			left: calc(50% - 23rem / 2);
		}
		.modul div {
			color: #253439;
		}
		.modul img {
			width: 20rem;
			height: 20rem;
		}
	}
	@media (min-width: 940px) {
		.portfolio {
			padding-top: 2.2rem;
		}
		.title {
			font-size: 1.1rem;
		}
		.flex-item {
			width: 4.5rem;
			height: 4.5rem;
		}
		img {
			width: 11rem;
			height: 11rem;
		}
		.modul {
			position: fixed;
			top: calc(50% - 28rem / 2);
			left: calc(50% - 28rem / 2);
		}
		.modul img {
			width: 25rem;
			height: 25rem;
		}
	}
	@media (min-width: 1200px) {
		.portfolio {
			padding-top: 2.4rem;
		}
		.title {
			font-size: 1.2rem;
			margin-bottom: 1rem;
		}
		.flex-item {
			width: 6.5rem;
			height: 6.5rem;
		}
		img {
			width: 15rem;
			height: 15rem;
		}
		.modul {
			position: fixed;
			top: calc(50% - 34rem / 2);
			left: calc(50% - 34rem / 2);
		}
		.modul img {
			width: 31rem;
			height: 31rem;
		}
		.modul div {
			font-size: 1.7rem;
		}
	}
	@media (min-width: 1600px) {
		.portfolio {
			padding-top: 2.7rem;
		}
		.title {
			font-size: 1.7rem;
			margin-bottom: 1.2rem;
		}
		.flex-item {
			width: 8.5rem;
			height: 8.5rem;
		}
		img {
			width: 20rem;
			height: 20rem;
		}
		.modul {
			position: fixed;
			top: calc(50% - 56rem / 2);
			left: calc(50% - 56rem / 2);
			padding: 3rem;
		}
		.modul img {
			width: 50rem;
			height: 50rem;
		}
		.modul div {
			font-size: 2rem;
		}
	}
</style>
