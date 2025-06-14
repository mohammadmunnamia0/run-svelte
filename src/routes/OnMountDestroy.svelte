<script>
	import { onDestroy, onMount } from "svelte";
    import {languages} from "./Data.js"
    
    let show=false;
    
    let languageList =[];

    onMount (()=>{
        console.log("Mounted");
        languageList = languages;
    });
    
    onDestroy (()=>{
        console.log("Destroyed");
    });
    
</script>

<style>
    p {
        border : 2px solid red;
        padding: 4px;
    }
</style>

<main>
    
    {#if show}
    <p>Im Toggled</p>

     <ul>
        {#each languageList as language}
        <li>{language}</li>
        {/each}
    </ul>
    {/if}

   

    <button onclick={() =>{show = !show}}>Toggle</button>
</main>