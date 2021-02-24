<script>
    import Box from "../components/Box.svelte";
    let shoe1 = undefined;
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
	}

    input {
        border-radius: 10px;
        border-style: hidden;
        margin: auto;
        align-content: center;
    }
</style>

<h3>Input your 3 favorite sneaks</h3>

<Box>
    <p>No. 1</p>
    <input type="text" placeholder="Dusty Jordan 1">
    <p>No. 2</p>
    <input type="text" placeholder="Nike Dunk Low Pine Green">
    <p>No. 3</p>
    <input type="text" placeholder="Odd Future Sk8 Hi">
</Box>