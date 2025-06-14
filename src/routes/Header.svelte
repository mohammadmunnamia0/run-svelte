<script lang="ts">
let {name} : {name:string} = $props();
</script>

<h1>
    Hello From {name} <br>  <!-- Hello From Munna -->

    <!-- Simple Javascript boolean Check the output for the result -->
    Hello From {name == 'X'} <br> <!-- Hello From false  -->
    Hello From {name == 'Munna'} <!-- Hello From true -->
</h1>

<h2>
    <!-- We can use javascript here without any hesitation -->
     {name.replace('M', 'm')} <br> <!--change Munna in to munna  -->
     {name.replaceAll('n', 'm')}  <!--change Munna in to Mumma  -->
</h2>