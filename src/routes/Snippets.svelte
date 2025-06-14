<!-- <script>
 let formState = $state({
        name :'',
        birthday :'',
        step:0,
        error:'',
    })
</script>

<main>


(@render formStep({question : "Whats Your name", id:'name, type:'text}))

</main>

    {#snippet formStep({id,question,type}:{
    id:String,
    question:String,
    type:String,
 })}
    <div>
        <label for={id}>{id}</label>
        <input {type} {id} bind:value={formState[id]}>
    </div>
 {/snippet} -->