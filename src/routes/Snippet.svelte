<script>
 let formState = $state({
        name :'',
        birthday :'',
        step:0,
        error:'',
    })
</script>

<main>
 {#snippet formStep()}

 {/snippet}
</main>