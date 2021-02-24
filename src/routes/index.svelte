<script>
	import logo from '../assets/prolebox.jpg';
</script>

<style>
	h1, figure, p {
		text-align: center;
		margin: 0 auto;
	}

	h1 {
		font-size: 2.8em;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0 0 0.5em 0;
	}

	figure {
		margin: 0 0 1em 0;
	}

	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}

	p {
		margin: 1em auto;
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
		}
		button {
			margin-left: 41%;
		}
	}

	@media (min-width: 320px) {
		button {
			margin-left: 15%;
		}
	}

	button {
		padding: 7px 45px;
		font-size: small;
		border-radius: 15px;
		color: blanchedalmond;
		background-color: rgb(27, 22, 92);
	}
</style>

<svelte:head>
	<title>Hype Test</title>
</svelte:head>

<h1>Hype Test</h1>

<figure>
	<img alt="Success Kid" src="{logo}">
	<figcaption>Are you a sneakerhead? Lets put that to the test!</figcaption>
</figure>

<p><strong>Lets put that to the test!</strong></p>
<a aria-current="page" href="calculator" ><button>Begin</button></a>
