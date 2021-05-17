<script lang="ts">
	import InputLabel from './inputLabel.svelte';

	export let icon: boolean = true;
	export let iconColor: string = '';
	export let iconBackground: string = '';
	export let type: 'primary' | 'secondary' = 'primary';
</script>

<InputLabel text={false}>
	<button class:icon class={type}>
		{#if icon}
			<span class="icon" style={`background-color: ${iconBackground}; color: ${iconColor}`}>
				<slot name="icon" />
			</span>
		{/if}
		<span class="text">
			<slot />
		</span>
	</button>
</InputLabel>

<style lang="scss">
	button {
		position: relative;
		font-size: 1rem;
		border: 0px;
		border-radius: 4px;
		cursor: pointer;
		font-weight: 600;
		line-height: 1.3;
		text-decoration: none;
		text-align: center;
		padding: calc(11px - 0.1ex) 28px calc(11px + 0.1ex);
		width: 100%;
		height: 2.6rem;
		background: rgb(17, 17, 17);
		color: white;
        transition: filter .1s;

        &:hover {
            filter: brightness(80%);
        }

		&.primary {
			background: rgb(17, 17, 17);
			color: white;
		}

		&.secondary {
			background: rgb(238 238 238);
			color: black;
		}

		&.icon {
			padding: calc(11px - 0.1ex) 10px calc(11px + 0.1ex) calc(2.6rem + 10px);
			min-width: 17rem;
		}

		span.icon {
			left: 0px;
			position: absolute;
			box-sizing: border-box;
			top: 0px;
			left: 0px;
			width: 2.6rem;
			height: 100%;
            border-top-left-radius: 4px;
            border-bottom-left-radius: 4px;

            :global(svg) {
                width: 1.3rem;
                height: 2.6rem;
            }
		}
	}
</style>
