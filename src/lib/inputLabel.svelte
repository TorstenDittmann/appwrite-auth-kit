<script lang="ts">
	export let key: string;
	export let label: string;
	export let text: boolean = true;
</script>

<label for={key} class:no-text={!text}>
	{#if text}<span>{label}</span>{/if}
	<slot />
</label>

<style lang="scss">
	label {
		max-width: 20rem;
		display: flex;
		flex-direction: column;
		justify-content: center;
		margin: 1.4rem auto;
		width: 100%;

		&.no-text {
			margin: 0.4rem auto;
		}

		span {
			font-size: 0.875rem;
			font-weight: 400;
			margin-bottom: 0.6ex;
		}
	}
</style>
