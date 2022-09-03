<script lang="ts">
	
</script>

<!-- <svelte:head>
	<title>Activities Catalogue</title>
	<meta name="description" content="About this app" />
</svelte:head> -->
<!--Table not actually connected to .js. Simply aesthetic-->

<div class="content">

	<!--Information to be pulled from inputs-->
	<h1>Activites Catalogue</h1>
	<table>
		<th>Your Activities</th>
		<th>Date</th>
		<th>Time</th>
		<th>Location</th>
			<tr>
				<td>Movie Night</td>
				<td>9/26/2022</td>
				<td>8:00 - 9:00 PM</td>
				<td>Greek Lawn</td>
			</tr>
			<tr>
				<td>Nine Gates Mahjong</td>
				<td>Friday, 9/9/2022</td>
				<td>5:00 - 6:00 PM</td>
				<td>Campus Center, 2nd Floor Lobby</td>
			</tr>
	</table>

	<p></p>

	<!--Information to be pulled from CampusGroups-->
	<h1>RIT Events</h1>
	<table>
		<th>RIT Events</th>
		<th>Date</th>
		<th>Time</th>
		<th>Location</th>
			<tr>
				<td>Women in Computing Boston Trip </td>
				<td>9/12/2022</td>
				<td>All Day</td>
				<td>TBD</td>
			</tr>
			<tr>
				<td>Juggling Club</td>
				<td>xx.xx.xxxx</td>
				<td>5:00 - 6:00 PM</td>
				<td>Student Alumni Union</td>
			</tr>
	</table>

</div>

	<!--table borders and width adjustments-->
<style>
	table{
		width: 100%;
		height: 50%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}
	table, th, td {
  border: 1px;
		text-align: center;
		color: rgb(255, 255, 255);
		padding: 20px;
	}
	th {background-color: rgb(218 41 28);}
	td {background-color: rgb(172 163 154);}
</style>
