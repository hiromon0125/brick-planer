<script lang="ts">
	let mon = 29;
	let tue = 30;
	let wed = 31;
	let thu = 1;
	let fri = 2;
	let sat = 3;
	let sun = 4;
	let time = new Date();
	$: currentDate = time.getDay();
	$: console.log(currentDate);
</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="content">
	<h1>Current Classes</h1>

	<div class="days">
		<p class="days" class:today={currentDate == 1}>Mon<br />{mon}</p>
		<p class="days" class:today={currentDate == 2}>Tue<br />{tue}</p>
		<p class="days" class:today={currentDate == 3}>Wed<br />{wed}</p>
		<p class="days" class:today={currentDate == 4}>Thu<br />{thu}</p>
		<p class="days" class:today={currentDate == 5}>Fri<br />{fri}</p>
		<p class="days" class:today={currentDate == 6}>Sat<br />{sat}</p>
		<p class="days" class:today={currentDate == 7}>Sun<br />{sun}</p>
	</div>

	<section>
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
</div>

<style>
	.content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}

	#date {
		text-align: center;
	}
	.days {
		display: flex;
		align-items: center;
		text-align: center;
		flex-direction: row;
		justify-content: space-evenly;
	}
	.today {
		color: orange;
		font-weight: bold;
	}
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
	.category_black {
		color: #35424a;
	}
</style>
