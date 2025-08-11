# chez-marie
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=3, user-scalable=yes" />
  <title>Chez Marie - Restaurant de la Mer</title>
  <link rel="stylesheet" href="style.css.css" />
  <style>
    /* Intégration directe CSS à la demande, voir CSS complet ci-dessous */
  </style>
</head>
<body>

  <header>
    <div class="container">
      <h1>Chez Marie - Saint-Gilles</h1>
      <p>Restaurant familial - Cuisine créole & produits frais de la mer</p>
    </div>
  </header>

  <nav id="navbar">
    <ul>
      <li><a href="#infos" class="nav-link">Infos</a></li>
      <li><a href="#menu" class="nav-link">Menu</a></li>
      <li><a href="#plats-du-jour" class="nav-link">Plat du jour</a></li>
      
    </ul>
  </nav>

  <main class="container">

    <section id="infos" aria-label="Informations du restaurant">
      <h2>📍 Informations</h2>
      <p><strong>Adresse :</strong> 3 Rue des Sables, Saint-Gilles les Bains, La Réunion</p>
      <p><strong>Téléphone :</strong> <a href="tel:+262692123456">06 92 12 34 56</a></p>
      <p><strong>Horaires :</strong> Ouvert du lundi au samedi, de 11h30 à 14h30 et de 18h00 à 21h30</p>
      <p><strong>Retrouvez-nous sur :</strong> 
        <a href="https://www.facebook.com/people/Chez-Marie-Saint-Gilles/100063819519025/" target="_blank" rel="noopener noreferrer">Facebook</a> | 
        <a href="https://goo.gl/maps/EXEMPLE" target="_blank" rel="noopener noreferrer">Google Maps</a>
      </p>
      <p><strong>Avis Google :</strong> ⭐⭐⭐⭐⭐ (4.8/5) - <a href="https://www.google.com/search?q=chez+marie+saint-gilles+avis" target="_blank" rel="noopener noreferrer">Voir les avis</a></p>
    </section>

    <section id="plats-du-jour" aria-label="Plats du jour mis en avant">
      <h2>🌟 Plat du jour</h2>
      <article class="plat-jour">
        <h3>Érou su poivre vert, frites et fondue de poireaux - 23€</h3>
        <p>Poisson frais du jour, mariné au poivre vert, servi avec des frites maison croustillantes et une fondue de poireaux onctueuse.</p>
      </article>
      <article class="plat-jour">
        <h3>Langouste grillée beurre d’ail - 39,50€</h3>
        <p>Langouste pêchée localement, grillée à la perfection, nappée d’un beurre d’ail savoureux et parfumé.</p>
      </article>
    </section>

    <section id="menu" aria-label="Menu du restaurant">
      <h2>🍹 Boissons</h2>
      <ul class="menu-list">
        <li>
          <span class="name">Jus de canne frais</span>
          <span class="price">4,50€</span>
          <p class="desc">Pressé à froid, sucré naturellement, saveur exotique intense.</p>
        </li>
        <li>
          <span class="name">Bière locale</span>
          <span class="price">5,00€</span>
          <p class="desc">Brassée à La Réunion, légère et rafraîchissante.</p>
        </li>
        <li>
          <span class="name">soft</span>
          <span class="price"></span>
          <p class="desc">bouteille d'eau, coca, sprite, etc... </p>
        </li>
      </ul>

      <h2>🍤 Apéritifs</h2>
      <ul class="menu-list">
        <li>
          <span class="name">Accras de morue</span>
          <span class="price">7,50€</span>
          <p class="desc">Beignets croustillants à la morue, recette traditionnelle créole.</p>
        </li>
        <li>
          <span class="name">Samoussas crevettes</span>
          <span class="price">8,00€</span>
          <p class="desc">Pâté fin et croustillant, farci aux crevettes fraîches épicées.</p>
        </li>
        <li>
          <span class="name">Ti punch</span>
          <span class="price">6,00€</span>
          <p class="desc">Cocktail créole au rhum, citron vert et sucre de canne.</p>
        </li>
      </ul>

      <h2>🍽️ Plats</h2>

