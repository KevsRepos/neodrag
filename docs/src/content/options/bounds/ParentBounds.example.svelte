<script lang="ts">
	import OptionsDemoBase from '$components/options/OptionsDemoBase.svelte';
</script>

<div>
	<OptionsDemoBase options={{ bounds: 'parent' }} renderParent={true}>
		Can't go outside the parent element
	</OptionsDemoBase>
</div>

<style lang="scss">
	div :global(.parent) {
		display: grid;
		place-content: center;

		width: 90%;
		height: 70%;

		border: var(--app-color-dark) solid 2px;
	}
</style>
