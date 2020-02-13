<nav id="nav" class:active>
	<a use:scrolltotop href='.' class="logo"><Logo /></a>
	<button class="menu-toggle" on:click="{() => active = !active}">
		<div class="stack top"></div>
		<div class="stack middle"></div>
		<div class="stack bottom"></div>
	</button>
	<ul on:click="{() => active = !active}">
		
		<li on:click="{() => active = !active}"><a  use:scrollto={'#whatWeDo'} class:selected='{segment === "./#whatWeDo"}' href="#whatWeDo" id="#whatWeDoLink">What we do</a></li>
		<li><a use:scrollto={'#howWeDoIt'} class:selected='{segment === "./#howWeDoIt"}' href="#howWeDoIt">How we do it</a></li>
		<li><a use:scrollto={'#contact'} class:selected='{segment === "./#contact"}' href="#contact">How to reach us</a></li>
	</ul>
</nav>


<script>
	export let segment;
	import { scrollto, scrolltotop } from "svelte-scrollto";
	import * as animateScroll from "svelte-scrollto";
	import Logo from "../components/Logo.svelte";

	let active = false;
	
	animateScroll.setGlobalOptions({
	duration: 1660,
	offset: -100,
	onStart: (element, offset) => {
        if(element) {
			console.log("Start scrolling to element:", element.id);
			let navBe = document.getElementById('nav');
			navBe.classList.remove('active');
        } else if(offset) {
            console.log("Start scrolling to page offset: (${offset.x}, ${offset.y})");
        }
    }
    
})
</script>

<style>
	nav {
		border: 1px solid #c4c4c4;
		border-width: .5rem 0 0;
		font-weight: 300;
		padding: 0 1em;
		background: #fff;
		position: fixed;
		z-index: 999;
		margin: 0 .5rem;
		width: calc(100vw - 1rem);
		height: 5.5rem;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.menu-toggle {
		z-index: 1;
		height: calc(1rem + 1px);
		width: 2.5rem;
		position: relative;
		padding: 0;
		margin: 0; 
		background: transparent;
		border: none;
	}
	.menu-toggle:focus {
		outline: none !important;
	}
	.menu-toggle .stack {
		height: 1px;
		width: 2.5rem;
		background: #2b9e8d;
		position: absolute;
		left: 0;
	}
	.menu-toggle .stack.top {
		top: 0;
		transition: .66s;
		transition: top .66s .66s, transform .66s;
	}
	.menu-toggle .stack.middle {
		top: .5rem;
		transform: scaleX(1);
		transition: transform .21s 1s;
	}
	.menu-toggle .stack.bottom {
		bottom: 0;
		transition: bottom .66s .66s, transform .66s;
	}
	.active .menu-toggle .stack.top {
		top: .5rem;
		transition: top .66s, transform .66s .66s;
		transform: rotate(-45deg);
	}
	.active .menu-toggle .stack.middle {
		transition: transform .21s;
		transform: scaleX(0);
	}
	.active .menu-toggle .stack.bottom {
		bottom: .5rem;
		transition: bottom .66s, transform .66s .66s;
		transform: rotate(45deg);
	}
	.logo :global(svg) {
		width: 10rem;
		height: auto;
	}
	ul {
		position: absolute;
		left: 0;
		right: 0;
		top: 0;
		bottom: 0;
		margin: 0;
		padding: 1rem;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		background: #fff;
		height: calc(100vh - 5rem);
		overflow: hidden;
		transform: translateY(-100vh);
		transition: .66s;
	}
	.active ul {
		transform: translateY(0);
		transition: .66s;
	}

	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: left;
	}

	.selected {
		position: relative;
		display: inline-block;
	}

	.selected::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 2px;
		background-color: #2b9e8d;
		display: block;
		bottom: -1px;
	}

	a {
		text-decoration: none;
		padding: 1em 0.5em;
		display: block;
	}
	@media (min-width: 480px) {
		nav {
			border-width: 1.5rem 0 0;
			margin: 0 1.5rem;
			width: calc(100vw - 3rem);
			justify-content: flex-start;
		}
		.logo {
			height: 3rem;
			display: flex;
			padding: 0;
		}
		.logo :global(svg) {
			width: 10rem;
			height: auto;
		}
		ul {
			position: relative;
			left: inherit;
			right: inherit;
			top: inherit;
			bottom: inherit;
			padding: 0;
			display: flex;
			flex-direction: row;
			align-items: center;
			background: transparent;
			height: inherit;
			overflow: inherit;
			transform: inherit;
			transition: .66s;
		}
		.menu-toggle {
			display: none;
		}
	}
</style>

