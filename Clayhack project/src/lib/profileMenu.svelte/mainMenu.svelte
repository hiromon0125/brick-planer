<script>
	import { menuState } from '$lib/store';
</script>

{#if $menuState}
	<div class="menu-container">
		<button
			on:click={() => {
				menuState.update((n) => !n);
			}}
			class="exit">X</button
		>
        <div class="profile">
            <img src="munson.jpg" alt="munson"/>
            <div class="profile-info">
                <h1 class="name-title">David Munson</h1>
                <p class="email">munsonisgoated@rit.edu</p>
            </div>
        </div>
        <p>munson</p>
        <p>munson</p>
        <p>munson</p>

	</div>
    <div class="curtain"></div>
    {/if}

<style>
	.menu-container {
		background-color: #fff;
		display: flex;
        flex-direction: column;
        position: absolute;
		width: 70%;
		height: 100vh;
		border: black 1px solid;
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
        background-color: rgba(0,0,0,0.7);
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
</style>
