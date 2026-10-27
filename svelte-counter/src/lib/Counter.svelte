<script>
  let isOn = $state(false)
  let {onToggle} = $props()

  function toggle(){
    isOn = !isOn
    onToggle(isOn)
  }
</script>

<button type="button" class:active={isOn} onclick={toggle}>
{isOn ? 'ON': 'OFF'}
</button>




<style>
  button.active {
    background: black;
    color: white;
  }

  button {
    width: 100px;
    height: 100px;
    box-sizing: border-box;
    border: 1px solid gray;
    border-radius: 0;
    background: white;
    color: black;
  }
</style>