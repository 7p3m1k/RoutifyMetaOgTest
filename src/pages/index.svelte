<script>
    import { metatags, ready } from '@roxi/routify';

    let dataTest;
    let dataNote;
		let dataImg;
		let moo = {};

    const getData = async() => {
        const res = await fetch("https://us-central1-allius.cloudfunctions.net/getUserBasicInfo?nickname=david");
        let loo = await res.json()
        // dataTest = await loo.name
        // dataNote = await loo.note
				// dataImg = await loo.photo_url
				moo = loo;
        $ready()
    }
    getData();
</script>


<h1>hello</h1>

<svelte:head>
    <title>{moo.title}</title>
    <meta property="og:title" content={moo.name}/>
    <meta property="og:image" content={moo.photo_url}/>
    <meta property="og:description" content={moo.note}/>
</svelte:head>

