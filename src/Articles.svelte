<script>
import Article from "./Article.svelte";
  let articles = [
    {
      image: "img/c21.jpg",
      titre: "CENTURY 21",
      texte:
        "REALISATION DU SITE INTERNET DE CENTURY 21 AVANTAGE AVEC ACTIVIMMO",
    },
    
    {
      image: "img/sainte-elisabeth.jpg",
      titre: "SAINTE-ELISABETH",
      texte:
        "RÉALISATION DU SITE INTERNET DE L’ÉCOLE SAINTE-ELISABETH D’ARCHENNES",
    },
    {
      image: "img/terblock.jpg",
      titre: "TERBLOCK",
      texte:
        "CRÉATION IDENTITÉ GRAPHIQUE ET SITE POUR LE CHÂTEAU DE TERBLOCK"
    },
    {
      image: "img/laure.jpg",
      titre: "LAURE",
      texte:
        "CRÉATION D’UN FLYER POUR LE SALON DE TOILETTAGE LAURE"
    }
  ];
</script>
<h1>Succes stories</h1>
<div>
{#each articles as article}
<Article {article}/>
{/each}
</div>
<style>
  div {
    margin-top : 10rem;
    margin-bottom : 10rem;
  }
</style>
