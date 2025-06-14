<script>
 let count = $state(0);
 let double = $derived(count*2);

 function increment (){
    count +=1;
 }

 $effect(()=>{
    console.log('The effect has run .Current Count is :', count)
 })
</script>

<main>
    <h1>{double}</h1>
    <button onclick={increment}>Increment</button>
</main>