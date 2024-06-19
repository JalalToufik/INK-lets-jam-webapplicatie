<script>
	import {
		MainHero,
		MainAbout,
		PlayerCarrousel,
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
<PlayerCarrousel />
<MainStats {data} />
<MainSponsor {data} />
<MainStory {data} />
<Carrousel />


