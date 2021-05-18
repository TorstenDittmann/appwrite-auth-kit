<script lang="ts">
	import Hint from "$lib/hint.svelte";
	import InputButton from "$lib/inputButton.svelte";
	import InputEmail from "$lib/inputEmail.svelte";
	import Paragraph from "$lib/Paragraph.svelte";
</script>

<h1>Password Recovery</h1>
<Paragraph
	>Enter your username or email address and we will send you a link to reset your password.</Paragraph
>

<InputEmail key="email" label="E-Mail" />
<InputButton>Forgot Password</InputButton>
<Hint><a href="/login">Back to login</a></Hint>
