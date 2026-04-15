<script lang="ts">
	import Navcard from '$lib/widgets/navcard.svelte';
    import Controlcards from '$lib/widgets/controlcards.svelte';
</script>

<div class="min-h-screen">
	<div class="h-full min-h-screen w-full">

		<div class="grid grid-cols-5 gap-2 m-2">
			<Navcard title="Blog" cols="col-span-2" />
			<Navcard title="Coding Projects" cols="col-span-3" />
			<Navcard title="Other Projects" cols="col-span-3" />
			<Navcard title="About me" cols="col-span-2" />
            
            <Controlcards />
		</div>
	</div>
</div>
