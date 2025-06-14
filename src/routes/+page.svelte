<script>
	import Header from "./Header.svelte";

    // let name = 'Su';
    let name = $state('su');
</script>

<!-- pass the props `name="Munna"` from here to other component Header.svelte -->
<Header name="Munna"/>

<!-- Initialize the variable `let name = 'Su'` and use it in side the own component without passing props -->
 
<!-- <Header name={name}/> -->

<Header {name}/> 

<!-- this both will same `name={name} & {name}` , show the same result. -->


<!-- bind values = help to change the value across everywhere  --> 
Example : <input type='text' placeholder="TypeAnything" bind:value={name}>

<!-- In React if we want to change anything we had to use onchange but here simple "bind:value={props_name}" -->
