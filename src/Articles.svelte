<script>
  import articles from "./articles.json";
  import Article from "./Article.svelte"
</script>
<container>
  <article>
    {#each articles as article}
      <Article {article} />
    {/each}
  </article>
  </container>


