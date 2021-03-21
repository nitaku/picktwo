<script lang="ts" context="module">
  export const width = 220
  export const height = 300
</script>

<script lang="ts">
  import * as cartocolor from 'cartocolor'

  export let title = 'Title'
  export let category = 'Category'
  export let text = 'Text'
  export let type = 'Check'
  export let color = 3

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
    fill={cartocolor.Bold[7][color]}
    fill-opacity="0.4"
    stroke={cartocolor.Bold[7][color]}
    stroke-width="6"
  />
  <text class="title" y={-height/2} dy="1.5em">{title}</text>
  <text class="category" dy=".35em">{category}</text>
  <text class="text" x={-width/2+22} y="38">{text}</text>
  <text class="type" y={height/2} dy="-1em">{type}</text>
</g>

<style>
  .title {
    font-size: 22px;
    font-weight: bold;
    text-anchor: middle;
  }
  .category {
    font-size: 18px;
    font-weight: bold;
    text-anchor: middle;
  }
  .text {
    font-size: 16px;
    text-anchor: left;
  }
  .type {
    font-size: 18px;
    font-weight: bold;
    text-anchor: middle;
  }
</style>