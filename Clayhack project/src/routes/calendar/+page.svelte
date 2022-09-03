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
        <a class = "class-desc-container" href="class">
            <div class="category_box" style="background-color: rgba(208,211,212,.90)">
                <p class="category_black">GCIS 123 | Gol 1459</p>
                <div class="time" style="width:100%">
                    <i class="fa-solid fa-clock whicon"></i>
                    <p class="description">9:00 AM</p>
                    <i class="fa-solid fa-location-dot whicon"></i>
                    <p class="description">0.2mi</p>
                </div>
            </div>
        </a>
        <a class = "class-desc-container" href="class">
            <div class="category_box" style="background-color: rgba(132, 189, 0, .65)">
                <p class="white">BIOL 101 | GOS 1250</p>
                <div class="time" style="width:100%">
                    <i class="fa-solid fa-clock whicon"></i>
                    <p class="description">12:00 PM</p>
                    <i class="fa-solid fa-location-dot whicon"></i>
                    <p class="description">0.3mi</p>
                </div>
            </div>
        </a>
        <a class = "class-desc-container" href="class">	
            <div class="category_box" style="background-color: rgba(0,156,189,.65)">
                <p class="white">MATH 182 | GOS 1350</p>
                <div class="time" style="width:100%">
                    <i class="fa-solid fa-clock whicon"></i>
                    <p class="description">2:00 PM</p>
                    <i class="fa-solid fa-location-dot whicon"></i>
                    <p class="description">0.0mi</p>
                </div>
            </div>
        </a>
        <a class = "class-desc-container" href="class">
            <div class="category_box" style="background-color: rgba(218, 41, 28,.65)">
                <p class="white">RIT 365 | GLE 2150</p>
                <div class="time" style="width:100%">
                    <i class="fa-solid fa-clock whicon"></i>
                    <p class="description">8:00 PM</p>
                    <i class="fa-solid fa-location-dot whicon"></i>
                    <p class="description">0.1mi</p>
                </div>
            </div>
        </a>
	</section>
</div>

<style>
    .class-desc-container {
        margin-top: 2rem;
    }

	.content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
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
	h1 {
		width: 100%;
		font-weight: bold;
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
		z-index: 100;
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
