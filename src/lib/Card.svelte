<script>
    export let image;
    export let title;
</script>

<div class= "rounded-lg shadow-lg bg-orange-200 my-2 p-3">	
    <!-- svelte-ignore a11y-img-redundant-alt -->
    <img src={image} alt="An Image" class="object-cover my-2 rounded-md" />
    <p class="font-semibold text-end -py-2 h-7 text-lg px-2">{title}</p>
</div>