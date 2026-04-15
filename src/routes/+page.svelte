<script lang="ts">
	import Navcard from '$lib/widgets/navcard.svelte';
	import Themecard from '$lib/widgets/themecard.svelte';
	import Githubcard from '$lib/widgets/githubcard.svelte';
</script>

<div class="min-h-screen">
	<div class="h-full min-h-screen w-full">
		<div class="m-2 grid grid-cols-5 grid-rows-3 gap-2">
			<Navcard title="Blog" cols="col-span-2" />
			<Navcard title="Coding Projects" cols="col-span-3" />
			<Navcard title="Other Projects" cols="col-span-3" />
			<Navcard title="About me" cols="col-span-2" />

			<Themecard />
			<Githubcard />
		</div>
	</div>
</div>
