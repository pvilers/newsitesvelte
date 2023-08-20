<script>
  export let article;
</script>

<div class="article">
  <h2>{article.titre}</h2>
  <img src={article.image} alt={article.titre} />
  <p>{article.texte}</p>
</div>

<style>
  .article {
    margin: 5rem;
  }
  img {
    width: 100%;
    margin: 1rem auto;
  }
</style>
