<script>
	import Nav from '$lib/Nav.svelte';
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
	<div class="sm:grid sm:grid-cols-3 sm:space-y-0 sm:gap-6 rounded-lg">
		<div class="h-56 px-2">
			{#each imageList['images'] as image}
				<!-- svelte-ignore a11y-img-redundant-alt -->
				<div class= " rounded-lg shadow-lg bg-orange-200">	
					<img src={image['image']} alt="An Image" class="object-cover my-2" />
					<p class=" font-semibold text-end -py-2 h-8 text-lg px-2">{image['title']}</p>
				</div>	
			{/each}
		</div>
	</div>
</div>
