<script>
    import RoutifyIntro from './example/_components/RoutifyIntro.svelte';
    import { metatags } from '@roxi/routify';
    import { onMount } from 'svelte';

    const fetchTitle = (async()=> {
        const response = await fetch("https://us-central1-allius.cloudfunctions.net/getUserBasicInfo?nickname=david");
        let testData = await response.json();
        await console.log(testData.name);
        return await testData.name;
    })();


    onMount(() => {
        metatags.title = fetchTitle();
    })

</script>

<RoutifyIntro />
