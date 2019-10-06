<script>
  import Image from "../components/Image/Image.svelte";

  let colors = {
    light: "#f9f7f7",
    gray: "#dbe2ef",
    blue: "#3f72af",
    navy: "#112d4e"
  };
</script>

<style>
  :root {
    --font-color: "#112d4e";
  }
  h1,
  figure {
    text-align: center;
    margin: 0 auto;
  }

  h1 {
    font-size: 2.5em;
    font-weight: 600;
    color: #112d4e;
    margin: 24px 0 0 0;
  }

  @media (min-width: 480px) {
    /* h1 {
      font-size: 4em;
    } */
  }

  #header {
    text-align: center;
    display: flex;
    color: #112d4e;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }

  .separator {
    width: 100%;
    height: 25px;
    padding: 24px 0 24px 0;
    margin: 0;
    text-align: center;
    font-size: 28px;
    letter-spacing: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  #bio {
    height: 300px;
    border: 1px solid rebeccapurple;
  }
</style>

<svelte:head>
  <title>Alejandro Roman - Software Engineer</title>
</svelte:head>
<section id="header" aria-label="Alejandro Roman">
  <figure>
    <Image bind:colors />
  </figure>
  <h1 style="--theme-color: {colors.navy}">Alejandro Roman</h1>
  <p class="separator" aria-hidden="true">{`.   .   .`}</p>
</section>
<section id="bio">Yo</section>
