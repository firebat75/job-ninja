<script>
	import successkid from "images/successkid.jpg";
	import { onMount } from "svelte";

	onMount(() => {
		//safe for browser only code
		console.log("only ever runs in the browser");
	});

	console.log("home");
</script>

<svelte:head>
	<title>Job Ninja</title>
</svelte:head>

<div>
	<img src="no-text-logo.png" alt="" />
	<h1>Jobs for Ninjas!</h1>
	<p>Find your next assignment here.</p>
	<a href="jobs" class="btn">New Jobs</a>
</div>

<style>
	h1,
	p {
		text-align: center;
		margin: 0 auto;
	}

	h1 {
		font-size: 2em;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0, 0, 0.5em, 0;
	}

	img {
		width: 200px;
		margin: 0 auto;
		display: block;
	}

	a {
		margin-top: 40px;
	}

	div {
		margin-top: 60px;
		text-align: center;
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
		}
	}
</style>
