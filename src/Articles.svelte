<script>
  import InfiniteScroll from "svelte-infinite-scroll";
  import articles from './articles.json';

  let page = 0;
  let size = 5;
  let datas = [];

  $: datas = [
     ...datas,
     ...articles.splice(size * page, size * (page + 1)),
  ];
</script>

<h1>Highlights</h1>
<container>
<article>
  {#each datas as article}
 <div class="article">
  <h2>{article.titre}</h2>
  <img src={article.image} alt={article.titre} width="341" height="237"/>
  <p>{article.texte}</p>
  <h5>
    All items loaded: {articles.length ? 'No' : 'Yes'}
  </h5>
</div>
    <hr />
  {/each}
  <InfiniteScroll
  hasMore={datas.length < articles.length}
  threshold={100}
  on:loadMore={() => page++} />
</article>
</container>

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
