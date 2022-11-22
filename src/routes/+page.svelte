<main>
	<!-- hint: go look in layout... -->
	<h1>This text uses a normal css animation (non js friendly one ❤)</h1>
	<p>
		<strong>Bug:</strong> Animation plays twice on load!?. <br />
		Can be hard to notice on Edge/Chrome but it's there as well<br />
		It also seems most pronounced in firefox 😭.
	</p>
	<button
		on:click={() => {
			location.reload();
		}}>Reload</button
	>
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
		animation: intro 0.3s;
	}

	@keyframes intro {
		from {
			transform: translateY(-50px);
		}
	}
</style>
