<script>
  let numeroTb;
  let labelText = "";

  const numeroValue = () => {
    const numeroValue = numeroTb.value;
    labelText = `Número da TB: ${numeroValue}`;
  };
</script>

<input type="text" bind:this={numeroTb} name="numero" id="numero" />
<button on:click={numeroValue}>Pesquisar</button>
<label>{labelText}</label>
