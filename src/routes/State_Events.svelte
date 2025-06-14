<script lang='ts'>

let status: 'OPEN' | 'CLOSED' = $state('OPEN') //Like the UseState in js

function toggle() {
    status = status === 'OPEN' ? 'CLOSED' : 'OPEN';
    // if status Open then on Toggle Show Closed otherwise Open
}
function onclick() {
    status = status === 'OPEN' ? 'CLOSED' : 'OPEN';
    // if status Open then on Toggle Show Closed otherwise Open
}

</script>

<h1>The Store is {status}</h1>

<!-- Now lets change the status value using "onclick" -->

<button onclick={toggle}>Toggle Status</button>

<button {onclick}>Toggle Status</button>

<!-- Using Arrow Function -->
 <button onclick={()=>{
 status = status === 'OPEN' ? 'CLOSED' : 'OPEN';
 }}>Toggle Status</button>