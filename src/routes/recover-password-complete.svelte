<script lang="ts">
	import InputButton from "$lib/inputButton.svelte";
	import InputPassword from "$lib/inputPassword.svelte";
</script>

<h1>Password Recovery</h1>

<InputPassword key="password" label="Password" />
<InputPassword key="password-again" label="Repeat Password" />
<InputButton>Save</InputButton>
