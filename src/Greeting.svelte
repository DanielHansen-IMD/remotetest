<script>
    let firstName;
    let lastName;
</script>

<label for="firstName">First Name</label><input name="firstName" bind:value={firstName}>

<label for="lastName">Last Name</label><input name="lastName" bind:value={lastName}>

<h2>This is the app for {firstName} {lastName}</h2>

<style>
    h2 {
		color: red;
	}
</style>