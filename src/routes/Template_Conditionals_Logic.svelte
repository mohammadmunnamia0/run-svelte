<script>
    let formState = $state({
        name :'',
        birthday :'',
        step:0,
        error:'',
    })
</script>

<main>
    <p>Step:{formState.step}</p>

   

    {#if formState.step === 0}

        <div>
            <label for="name">Your name</label>
            <input type="text" id="name" bind:value={formState.name}>
        </div>

        <button onclick={() =>{
        if(formState.name !== ''){
            formState.step +=1;
            formState.error ='';
        }
          else{
                formState.error = 'Your Field is Empty.'
            }
        }}>Next</button>

    {:else if formState.step === 1}    
        <div>
                <label for="birthday">Your birthday</label>
                <input type="date" id="birthday" bind:value={formState.birthday}>
            </div>

            <button onclick={() =>{
            if(formState.birthday !== ''){
                formState.step +=1;
                formState.error ='';
            }
            else{
                formState.error = 'Your Field is Empty.'
            }
            }}>Next</button>
    {/if}

     {#if formState.error}

      <p>{formState.error}</p>

    {/if}

    
</main>