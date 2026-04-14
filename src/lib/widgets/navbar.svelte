<script lang="ts">
    import { resolve } from '$app/paths';
</script>

<div class="rounded-full overflow-hidden m-2">
    <div class="navbar bg-base-200">
    <div class="flex-1 text-base-content font-black ml-4">
        <a href={resolve('/')}>CodingKitten</a>
    </div>
    <div class="flex-none">
        <ul class="menu menu-horizontal px-1">
        <li><a href={resolve('/')}>Link</a></li>
        <li>
            <details>
            <summary>Parent</summary>
            <ul class="bg-base-100 rounded-t-none p-2">
                <li><a href={resolve('/')}>Link 1</a></li>
                <li><a href={resolve('/')}>Link 2</a></li>
            </ul>
            </details>
        </li>
        </ul>
    </div>
    </div>
</div>