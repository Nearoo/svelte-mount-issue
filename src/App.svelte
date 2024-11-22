<script lang="ts">
  import { mount, onMount } from "svelte";
  import MyComponent from "./MyComponent.svelte";
  let div: HTMLDivElement

  onMount(() => {
    const mounted: MyComponent = mount(MyComponent, { target: div })
  })
</script>



<div bind:this={div}></div>