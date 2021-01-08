<script>
  import { Router } from "@roxi/routify";
  import { routes } from "../.routify/routes";
  import { metatags } from '@roxi/routify'
        metatags.description = 'Routes for Svelte'
        metatags.title = 'Routify'
        metatags.image = "rock"
        metatags.url = "link"
        
</script>

<style  global>
  @import "../assets/global.css";
</style>

<Router {routes} />

<head>
  <meta name="description" content="Routes for Svelte">
  <meta property="og:description" content="Routes for Svelte">
  <meta property="og:url" content="https://www.imdb.com/title/tt0117500/" />
  <meta property="og:image" content="https://ia.media-imdb.com/images/rock.jpg" />
  <title>Routify</title>
    <meta name="title" content="Routes for Svelte">
    <meta property="og:title" content="Routes for Svelte">
</head>