<h3>Poissons & fruits de mer</h3>
<ul class="menu-list">
  <li>
    <span class="name">Espadon grillé, sauce vanille</span>
    <span class="price">22€</span>
    <p class="desc">Poisson frais pêché localement, accompagné d'une sauce crémeuse à la vanille Bourbon.</p>
  </li>
  <li>
    <span class="name">Fricassée de la mer aux agrumes</span>
    <span class="price">26€</span>
    <p class="desc">Espadon, camarons, calamars cuisinés aux zestes d’agrumes frais.</p>
  </li>
  <li>
    <span class="name">Voilier rôti</span>
    <span class="price">21€</span>
    <p class="desc">Filet de voilier cuit au four avec un mélange d'épices réunionnaises.</p>
  </li>
  <li>
    <span class="name">Thon banane</span>
    <span class="price">24€</span>
    <p class="desc">Thon frais servi avec une compotée de bananes épicées.</p>
  </li>
  <li>
    <span class="name">Thazard à la créole</span>
    <span class="price">23,50€</span>
    <p class="desc">Poisson local mijoté avec tomates, oignons et curcuma.</p>
  </li>
  <li>
    <span class="name">Tartare de thon</span>
    <span class="price">20,50€</span>
    <p class="desc">Thon frais coupé au couteau, assaisonné à la perfection.</p>
  </li>
  <li>
    <span class="name">Tartare de thon à l'ancienne (moutarde)</span>
    <span class="price">21,50€</span>
    <p class="desc">Version traditionnelle avec une pointe de moutarde locale.</p>
  </li>
  <li>
    <span class="name">Civet de zourites</span>
    <span class="price">23€</span>
    <p class="desc">Ragoût de poulpe mijoté au vin rouge et épices.</p>
  </li>
</ul>

<h3>Viandes rouges</h3>
<ul class="menu-list">
  <li>
    <span class="name">Entrecôte (France)</span>
    <span class="price">24€</span>
    <p class="desc">Viande française de qualité, grillée à la demande.</p>
  </li>
  <li>
    <span class="name">Côte de bœuf (France)</span>
    <span class="price">26€</span>
    <p class="desc">Côte de bœuf tendre et juteuse, cuisson au charbon.</p>
  </li>
  <li>
    <span class="name">Kangourou (Australie)</span>
    <span class="price">23€</span>
    <p class="desc">Viande maigre et savoureuse, marinée aux épices locales.</p>
  </li>
  <li>
    <span class="name">Magret (France)</span>
    <span class="price">25€</span>
    <p class="desc">Magret de canard rosé, cuisson parfaite.</p>
  </li>
  <li>
    <span class="name">Magret aux letchis</span>
    <span class="price">26,50€</span>
    <p class="desc">Magret de canard tendre, nappé d’une sauce sucrée aux letchis de saison.</p>
  </li>
</ul>

<h3>Viandes blanches (poulet)</h3>
<ul class="menu-list">
  <li>
    <span class="name">Poulet à la créole</span>
    <span class="price">18€</span>
    <p class="desc">Poulet mariné et rôti aux épices traditionnelles.</p>
  </li>
</ul>


      <h2>🍰 Desserts</h2>
      <ul class="menu-list">
        <li>
          <span class="name">Flan coco maison</span>
          <span class="price">6,50€</span>
          <p class="desc">Flan onctueux à la noix de coco fraîche, recette authentique.</p>
        </li>
        <li>
          <span class="name">Tarte aux fruits tropicaux</span>
          <span class="price">7,00€</span>
          <p class="desc">Pâte sablée croustillante, garnie de fruits frais de La Réunion.</p>
        </li>
        <li>
          <span class="name">Gâteau patate</span>
          <span class="price">6€</span>
          <p class="desc">Spécialité réunionnaise à base de patate douce.</p>
        </li>
        <li>
          <span class="name">Salade de fruits frais</span>
          <span class="price">5,50€</span>
          <p class="desc">Fruits de saison coupés et servis frais.</p>
        </li>
      </ul>
    </section>

    <section id="avis-google" aria-label="Avis Google">
      <h2>⭐ Avis Google</h2>
      <blockquote>
        <p>"Un accueil chaleureux et une cuisine délicieuse, tout est frais et authentique!"</p>
        <footer>- Marie D.</footer>
      </blockquote>
      <blockquote>
        <p>"Meilleur restaurant de fruits de mer de Saint-Gilles, je recommande vivement."</p>
        <footer>- Jean P.</footer>
      </blockquote>
    </section>

  </main>

  <footer>
    <p>© 2025 Chez Marie - Réalisé avec ❤ à La Réunion 🌴</p>
  </footer>

</body>
</html>
