<script lang="ts">
	import { goto } from '$app/navigation';
	import { page } from '$app/stores';
	import MunsonBtn from './munsonBtn.svelte';
	let listOfTitles: { [key: string]: string } = {
		'/': 'Home',
		'/about': 'About',
		'/calendar': 'Calendar',
		'/activities': 'Activities',
		'/setting': 'Settings'
	};

	// $page.url.pathname === '/about'
</script>

<header>
	<div class="corner">
		<MunsonBtn />
	</div>
	<h1>{listOfTitles[$page.url.pathname]}</h1>

	<div class="corner">
		<img
			on:click={() => {
				goto('https://mycourses.rit.edu/');
			}}
			class="logo"
			src="/rit.png"
			alt=""
		/>
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
		box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
		padding-bottom: 6px;
	}

	.corner {
		position: relative;
		width: 3rem;
	}

	.logo {
		height: 2.4rem;
		margin: 15px;
		position: absolute;
		right: 0;
	}
</style>
