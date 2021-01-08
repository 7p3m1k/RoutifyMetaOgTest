<script>
    import { metatags, ready } from '@roxi/routify';

    let dataTest;
    const getData = async() => {
        const res = await fetch("https://us-central1-allius.cloudfunctions.net/getUserBasicInfo?nickname=david");
        const loo = await res.json()
        dataTest = await loo.name
        $ready()
    }
    getData();
</script>


<h1>hello</h1>
<svelte:head>
    <title>{dataTest}</title>
</svelte:head>

