<script lang="ts">
	import { page } from '$app/stores';
	import MunsonBtn from './munsonBtn.svelte';
	let listOfTitles: { [key: string]: string } = {
		'/': 'Home',
		'/about': 'About',
		'/calendar': 'Calendar',
		'/activities': 'Activities'
	};

	// $page.url.pathname === '/about'
</script>

<header>
	<div class="corner">
		<MunsonBtn />
	</div>
	<h1>{listOfTitles[$page.url.pathname]}</h1>

	<div class="corner">
		<!-- TODO put something else here? github link? -->
	</div>
</header>

<style>
	h1 {
		margin: 0;
		margin-top: 15px;
	}

	header {
		display: flex;
		justify-content: space-between;
		position: relative;
		height: 4rem;
	}

	.corner {
		width: 3rem;
	}
</style>
