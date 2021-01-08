<script>
  import { Router } from "@roxi/routify";
  import { routes } from "../.routify/routes";
  import Meta from './Meta.svelte'
	
	const metadata = {
		title: 'Svelte is Awesome',
		description: 'It really is!',
		image: 'https://svelte.dev/images/twitter-card.png',
		imageAlt: 'Svelte svelte.dev',
		url:'svelte.dev'
	}
</script>

<style  global>
  @import "../assets/global.css";
</style>

<Router {routes} />
<Meta {metadata}/>