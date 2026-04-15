<script lang="ts">
	import { resolve } from '$app/paths';

	import CaretLeftIcon from 'phosphor-svelte/lib/CaretLeftIcon';
	let { pagetitle, destination } = $props();
</script>

<div class="m-2 rounded-2xl bg-base-200 py-2">
	<div class="flex h-full flex-row items-center p-4">
		<a href={resolve(destination)} class="flex flex-1 flex-row items-center gap-2 font-[Space_Grotesk_Variable] text-2xl font-bold">
			<CaretLeftIcon weight="fill" />
			Back
		</a>
		<h1 class="flex-1 text-end font-[Space_Grotesk_Variable] text-2xl text-base-content">
			{pagetitle}
		</h1>
	</div>
</div>
