<script>
  import { getContext } from "svelte"

  export let colourValue = 'ff00ff'


  const { styleable } = getContext("sdk")
  const component = getContext("component")
</script>

<div use:styleable={$component.styles}>
  {colourValue}
  <div style="background-color: #{colourValue}; width:200px; height:200px;">
  </div>
</div>
