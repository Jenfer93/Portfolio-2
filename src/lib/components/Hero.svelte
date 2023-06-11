<script lang="ts">
	import Down from '../images/1492533501-arrow-30_83308.svg';
</script>

<div>
	<h1>Front End Developer</h1>
	<h2>Jenny Feragen</h2>
	<p>
		Scroll down to learn more <br />
		<a href="#myWork"><img src={Down} alt="down arrow" /></a>
	</p>
</div>

<style lang="scss">
	div {
		color: var(--primary);
		min-height: 100vh;
		text-align: center;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		overflow: hidden;
	}

	h1 {
		font-size: var(--font-size-xxxl);
		margin: var(--spacing-null);
		animation: 1s slide-up; 
	}

	@keyframes slide-up {
		from {
			margin-top: 100vw;
			height: 300%; 
		}

		to {
			margin-top: 0%;
			height: 100%;
		}
	}


	h2 {
		font-size: var(--font-size-xl);
	}

	p {
		font-style: italic;
	}

	img {
		width: 50px;
		height: 50px;
		animation: 2s linear infinite 0s bounce;
		filter: invert(96%) sepia(7%) saturate(1005%) hue-rotate(315deg) brightness(101%) contrast(90%);
	}

	@keyframes bounce {
		from {
			/* pushes the sun down past the viewport */
			transform: translateY(1vh);
		}
		to {
			/* returns the sun to its default position */
			transform: translateY(5vh);
		}
	}

	@media only screen and (max-width: 600px) {
		div {
			min-height: 100vh;
		}

		h1 {
			font-size: var(--font-size-xxl);
		}

		h2 {
			font-style: var(--font-size-m);
		}
	}
</style>
