<script lang="ts">
	import Hand from './Hand.svelte'

	let cards = [{
		title: '10,000 Steps',
		category: 'Fitness',
		color: 4,
		text: ''
	},{
		title: 'Chapter',
		category: 'Reading',
		color: 0,
		text: 'Read a chapter of a novel.'
	},{
		title: 'Veggie Dinner',
		category: 'Cooking',
		color: 3,
		text: 'Cook a vegetable meal.'
	},{
		title: 'Count the Breath',
		category: 'Meditation',
		color: 1,
		text: ''
	},{
		title: 'Bugfix',
		category: 'Productivity',
		color: 2,
		text: 'Fix a bug in one project.'
	}]
</script>

<svg class="main" viewBox="-800 0 1600 900">
  <Hand {cards} transform="translate(0,740)"/>
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
	}
</style>