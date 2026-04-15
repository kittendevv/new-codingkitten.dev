<script lang="ts">
	import HandHeartIcon from 'phosphor-svelte/lib/HandHeartIcon';

	let containerWidth = $state(0);
</script>

<div class="col-span-1 row-span-1 aspect-square rounded-2xl bg-base-200">
	<a href="https://ko-fi.com/codingkitten" target="_blank" rel="noopener noreferrer external" class="h-full w-full">
		<div class="flex h-full items-center justify-center text-base-content" bind:clientWidth={containerWidth}>
			<HandHeartIcon size={containerWidth / 4} weight="fill" />
		</div>
	</a>
</div>
