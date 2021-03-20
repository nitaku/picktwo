<script lang="ts" context="module">
  export const width = 200
  export const height = 300
</script>

<script lang="ts">
	export let transform : string
</script>

<g transform={transform}>
  <rect
    {width}
    {height}
    x={-width/2}
    y={-height/2}
    rx="20"
    ry="20"
    fill="whitesmoke"
    stroke="black"
    stroke-width="10"
  />
</g>

<style>
</style>