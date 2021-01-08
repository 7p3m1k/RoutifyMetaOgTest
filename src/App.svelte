<script>
  import { Router } from "@roxi/routify";
  import { routes } from "../.routify/routes";
  import { metatags } from '@roxi/routify'
        metatags.description = 'Routes for Svelte'
        metatags.title = 'Routify'
        metatags.image = "https://source.unsplash.com/random"
        metatags.url = "https://routify.dev/docs/metatags"
</script>

<style  global>
  @import "../assets/global.css";
</style>

<Router {routes} />


<meta name="description" content="Routes for Svelte">
<meta property="og:description" content="Routes for Svelte">

<title>Routify</title>
<meta name="title" content="Routes for Svelte">
<meta property="og:title" content="Routes for Svelte">

<meta name="image" content="https://source.unsplash.com/random">
<meta property="og:image" content="https://source.unsplash.com/random">


<meta name="url" content="https://routify.dev/docs/metatags">
<meta property="og:url" content="https://routify.dev/docs/metatags">