<script>
    import { onMount } from 'svelte';
    import { page } from '$app/stores'

    let posts = []
    onMount( async () => {
        const response = await fetch('https://jsonplaceholder.typicode.com/posts') 
        posts = await response.json()
        console.log(posts)
    })

        const apiId = $page.params.apiId

</script>

<h1>Page # {apiId}</h1>

{#each posts as post(post.id)}
<h1>{post.id}. {post.title}</h1>
<p>{post.body}</p>
<hr>
{:else}
<p>Loading...</p>
{/each}








