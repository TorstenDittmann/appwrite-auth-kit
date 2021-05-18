<script lang="ts">
	import InputButton from "$lib/inputButton.svelte";
	import InputEmail from "$lib/inputEmail.svelte";
	import InputPassword from "$lib/inputPassword.svelte";
	import Paragraph from "$lib/paragraph.svelte";
</script>

<Paragraph>Already have an account? <a href="/login">Click here to login</a></Paragraph>
<InputEmail key="name" label="Name" />
<InputEmail key="email" label="E-Mail" />
<InputPassword key="password" label="Password" />
<InputButton>Register</InputButton>
