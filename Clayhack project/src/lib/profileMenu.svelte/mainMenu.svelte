<script>
	import { menuState } from '$lib/store';

	function menuStateChange() {
		menuState.update((n) => !n);
	}
</script>

{#if $menuState}
	<div class="menu-container">
		<button on:click={menuStateChange} class="exit"><i class="fa-solid fa-x"></i></button>
		<div class="profile">
			<img src="munson.jpg" alt="munson" />
			<div class="profile-info">
				<h1 class="name-title">David Munson</h1>
				<p class="email">munsonisgoated@rit.edu</p>
			</div>
		</div>
		<a class="link" on:click={menuStateChange} href="/"> <i class="fa-solid fa-house" />Home</a>
		<a class="link" on:click={menuStateChange} href="calendar">
			<i class="fa-solid fa-calendar" />Calendar</a
		>
		<a class="link" on:click={menuStateChange} href="activities"
			><i class="fa-solid fa-flag" /> Activties</a
		>
		<a class="link" on:click={menuStateChange}><i class="fa-solid fa-heart" />Favorite Locations</a>
		<a class="link" on:click={menuStateChange}><i class="fa-solid fa-bowl-food" />Food Locations</a>
	</div>
	<div class="curtain" on:click={menuStateChange} />
{/if}

<style>
	.menu-container {
		background-color: #fff;
		display: flex;
		flex-direction: column;
		position: absolute;
		width: 70%;
		height: 100vh;
		top: 0;
		left: 0;
		z-index: 10000;
		align-items: stretch;
	}

	.exit {
		width: 50px;
		height: 50px;
		background-color: transparent;
		border: none;
	}

	.curtain {
		position: absolute;
		width: 30%;
		height: 100vh;
		background-color: rgba(0, 0, 0, 0.7);
		top: 0;
		right: 0;
	}

	img {
		width: 10rem;
		clip-path: circle();
	}

	.profile {
		display: flex;
		flex-direction: column;
		align-items: center;
		text-align: center;
	}

	.name-title {
		margin-bottom: 0;
	}

	.email {
		margin-top: 0;
		opacity: 0.5;
	}

	a {
		padding-top: 1rem;
		padding-bottom: 1rem;
		font-size: 3vh;
		display: flex;
		flex-direction: row;
	}

	i {
		margin-left: 1rem;
		margin-right: 1rem;
	}

	a:hover {
		background-color: rgba(255, 62, 0, 0.4);
	}

	.exit:hover {
		opacity: 0.4;
	}
</style>
