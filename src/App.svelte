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
