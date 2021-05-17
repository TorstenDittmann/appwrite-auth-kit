<script lang="ts">
import InputButton from "$lib/inputButton.svelte";

import InputPassword from "$lib/inputPassword.svelte";
import Separator from "$lib/separator.svelte";
</script>

<h1>Verify</h1>

<InputPassword key="password" label="Password" />
<InputPassword key="password-again" label="Repeat Password" />
<InputButton>Save</InputButton>