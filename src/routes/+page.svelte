<script>
	import {
		MainHero,
		MainAbout,
		MainStats,
		MainSponsor,
		MainStory,
		Carrousel
	} from '$lib/index.js';
	export let data;
</script>

<svelte:head><title>INK - Legends</title></svelte:head>

<MainHero />
<MainAbout {data} />
<MainStats {data} />
<MainSponsor {data} />
<MainStory {data} />
<Carrousel />


