<script lang="ts">
</script>

<svelte:head>
	<script src="https://kit.fontawesome.com/cc7ada224f.js" crossorigin="anonymous"></script>
	<title>Home</title>
	<meta name="description" content="Home page" />
</svelte:head>

<section>
	
	<h2 class = "category_heading" style = "font-color: #35424a">Classes</h2>
	<a href="calendar">
		<div class="category_box" style="background-color: rgba(208,211,212,.90)">
			<p class="category_black">GCIS 123: Gol 1459</p>
			<div class="time" style="width:100%">
				<i class="fa-solid fa-clock whicon"></i>
				<p class="description">12:00</p>
				<i class="fa-solid fa-location-dot whicon"></i>
				<p class="description">0.2mi</p>
			</div>
		</div>
	</a>

	<h2 class = "category_heading">Dining</h2>
	<a href="calendar">
		<div class="category_box" style="background-color: rgba(132, 189, 0, .65)">
			<p class="white">Ritz Sports Arena</p>
			<div class="time" style="width:100%">
				<i class="fa-solid fa-clock whicon"></i>
				<p class="description">12:00 - 4:00</p>
				<i class="fa-solid fa-location-dot whicon"></i>
				<p class="description">0.2mi</p>
			</div>
		</div>
	</a>

	<h2 class = "category_heading">Lounges</h2>
	<a href="calendar">	
		<div class="category_box" style="background-color: rgba(0,156,189,.65)">
			<p class="white">Fireside Lounge</p>
			<div class="time" style="width:100%">
				<i class="fa-solid fa-clock whicon"></i>
				<p class="description">0.2mi</p>
			</div>
		</div>
	</a>

	<h2 class = "category_heading">Activties</h2>
	<a href="calendar">
		<div class="category_box" style="background-color: rgba(218, 41, 28,.65)">
			<p class="white">Wiedman Fitness Center</p>
			<div class="time" style="width:100%">
				<i class="fa-solid fa-clock whicon"></i>
				<p class="description">6am - 11pm</p>
				<i class="fa-solid fa-location-dot whicon"></i>
				<p class="description">0.2mi</p>
			</div>
		</div>
	</a>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	.time {
		display: flex;
		flex-direction: row;
		text-align: right;
		float: right;
		justify-content: flex-end;
	}

	.category_heading {
		width: 100%;
		font-weight: bold;
		font-size: 26px;
		text-align: center;
	}

	.white {
		color:white;
	}
	.category_box {
		width: 322px;
		padding: 15px;
		padding-top: 10px;
		border: 10px;
		height: 90px;
		text-align: center;
		border-radius: 15px;
		color: white;
		font-size: 20px;
	}

	.whicon {
		color: white;
		position: relative;
		right: 5px;
		top: 5px;
	}

	.category_black {
		color: #35424a
	}

	.description {
		margin: 0;
		margin-right: 10px;
		font-size: 14px;
		padding-top: 6px;

	}
</style>
