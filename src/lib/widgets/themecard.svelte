<script lang="ts">
	import { onMount } from 'svelte';
	import { applyTheme, getTheme } from '$lib/theme';

	import MoonIcon from 'phosphor-svelte/lib/MoonIcon';
	import SunIcon from 'phosphor-svelte/lib/SunIcon';

	let isDark = $state(true);

	onMount(() => {
		const saved = getTheme();
		isDark = saved;
		applyTheme(saved);
	});

	function flipTheme() {
		isDark = !isDark;
		applyTheme(isDark);
	}
</script>

<div class="col-span-1 row-span-1 aspect-square rounded-2xl bg-base-200">
	<button class="h-full w-full cursor-pointer" onclick={flipTheme}>
		<div class="flex h-full items-center justify-center text-base-content">
			{#if isDark}
				<MoonIcon size="64" weight="fill" />
			{:else}
				<SunIcon size="64" weight="fill" />
			{/if}
		</div>
	</button>
</div>
