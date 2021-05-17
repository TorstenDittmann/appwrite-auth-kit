<main>
	<slot />
</main>

<style lang="scss">
	main {
		display: flex;
        flex-direction: column;
		grid-area: content;
		align-items: center;
		justify-content: center;
        padding: 2rem;
	}
</style>
