<script>
    // declare our props
    // the 'export' allows the props to be accessed outside of the component
    export let firstName;
    export let lastName;
</script>
<!-- Inputs for each name, reactively binding the value each input to each prop -->
<label for="firstName">First Name</label><input name="firstName" bind:value={firstName}>
<label for="lastName">Last Name</label><input name="lastName" bind:value={lastName}>

<!-- Outputting the prop in our h2 -->
<h2>This is the app for {firstName} {lastName}</h2>

<style>
    /* This style is scoped to just this component */
    h2 {
		color: red;
	}
</style>