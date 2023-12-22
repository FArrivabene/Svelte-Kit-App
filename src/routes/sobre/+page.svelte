<script>
  import NovoClick from "../clicaAqui/CliqueAqui.svelte";
  import Title from "../title/Title2.svelte";

  const products = [
    { title: "bicicleta", preco: 1200, stock: 5 },
    { title: "bolas", preco: 25, stock: 33 },
    { title: "capacete", preco: 35, stock: 12 },
    { title: "sapato", preco: 55, stock: 13 },
    { title: "camiseta", preco: 45, stock: 26 },
    { title: "bicicleta", preco: 1500, stock: 8 },
  ];

  let textTB = "";
  let bikeProducts = [];

  const numeroValue = () => {
    const searchTerm =
      textTB && typeof textTB === "string" ? textTB.trim().toLowerCase() : "";
    bikeProducts = products.filter((product) =>
      product.title.toLowerCase().includes(searchTerm)
    );

    if (!bikeProducts.length) {
      alert("Nenhum resultado encontrado.");
    }
  };
</script>

<h1>Sobre</h1>

<input type="text" bind:this={textTB} name="numero" id="numero" />
<button on:click={numeroValue}>Pesquisar</button>

<table>
  <thead>
    <tr>
      <th>Título</th>
      <th>Preço</th>
      <th>Estoque</th>
    </tr>
  </thead>
  <tbody>
    {#each bikeProducts as product}
      <tr>
        <td>{product.title}</td>
        <td>R$ {product.preco}</td>
        <td>{product.stock} unidades</td>
      </tr>
    {/each}
  </tbody>
</table>

<!--
{#each bikeProducts as product (product.title)}
  <li>{product.title}</li>
  <p>Preço: R$ {product.preco}, Estoque: {product.stock} unidades</p>
{/each}
{#if bikeTitle.length >= 5}
  <Title title2={bikeTitle} />
{/if}
<NovoClick />
-->
