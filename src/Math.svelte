<script>
    // declare our props
    let num1;
    let num2;
    // letting the 'result' prop be accessed outside of the component with the 'export' prefix
    export let result;

    // reactively updating the result prop using the '$:' prefix
    $: result = num1 * num2;
</script>

<h2>Math!</h2>

<!-- binding the input values to the props, then outputting the result prop -->
<input bind:value={num1}> x <input bind:value={num2}> = {result}

<style>
    /* This style is scoped to just this component */
    h2 {
		color: blue;
	}
</style>