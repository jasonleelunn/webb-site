<script lang="ts">
	import Tile from './Tile.svelte';

	interface ImageInfo {
		src: string;
		alt: string;
	}

	const images: ImageInfo[] = [
		{ src: 'astronaut-on-earth.svg', alt: 'spaceman' },
		{ src: 'space-shuttle-launch.svg', alt: 'rocket' },
		{ src: 'astronaut-on-earth.svg', alt: 'spaceman' },
		{ src: 'space-shuttle-launch.svg', alt: 'rocket' },
		{ src: 'astronaut-on-earth.svg', alt: 'spaceman' },
		{ src: 'space-shuttle-launch.svg', alt: 'rocket' },
	];
</script>

<div class="flex flex-wrap justify-center bg-slate-500 m-3 rounded-md">
	{#each images as image}
		<Tile src="images/{image.src}" alt={image.alt} />
	{/each}
</div>
