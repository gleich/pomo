<script>
	let running = $state(false);
</script>

<div class="container">
	<h1 class={running ? 'running-title' : 'starting-title'}>
		<span contenteditable>25</span>:<span contenteditable>00</span>
	</h1>

	<button class="state-button"> Start </button>
</div>

<style>
	h1 {
		font-weight: 600;
	}

	.container {
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		height: 100vh;
		gap: 15px;
	}

	.running-title {
		color: var(--green-foreground);
	}

	.starting-title {
		color: grey;
	}

	.state-button {
		width: 200px;
		padding: 10px;
	}
</style>
