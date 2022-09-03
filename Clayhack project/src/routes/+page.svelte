<script lang="ts">
	import Counter from '$lib/Counter.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Home page" />
</svelte:head>

<section>
	<h1>Home</h1>

<<<<<<< HEAD
	
	<h2 class = category_heading style = "font-color: #35424a">Classes</h2>
	<a href="calendar">
		<p class = category_box style="background-color: rgba(208,211,212,.90)">GCIS 123: Gol 1459</p>
	</a>
	
	
	<h2 class = category_heading>Dining</h2>
	<a href="calendar">
		<p class = category_box style="background-color: rgba(132,189,.65)">GCIS 123: Gol 1459</p>
	</a>

	<h2 class = category_heading>Lounges</h2>
	<a href="calendar">	
		<p class = category_box style="background-color: rgba(0,156,189,.65) ">GCIS 123: Gol 1459</p>
	</a>

	<h2 class = category_heading>Activties</h2>
	<a href="calendar">
		<p class = category_box style="background-color: rgba(218,41,28,.65) ">GCIS 123: Gol 1459</p>
	</a>
=======
	<div>
		<h2 class="category_heading">Classes</h2>
		<p class="category_box" style="background-color: rgba(208,211,212,.65)">GCIS 123: Gol 1459</p>
	</div>

	<div>
		<h2 class="category_heading">Dining</h2>
		<p class="category_box" style="background-color: rgba(132,189,.65)">GCIS 123: Gol 1459</p>
	</div>

	<div>
		<h2 class="category_heading">Lounges</h2>
		<p class="category_box">GCIS 123: Gol 1459</p>
	</div>
>>>>>>> c64d8e61b9a5f71668b57b92221eb7fb77d0397d
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	h1 {
		width: 100%;
		font-weight: bold;
	}

	.category_heading {
		width: 100%;
		font-weight: bold;
		font-size: 26px;
		text-align: center;
	}

	.category_box {
		width: 322px;
		padding: 15px;
		padding-top: 40px;
		border: 10px;
		height: 50px;
		text-align: center;
		border-radius: 15px;
		color: white;
		font-size: 20px;
	}


	.category_white {
		color: #35424a
	}
</style>
