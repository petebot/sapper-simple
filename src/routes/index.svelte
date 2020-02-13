<svelte:head>
	<title>Title</title>
</svelte:head>

<!-- <svelte:window bind:innerHeight={sectionElement} /> -->

<div class="hero">
	<Logo classname="hero-logo" />
	<h1>Change for good.</h1>
</div>

<section id="whatWeDo">
	<h1>Theophrastus mediocriterne delectat, cum tractat locos ab Aristotele ante tractatos?</h1>

	<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Hoc non est positum in nostra actione. Qui est in parvis malis. Quippe: habes enim a rhetoribus; Quippe: habes enim a rhetoribus; Duo Reges: constructio interrete. <b>Hic ambiguo ludimur.</b> </p>

	<ol>
		<li>Quodcumque in mentem incideret, et quodcumque tamquam occurreret.</li>
		<li>At eum nihili facit;</li>
		<li>Sed vos squalidius, illorum vides quam niteat oratio.</li>
		<li>Quid, si etiam iucunda memoria est praeteritorum malorum?</li>
	</ol>


	<blockquote cite='http://loripsum.net'>
		Quacumque enim ingredimur, in aliqua historia vestigium ponimus.
	</blockquote>


	<p>Sed in rebus apertissimis nimium longi sumus. Equidem e Cn. <i>Quid dubitas igitur mutare principia naturae?</i> Ergo hoc quidem apparet, nos ad agendum esse natos. </p>

	<ul>
		<li>Itaque mihi non satis videmini considerare quod iter sit naturae quaeque progressio.</li>
		<li>Quis istud, quaeso, nesciebat?</li>
		<li>Nos vero, inquit ille;</li>
		<li>Sed ad illum redeo.</li>
	</ul>



</section>

<section id="howWeDoIt">
	<h1>Ex rebus enim timiditas, non ex vocabulis nascitur.</h1>

	<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suo genere perveniant ad extremum; Idem adhuc; Quodsi ipsam honestatem undique pertectam atque absolutam. Erit enim mecum, si tecum erit. Duo Reges: constructio interrete. </p>

	<blockquote cite='http://loripsum.net'>
		Quia voluptatem hanc esse sentiunt omnes, quam sensus accipiens movetur et iucunditate quadam perfunditur.
	</blockquote>

	<h2>Look at that</h2>


	<ol>
		<li>Nulla erit controversia.</li>
		<li>Qui autem esse poteris, nisi te amor ipse ceperit?</li>
		<li>Quod autem meum munus dicis non equidem recuso, sed te adiungo socium.</li>
		<li>Non quam nostram quidem, inquit Pomponius iocans;</li>
	</ol>


	<p><a href='http://loripsum.net/' target='_blank'>Hoc etsi multimodis reprehendi potest, tamen accipio, quod dant.</a> Falli igitur possumus. Sed virtutem ipsam inchoavit, nihil amplius. Addidisti ad extremum etiam indoctum fuisse. <a href='http://loripsum.net/' target='_blank'>Respondent extrema primis, media utrisque, omnia omnibus.</a> Si verbum sequimur, primum longius verbum praepositum quam bonum. </p>

	<ul>
		<li>Aufidio, praetorio, erudito homine, oculis capto, saepe audiebam, cum se lucis magis quam utilitatis desiderio moveri diceret.</li>
		<li>Quacumque enim ingredimur, in aliqua historia vestigium ponimus.</li>
		<li>Haec bene dicuntur, nec ego repugno, sed inter sese ipsa pugnant.</li>
		<li>Ut pulsi recurrant?</li>
	</ul>



</section>

<section id="contact">
	<h1>Negat esse eam, inquit, propter se expetendam.</h1>

	<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. <a href='http://loripsum.net/' target='_blank'>Itaque contra est, ac dicitis;</a> Sed vos squalidius, illorum vides quam niteat oratio. Negare non possum. Duo Reges: constructio interrete. </p>

	<ul>
		<li>At ego quem huic anteponam non audeo dicere;</li>
		<li>Paulum, cum regem Persem captum adduceret, eodem flumine invectio?</li>
		<li>Ita relinquet duas, de quibus etiam atque etiam consideret.</li>
		<li>Quid ergo aliud intellegetur nisi uti ne quae pars naturae neglegatur?</li>
		<li>Familiares nostros, credo, Sironem dicis et Philodemum, cum optimos viros, tum homines doctissimos.</li>
		<li>Qua tu etiam inprudens utebare non numquam.</li>
	</ul>


	<blockquote cite='http://loripsum.net'>
		Octavio fuit, cum illam severitatem in eo filio adhibuit, quem in adoptionem D.
	</blockquote>


	<ol>
		<li>Quae qui non vident, nihil umquam magnum ac cognitione dignum amaverunt.</li>
		<li>Modo etiam paulum ad dexteram de via declinavi, ut ad Pericli sepulcrum accederem.</li>
		<li>Pisone in eo gymnasio, quod Ptolomaeum vocatur, unaque nobiscum Q.</li>
	</ol>


	<p>An eiusdem modi? <a href='http://loripsum.net/' target='_blank'>Restinguet citius, si ardentem acceperit.</a> Itaque hic ipse iam pridem est reiectus; <a href='http://loripsum.net/' target='_blank'>Philosophi autem in suis lectulis plerumque moriuntur.</a> Sed quot homines, tot sententiae; <b>Si longus, levis;</b> </p>


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