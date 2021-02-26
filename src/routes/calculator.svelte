<script>
    import Box from "../components/Box.svelte";
    const SneaksAPI = require('sneaks-api');
    const sneaks = new SneaksAPI();

    let shoe1, shoe2, shoe3 = '';

    function handlesubmit() {
        console.log(
            sneaks.getMostPopular(function(err, products){
                console.log(products)
            })
        )
    }
</script>

<style>
    h3, p {
        text-align: center;
        margin: 0 auto;
    }

    h3 {
		font-size: 2.3em;
		text-transform: uppercase;
		font-weight: 300;
        margin-bottom: 1.5em;
	}

    input {
        border-radius: 10px;
        border-style: hidden;
        margin: auto;
        align-content: center;
    }

    button {
        margin: auto;
        border: none;
        padding: 5px 15px;
        color: bisque;
        display: block;
        margin-top: 1em;
        border-radius: 10px;
        font-size: 1em;
        background-color: rgba(34, 10, 122, 0.719);
        font-weight: 300;
    }
</style>

<svelte:head>
	<title>Calculator</title>
</svelte:head>

<h3>Input your 3 favorite sneaks</h3>

<Box>
    <p>No. 1</p>
    <input type="text" placeholder="Dusty Jordan 1" bind:value={shoe1} >
    <p>No. 2</p>
    <input type="text" placeholder="Nike Dunk Low Pine Green" bind:value={shoe2} >
    <p>No. 3</p>
    <input type="text" placeholder="Odd Future Sk8 Hi" bind:value={shoe3}>

    <button on:click={handlesubmit} >Run the Numbers</button>
</Box>