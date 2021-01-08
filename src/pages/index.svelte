<script>
import RoutifyIntro from './example/_components/RoutifyIntro.svelte';
import { metatags } from '@roxi/routify';
import { onMount } from 'svelte';

    // const fetchTitle = (async()=> {
    //     const response = await fetch("https://us-central1-allius.cloudfunctions.net/getUserBasicInfo?nickname=david")
    //     return await response.json()
    // })();

    onMount(async() => {
        const res = await fetch("https://us-central1-allius.cloudfunctions.net/getUserBasicInfo?nickname=david");
        
    })

</script>

<RoutifyIntro />

<!-- {#await fetchTitle}
{:then data}
<h1>{data.name}</h1>
{/await} -->