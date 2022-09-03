<script lang="ts">
    //Sat Sep 03 2022
    /*let todayDate = new Date();
    let weekDay = "" + todayDate.getDate();
    let month = "" + todayDate.getMonth();
    let day = "" + todayDate.getDay();
    let year = "" + todayDate.getFullYear();
    let date = "Todays Date: " + weekDay + month + day + year;*/
    let date = new Date();
    let mon = 29;
    let tue = 30;
    let wed = 31;
    let thu = 1;
    let fri = 2;
    let sat = 3;
    let sun = 4;

</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="content">
	<h1>Current Classes</h1>
    <p id="date">
        {date}
    </p>

    <div class="days">
        <p class="days">Mon<br>{mon}</p>
        <p class="days">Tue<br>{tue}</p>
        <p class="days">Wed<br>{wed}</p>
        <p class="days">Thu<br>{thu}</p>
        <p class="days">Fri<br>{fri}</p>
        <p class="days" id="today">Sat<br>{sat}</p>
        <p class="days">Sun<br>{sun}</p>
    </div>

    <section>
        <a href="calendar_extend">
            <p class = "category_box category_black" style="background-color: rgba(208,211,212,.90)">GCIS 123: GOL 1459</p>
        </a>
        <a href="calendar">
            <p class = "category_box" style="background-color: rgba(132,189,.65)">BIOL 101: GOS 1250</p>
        </a>
        <a href="calendar">	
            <p class = "category_box" style="background-color: rgba(0,156,189,.65) ">MATH 182: GOS 1350</p>
        </a>
        <a href="calendar">
            <p class = "category_box" style="background-color: rgba(218,41,28,.65) ">RIT 365: GLE 2150</p>
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
    #today
    {
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
		color: #35424a
	}
</style>