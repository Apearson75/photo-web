<script>
	import Nav from '$lib/Nav.svelte';
	import Card from '$lib/Card.svelte';
	var imageList = {
		images: [
			{
				image:'https://cdn.discordapp.com/avatars/813128377967575061/d4e8a52c2861eb342570ea1c4de40960.png?size=4096',
				title: 'Blender Render'
			},
			{
				image:'https://cdn.discordapp.com/attachments/853331978538844210/987654225381167124/20220613_164345.jpg',
				title: 'Sunflower'
			},
			{
				image:'https://cdn.discordapp.com/attachments/853331978538844210/987661195471384587/20220611_123928.jpg',
				title: 'Random Plant'
			}
		]
	};
</script>

<div class="">
	<Nav />
	<div class="sm:grid sm:grid-cols-3 sm:space-y-0 sm:gap-6 lg:flex lg:flex-wrap lg:flex-l lg:px-80 lg:py-10 lg:mx-40 rounded-lg">
		<div class="h-56 px-2">
			{#each imageList['images'] as image}
				<!-- svelte-ignore a11y-img-redundant-alt -->
				<Card image={image['image']} title={image['title']} />
			{/each}
		</div>
	</div>
</div>
