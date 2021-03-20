<script lang="ts">
	import Hand from './Hand.svelte'
</script>

<svg class="main" viewBox="-800 0 1600 900">
  <Hand cards={[1,2,3,4,5]} transform="translate(0,740)"/>
</svg>

<style>
	:global(html, body) {
		padding: 0;
		margin: 0;
		width: 100%;
		height: 100%;
		overflow: hidden;
	}
	.main {
		width: 100%;
		height: 100%;
		background: gray;
	}
</style>