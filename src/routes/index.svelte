<svelte:head>
	<title>HABIT66 | Change for good.</title>
</svelte:head>

<!-- <svelte:window bind:innerHeight={sectionElement} /> -->

<div class="hero">
	<Logo classname="hero-logo" />
	<h1>Change for good.</h1>
</div>

<section id="whatWeDo">
	<h1>Some words speak louder than actions.</h1>

	<p>Most of advertising tries to get people to feel some thing or think some way about a brand. But when it comes to health, it takes more than good juju and good intentions to move people.</p>

	<p>We go one step further. We create healthcare communications designed to make people change how they act. And we help make those new behaviors so routine, people don’t even have to think about them.</p>

	<p>Sound like mind control? It’s even cooler than that.</p>
</section>

<section id="howWeDoIt">
	<h1>We break it. Then fix it.</h1>
	<p>Studies show that it takes, on average, 21 days to break a habit. And 66 days to make a new one. </p>

	<p>It’s not easy to shake people out of the behaviors that they do on autopilot. Unless you know what you’re doing. (Guess what?? We do.)</p>
	<h2>
		Smarter nerds
	</h2>
	<p>Our HABIT66 team is not your traditional advertising roster. We hire people with backgrounds in behavioral economics and behavioral psychology. People who know the latest evidence-based strategies to change not just the minds of your audience, but truly, their actions. This very specific set of skills is bolstered through our exclusive partnership with the Behavioral Economics team at <a href="https://www.cmu.edu/dietrich/behavioral-economics/index.html" target="_blank">Carnegie Mellon University</a>. </p>
	<a href="https://www.cmu.edu/dietrich/behavioral-economics/index.html" target="_blank"><CmuLogo /></a>
	<h2>Bigger data</h2>
	<p>As part of W2O group, we leverage AOS, the best-in-class, propriety analytics platform. Want to know what a doctor prescribed last month? You probably know that already. But want to know what else she did that day? And why? And what she’ll prescribe next month? That’s AOS. We’ve mapped the digital footprint of 1.1 million health ecosystem profiles, including physicians, healthcare advocates, patients, and hospitals in 173 countries around the world. Boom.</p>
	<a href="https://www.w2ogroup.com/analytics/" target="_blank"><W2oLogo /></a>
</section>

<section id="contact">
	<h1>Expectations, like habits, were meant to be broken. </h1>
	<p>You give us the behavior you want to change. We’ll give you a plan for the first 66-days. </p>
	<p>
	Contact us at <a href="mailto:hello@habit66.com">hello@habit66.com</a>
	</p>
</section>


<script>
	import Logo from '../components/Logo.svelte';
	import CmuLogo from '../components/CmuLogo.svelte';
	import W2oLogo from '../components/W2oLogo.svelte';
	// import { onMount } from 'svelte';

	// let sectionElement;
	// let x;

	// onMount(() => {
	// 	x = sectionElement;
	// })

	// let hashVisible = sectionElement.getBoundingClientRect().bottom <= window.innerHeight;
	
</script>

<style>
	h1, p {
		text-align: center;
		margin: 0 auto;
	}

	h1 {
		font-size: 1.4em;
		text-transform: uppercase;
		margin: 0 0 1.5em 0;
	}



	p {
		font-size: 1.5rem;
		margin: 1em 0;
	}
	.hero {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		padding: 4rem;
		min-height: calc(100vh - 3rem);
		margin-bottom: 4rem;
	}
	section {
		padding: 2rem;
		max-width: 52rem;
		min-height: 100vh;
		display: flex;
		flex-direction: column;
		justify-content: center;
	}
	section p, section h1 {
		text-align: left;
	}
	h2 {
		margin-top: 4rem;
	}
	@media (min-width: 480px) {
		h1 {
			font-size: 2em;
		}
	}
</style>