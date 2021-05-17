<script lang="ts">
	import Content from '$lib/content.svelte';

	import Cover from '$lib/cover.svelte';
</script>

<section class="content">
	<Cover />
	<Content>
		<slot />
	</Content>
</section>

<style lang="scss">
	:global(body) {
		height: 100%;
		font-family: 'Poppins', sans-serif;
	}
	section.content {
		display: grid;
		grid-template-columns: 1fr 1fr;
		grid-template-rows: 1fr;
		gap: 0px 0px;
		grid-template-areas: 'cover content';
		height: 100vh;
		width: 100vw;
	}
</style>
