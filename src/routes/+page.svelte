<main>
	<h1>Welcome to FunkyKit</h1>
	<p>
		bad => Refresh and see animation play twice (it shouldn't) <br />
		Ok so the issue seems to have something with what's in layout...
	</p>
</main>

<style>
	main {
		min-height: 100vh;
		background-color: rgb(231, 231, 231);

		display: flex;
		justify-content: center;
		align-items: center;

		flex-direction: column;
	}

	/* this is where things go south */
	h1 {
		animation: intro 0.5s;
	}

	@keyframes intro {
		from {
			transform: translateY(-50px);
		}
	}
</style>
