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
        <p class="days">Mon ({mon})</p>
        <p class="days">Tue ({tue})</p>
        <p class="days">Wed ({wed})</p>
        <p class="days">Thu ({thu})</p>
        <p class="days">Fri ({fri})</p>
        <p class="days">Sat ({sat})</p>
        <p class="days">Sun ({sun})</p>
    </div>

    <div class="planner">8:00 AM</div>
    <div class="planner">9:00 AM</div>
    <div class="planner">10:00 AM</div>
    <div class="planner">11:00 AM</div>
    <div class="planner">12:00 PM</div>
    <div class="planner">1:00 PM</div>
    <div class="planner">2:00 PM</div>
    <div class="planner">3:00 PM</div>
    <div class="planner">4:00 PM</div>
    <div class="planner">5:00 PM</div>
    <div class="planner">6:00 PM</div>
    <div class="planner">7:00 PM</div>
    <div class="planner">8:00 PM</div>
    <div class="planner">9:00 PM</div>
    <div class="planner">10:00 PM</div>
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
        flex-direction: row;
        justify-content: space-evenly;
    }
    .planner {
        display: flex;
        align-items: center;
        justify-content: flex-end;
        border-top: thin dotted;
    }

</style>