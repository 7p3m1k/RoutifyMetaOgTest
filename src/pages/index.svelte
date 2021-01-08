<script>
    import { metatags, ready } from '@roxi/routify';

    let dataTest;
    let dataNote;
    let dataImg;

    const getData = async() => {
        const res = await fetch("https://us-central1-allius.cloudfunctions.net/getUserBasicInfo?nickname=david");
        const loo = await res.json()
        dataTest = await loo.name
        dataNote = await loo.note
        dataImg = await loo.photo_url
        $ready()
    }
    getData();
</script>


<h1>hello</h1>

<svelte:head>
    <title>{dataTest}</title>
    <meta property="og:title" content={dataTest}/>
    <meta property="og:image" content={dataImg}/>
    <meta property="og:description" content={dataNote}/>
</svelte:head>

