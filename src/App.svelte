<script>
  import { BarChartSimple } from "@carbon/charts-svelte";
</script>

<svelte:head>
  <link
    rel="stylesheet"
    href="https://unpkg.com/@carbon/charts@0.30.10/styles.min.css" />
</svelte:head>

<BarChartSimple
  data={[{ group: 'Qty', value: 65000 }, { group: 'More', value: 29123 }, { group: 'Sold', value: 35213 }, { group: 'Restocking', value: 51213 }, { group: 'Misc', value: 16932 }]}
  options={{ title: 'Simple bar (discrete)', axes: { left: { mapsTo: 'value' }, bottom: { mapsTo: 'group', scaleType: 'labels' } }, height: '400px' }} />
