<script>
 let count = $state(0);
 let double = $derived(count*2);

 function increment (){
    count +=1;
 }

 $effect(()=>{
    console.log('The effect has run .Current Count is :', count)
 })

 $inspect(count) 
// $inspect will update when the count update , its basically working as a inspect on the browser
</script>

<main>
    <h1>{double}</h1>
    <button onclick={increment}>Increment</button>
</main>