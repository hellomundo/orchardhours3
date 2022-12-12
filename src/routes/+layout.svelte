<script>
	
	//import '@skeletonlabs/skeleton/themes/theme-rocket.css';
	import '../theme.postcss'
	import '@skeletonlabs/skeleton/styles/all.css';
	import '../app.postcss';

	import {AppShell, AppBar} from '@skeletonlabs/skeleton'
</script>

<AppShell>
    <!-- Header -->
	<svelte:fragment slot="header">
		<!-- Insert the App Bar: -->
		<AppBar>
			<svelte:fragment slot="lead">
				<h1>Skeleton</h1>
			</svelte:fragment>
			<svelte:fragment slot="trail">
				<a class="btn btn-sm" href="https://github.com/" target="_blank" rel="noreferrer">GitHub</a>
			</svelte:fragment>
		</AppBar>
		<!-- --- -->
	</svelte:fragment>    <!-- Sidebar -->
    <!-- Page Content Slot -->
    <slot />
    <!-- Footer Slots -->
	<svelte:fragment slot="pageFooter">Page Footer</svelte:fragment>
	<svelte:fragment slot="footer">Footer</svelte:fragment>

</AppShell>


