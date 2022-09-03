<script lang="ts">
</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>
<div class="content">
	<h1 id="text-align">GCSIS 123 | GOL 1459</h1>
	<img
		id="center"
		src="https://www.rit.edu/computing/sites/rit.edu.computing/files/images/jumbotron/computing-departments-jumbotron.jpg"
		alt="GCSIS 123"
	/>
	<p id="center">
		A first course introducing students to the fundamentals of computational problem solving.
		Students will learn a systematic approach to problem solving, including how to frame a problem
		in computational terms, how to decompose larger problems into smaller components, how to
		implement innovative software solutions using a contemporary programming language, how to
		critically debug their solutions, and how to assess the adequacy of the software solution.
		Additional topics include an introduction to object-oriented programming and data structures
		such as arrays and stacks. Students will complete both in-class and out-of-class assignments.
		Lab 6 (Fall, Spring).
	</p>
	<iframe
		src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2913.955434066646!2d-77.68219628452063!3d43.084432279144906!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89d14c5f0e79fc29%3A0x7d07467604d60318!2sGolisano%20College%20of%20Computing%20and%20Information%20Sciences!5e0!3m2!1sen!2sus!4v1662234584833!5m2!1sen!2sus"
		width="600"
		height="450"
		style="border:0;"
		loading="lazy"
		referrerpolicy="no-referrer-when-downgrade"
		title="google map of the classroom"
	/>
</div>

<style>
	iframe {
		width: 100%;
	}
	.content {
		width: 100%;
		max-width: var(--column-width);
	}
	h1 {
		width: 100%;
		font-weight: bold;
	}
	#center {
		align-items: center;
		width: 500px;
	}
	#text-align {
		text-align: left;
	}
	#center {
		text-align: center;
	}
</style>
