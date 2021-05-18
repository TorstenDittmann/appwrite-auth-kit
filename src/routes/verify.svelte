<script lang="ts">
	import Paragraph from "$lib/paragraph.svelte";
	import { CheckCircleIcon } from "svelte-feather-icons";
</script>

<h1><CheckCircleIcon inline={true} size="1.5x" /><span>Account Verified</span></h1>
<Paragraph><a href="/">Back to your app.</a></Paragraph>

<style lang="scss">
	h1 {
		display: flex;
		align-items: center;
		justify-content: center;
		line-height: 3rem;

		span {
			margin-left: 1rem;
		}
	}
</style>
