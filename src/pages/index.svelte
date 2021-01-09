<script>
    import { ready } from '@roxi/routify';
		import { onMount } from 'svelte';

		let data = {};

    const getData = async() => {
        const res = await fetch("https://us-central1-allius.cloudfunctions.net/getUserBasicInfo?nickname=david");
        let loo = await res.json()
				data = loo;
        $ready()
		}
		
		onMount(() => {
			getData();
	});
</script>


<h1>hello</h1>

<svelte:head>
    <title>{data.title}</title>
    <meta property="og:title" content={data.name}/>
    <meta property="og:image" content={data.photo_url}/>
    <meta property="og:description" content={data.note}/>
</svelte:head>

