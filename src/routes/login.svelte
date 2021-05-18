<script lang="ts">
	import { GithubIcon, TwitterIcon, FacebookIcon } from "svelte-feather-icons";

	import InputButton from "$lib/inputButton.svelte";
	import InputEmail from "$lib/inputEmail.svelte";
	import InputPassword from "$lib/inputPassword.svelte";
	import Separator from "$lib/separator.svelte";
	import Hint from "$lib/hint.svelte";
	import Paragraph from "$lib/paragraph.svelte";
</script>

<InputButton type="secondary" icon={true} iconBackground="#FAFAFA" iconColor="#333333">
	<GithubIcon slot="icon" />
	Login with GitHub
</InputButton>
<InputButton type="secondary" icon={true} iconBackground="#3B5998" iconColor="#FFFFFF">
	<FacebookIcon slot="icon" />
	Login with Facebook
</InputButton>
<InputButton type="secondary" icon={true} iconBackground="#1DA1F2" iconColor="#FFFFFF">
	<TwitterIcon slot="icon" />
	Login with Twitter
</InputButton>

<Separator />
<Paragraph>Don't have an account yet? <a href="/register">Click here to register</a></Paragraph>
<InputEmail key="email" label="E-Mail" />
<InputPassword key="password" label="Password" />
<InputButton>Login</InputButton>
<Hint><a href="/recover-password">Forgot your password</a></Hint>
