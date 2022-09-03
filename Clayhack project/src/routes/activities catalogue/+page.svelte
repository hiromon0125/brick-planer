<script lang="ts">
	
</script>

<!-- <svelte:head>
	<title>Activities Catalogue</title>
	<meta name="description" content="About this app" />
</svelte:head> -->

<div class="content">
	<!--Information pulled from inputs-->
	<h1>Your Activities</h1>

	<table>
		<tr>
			<td>Movie Night</td>
			<td>Women in Business</td>
		</tr>
	</table>

	<!--Information pulled from CampusGroups-->>
	<h1>RIT Events</h1>

	<table>
		<tr>
			<td>Women in Computing Boston Trip </td>
			<td>Juggling Club Meet</td>
		</tr>
	</table>

</div>

<style>
	.content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}
</style>
