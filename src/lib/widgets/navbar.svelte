<script lang="ts">
	import { resolve } from '$app/paths';
</script>

<div class="m-2 overflow-hidden rounded-full">
	<div class="navbar bg-base-200">
		<div class="ml-4 flex-1 font-black text-base-content">
			<a href={resolve('/')}>CodingKitten</a>
		</div>
		<div class="flex-none">
			<ul class="menu menu-horizontal px-1">
				<li><a href={resolve('/')}>Link</a></li>
				<li>
					<details>
						<summary>Parent</summary>
						<ul class="rounded-t-none bg-base-100 p-2">
							<li><a href={resolve('/')}>Link 1</a></li>
							<li><a href={resolve('/')}>Link 2</a></li>
						</ul>
					</details>
				</li>
			</ul>
		</div>
	</div>
</div>
