<script lang="ts">
	
</script>

<!-- <svelte:head>
	<title>Activities Catalogue</title>
	<meta name="description" content="About this app" />
</svelte:head> -->

<div class="content">
	<!--Information pulled from inputs-->

	<table>
		<th>Your Activities</th>
		<th>Time</th>
			<tr>
				<td>Movie Night</td>
				<td>8:00 - 9:00 PM</td>
			</tr>
	</table>

	<!--Information pulled from CampusGroups-->
	
	<table>
		<th>RIT Events</th>
			<tr>
				<td>Women in Computing Boston Trip </td>
				<td>Juggling Club Meet</td>
			</tr>
	</table>

</div>

<style>
	table{
		width: 50%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}
</style>
