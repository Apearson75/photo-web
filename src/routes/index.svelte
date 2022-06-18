<script>
	import Nav from "$lib/Nav.svelte";
	var imageList = [
		"https://cdn.discordapp.com/avatars/813128377967575061/d4e8a52c2861eb342570ea1c4de40960.png?size=4096",
		"https://cdn.discordapp.com/attachments/853331978538844210/987654225381167124/20220613_164345.jpg",
		"https://cdn.discordapp.com/attachments/853331978538844210/987661195471384587/20220611_123928.jpg",
	];
</script>

<div class="">
	<Nav/>
	<div class="sm:grid sm:grid-cols-3 sm:space-y-0 sm:gap-6">
		<div class="h-56 px-2">
			{#each imageList as image}
			<!-- svelte-ignore a11y-img-redundant-alt -->
			<img src={image} alt="An Image" class="rounded-lg shadow-lg object-cover my-2"/>
			{/each}
	  	</div>
	</div>
</div>