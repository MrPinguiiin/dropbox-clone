<script lang="ts">
	import Logo from './Logo.svelte';
	import * as Avatar from '$lib/components/ui/avatar';
	import { Button } from '$lib/components/ui/button';
</script>

<header class="sticky left-0 top-0 flex items-center justify-between bg-background">
	<!-- logo -->
	<Logo />
	<!-- avatar -->
	<div class="flex items-center gap-5">
		<Avatar.Root>
			<Avatar.Image src="https://github.com/shadcn.png" alt="@shadcn" />
			<Avatar.Fallback>CN</Avatar.Fallback>
		</Avatar.Root>
		<Button variant="outline">Sign Out</Button>
	</div>
	<!-- logout -->
</header>
