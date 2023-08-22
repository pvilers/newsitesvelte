<script>
  export let article;
  import {lazyimage} from 'svelte-lazyimage-cache'
  const placeholder = 'https://media3.giphy.com/media/3oEjI6SIIHBdRxXI40/200.gif'
</script>

<div class="article">
  <h2>{article.titre}</h2>
  <img alt={article.titre} width="341" height="237" use:lazyimage src={placeholder} data-src={article.image} on:cacheload={()=>console.log('load from cache')} on:imgload={() => console.log("Load from internet")}/>
  <p>{article.texte}</p>
</div>
<hr />
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
