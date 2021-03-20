<script lang="ts">
    import Card, {width} from './Card.svelte'

	export let cards : Array<any>
    export let separation = 30
    export let transform : string
</script>

<g transform="translate({-(cards.length-1)*(width+separation)/2},0) {transform}">
{#each cards as card, i}
  <Card transform="translate({i*(separation+width)},0)"/>
{/each}
</g>

<style>
</style>