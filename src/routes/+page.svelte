<script>
  import { player1 } from "/src/lib/data.js";
</script>

<main>
  <section>
    {#each player1 as player} <article class="card">
<img src="/{player.images}" alt="player images">
<a href={player.url} target="_blank">

 <h1>{player.title}</h1>
 <p>{player.biography}</p>
 </a>
      </article>
    {/each}
  </section>
</main>




<style>
  section {
    padding: auto;
    display: flex;
    justify-content: center;
    gap: 2rem;
  }
  article {
    padding: 5rem;
    border: 3px solid rgb(214, 20, 20);
    border-radius: 2rem;
    background-color: rgb(214, 185, 56);


    
  }
  article:hover {
    background-color: rgb(240, 236, 236);
  
  }

  main {
  max-width: 85ch;
  margin: auto;
}
</style>