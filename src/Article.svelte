<script>
  export let article;
</script>

<div class="article">
  <h2>{article.titre}</h2>
  <img src={article.image} alt={article.titre} width="341" height="237"/>
  <p>{article.texte}</p>
</div>

<style>
  .article {
    margin: 5rem 0;
  }
  img {
    width: 100%;
    height: auto;
    margin: 2rem auto;
    aspect-ratio: 16 / 10;
    object-fit: cover;
  }
</style>
