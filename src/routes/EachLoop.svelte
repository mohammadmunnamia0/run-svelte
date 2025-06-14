<script>
 let people = [
    {
        name:'munna',
        profession : 'dev',
        age:24
    },
    {
        name:'rabbi',
        profession : 'qa',
        age:42
    },
    {
        name:'abbi',
        profession : 'Devops',
        age:35
    }
 ]
</script>

<main>
    {#each people as person}
    <li>{person.name} is a {person.profession}</li>
    {/each}

    <!-- i for show the index number -->
    {#each people as person,i }
    <li>[{i}] {person.name} is a {person.profession}</li>
    {/each}
</main>