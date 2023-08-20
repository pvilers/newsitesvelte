<script>
  import Article from "./Article.svelte";
  let articles = [
    {
      image: "img/pimthai.webp",
      titre: "PIMTHAI",
      texte: "REALISATION DU MENU DU TRAITEUR PIMTHAI",
    },
    {
      image: "img/sofille.webp",
      titre: "SO FILLE",
      texte: "REALISATION DU SITE INTERNET DE L'INSTITUT SOFILLE",
    },
    {
      image: "img/whynot.webp",
      titre: "WHY NOT EVENTS",
      texte:
        "REALISATION RÉALISATION IDENTITé GRAPHIQUE POUR WHY NOT EVENTS & WHY NOT TRAITEUR",
    },
    {
      image: "img/c21.webp",
      titre: "CENTURY 21",
      texte:
        "REALISATION DU SITE INTERNET DE CENTURY 21 AVANTAGE AVEC ACTIVIMMO",
    },
    {
      image: "img/peintagone.webp",
      titre: "PEINTAGONE",
      texte:
        "CRÉATION D’IDENTITÉ VISUELLE POUR LA SOCIÉTÉ DE PEINTURE 100% BELGE PEINTAGONE",
    },
    {
      image: "img/sainte-elisabeth.webp",
      titre: "SAINTE-ELISABETH",
      texte:
        "RÉALISATION DU SITE INTERNET DE L’ÉCOLE SAINTE-ELISABETH D’ARCHENNES",
    },
    {
      image: "img/jardinsenherbe.webp",
      titre: "JARDINS EN HERBE",
      texte:
        "RÉALISATION DU LOGO ET DE POLOS POUR L’ENTREPRISE DE JARDINAGE JARDINS EN HERBE",
    },
    {
      image: "img/terblock.webp",
      titre: "TERBLOCK",
      texte: "CRÉATION IDENTITÉ GRAPHIQUE ET SITE POUR LE CHÂTEAU DE TERBLOCK",
    },
    {
      image: "img/laure.webp",
      titre: "LAURE",
      texte: "CRÉATION D’UN FLYER POUR LE SALON DE TOILETTAGE LAURE",
    },
    {
      image: "img/gerardlaw.webp",
      titre: "GERARD LAW",
      texte:
        "RÉALISATION DU LOGO, identité graphique ET DU SITE DU BUREAU D'AVOCAT GERARD LAW",
    },
  ];
</script>

<h1>Highlights</h1>
<article>
  {#each articles as article}
    <Article {article} />
  {/each}
</article>
