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

<svelte:head>
  <meta name="description" content="Routes for Svelte">
  <meta property="og:description" content="Routes for Svelte">

  <meta name="url" content="link">
  <meta property="og:url" content="https://www.imdb.com/title/tt0117500/" />

  <meta name="image" content="rock">
  <meta property="og:image" content="https://hedwig-cf.netmarble.com/forum-common/sknightsmmo/sk2/thumbnail/e5ad35cac65842d0a9c1d87ac0068854_1609927010739_d.jpg" />

  <title>Routify</title>
  <meta name="title" content="Routes for Svelte">
  <meta property="og:title" content="Routes for Svelte">
</svelte:head>