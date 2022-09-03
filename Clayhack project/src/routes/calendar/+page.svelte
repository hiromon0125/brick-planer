<script lang="ts">
	//Document.getElementById("date").innerHTML = Date();
</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="content">
	<h1>Current Classes</h1>
	<p id="date">Date </p>

	<ul>
		<li style="display:inline">Sun</li>
		<li style="display:inline">Mon</li>
		<li style="display:inline">Tue</li>
		<li style="display:inline">Wed</li>
		<li style="display:inline">Thur</li>
		<li style="display:inline">Sun</li>
	</ul>

	<pre>npm create svelte@latest</pre>

	<p>
		The page you're looking at is purely static HTML, with no client-side interactivity needed.
		Because of that, we don't need to load any JavaScript. Try viewing the page's source, or opening
		the devtools network panel and reloading.
	</p>

	<p>
		The <a href="/todos">TODOs</a> page illustrates SvelteKit's data loading and form handling. Try using
		it with JavaScript disabled!
	</p>
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

</style>