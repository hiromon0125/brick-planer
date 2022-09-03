<script>
	import { menuState } from '$lib/store';
	$: menuState.subscribe(() => {
		console.log('menu open');
	});
</script>

<img
	on:click={() => {
		menuState.update((n) => !n);
	}}
	src="munson.jpg"
	alt="munson"
/>

<style>
	img {
        width: 80px;
		clip-path: circle();
		margin: 20px;
		overflow: hidden;
	}

    img:hover {
        opacity: 0.5;
    }
</style>
