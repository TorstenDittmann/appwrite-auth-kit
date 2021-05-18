<script lang="ts">
	import InputLabel from "./inputLabel.svelte";
	export let key: string, label: string, value: string;
</script>

<InputLabel {key} {label}>
	<input id={key} type="email" bind:value />
</InputLabel>

<style lang="scss">
	input {
		color: rgb(51, 51, 51);
		font-size: 1rem;
		line-height: 1.4;
		background-color: white;
		font-family: "Poppins", sans-serif;
		border: 1px solid rgb(221, 221, 221);
		border-radius: 4px;
		display: block;
		font-weight: 400;
		padding: 1rem;
		width: 100%;
		appearance: none;
		box-sizing: border-box;
	}
</style>
