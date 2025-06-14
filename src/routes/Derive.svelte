<script>
    let name = $state('Munna');

    let full_name = $derived(name + ' ' + 'Mia')
</script>

<h2>
   {full_name}
   <!-- Whats actually happens here the full name is derived his first part from the name that why we write it using derived-->
</h2>
<input type="text" bind:value={name}>