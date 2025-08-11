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
/* Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Couleurs pro, neutres */
:root {
  --bleu-fonce: #0a3d62;
  --gris-fonce: #2f3640;
  --gris-clair: #718093;
  --blanc: #ffffff;
  --gris-bg: #f5f6fa;
  --bleu-hover: #0984e3;
  --ombre: rgba(0, 0, 0, 0.1);
}

/* Body */
body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: var(--gris-bg);
  color: var(--gris-fonce);
  padding: 50px 20px;
  text-align: center; /* centre tout par défaut */
}

/* Conteneur principal */
body > * {
  max-width: 900px;
  margin: auto;
  background: var(--blanc);
  border-radius: 10px;
  box-shadow: 0 6px 18px var(--ombre);
  padding: 40px 50px;
  text-align: center; /* centre contenu */
}

/* Header */
header {
  margin-bottom: 30px;
  text-align: center;
}

header h1 {
  color: var(--bleu-fonce);
  font-size: 3rem;
  font-weight: 700;
  margin-bottom: 10px;
}

header p {
  font-size: 1.3rem;
  color: var(--gris-clair);
  font-weight: 600;
}

/* Navigation sticky */
nav#navbar {
  position: sticky;
  top: 0;
  background: var(--blanc);
  z-index: 100;
  box-shadow: 0 2px 8px var(--ombre);
  padding: 15px 0;
  margin-bottom: 40px;
  text-align: center;
}

nav#navbar ul {
  list-style: none;
  display: inline-flex;
  gap: 40px;
  padding: 0;
  margin: 0;
  justify-content: center;
}

nav#navbar ul li a {
  text-decoration: none;
  color: var(--bleu-fonce);
  font-weight: 700;
  font-size: 1.2rem;
  padding: 8px 15px;
  border-radius: 6px;
  transition: background-color 0.3s ease, color 0.3s ease;
  user-select: none;
}

nav#navbar ul li a:hover,
nav#navbar ul li a:focus,
nav#navbar ul li a.active {
  background-color: var(--bleu-fonce);
  color: var(--blanc);
  outline: none;
}

/* Sections générales */
section, #avis-google {
  max-width: 900px;
  margin: 40px auto;
  padding: 0 20px;
  text-align: center; /* Centre texte */
}

/* Titres des sections */
section h2 {
  font-size: 2.4rem;
  color: var(--bleu-fonce);
  border-bottom: 3px solid var(--bleu-fonce);
  padding-bottom: 8px;
  margin-bottom: 30px;
  font-weight: 700;
}

/* Liste des plats centrée dans son conteneur */
.menu-list {
  list-style: none;
  padding: 0;
  max-width: 700px;
  margin: 0 auto 40px auto; /* centre horizontal + espace dessous */
  text-align: left; /* texte aligné à gauche pour lisibilité */
}

/* Chaque plat - grille 2 colonnes */
.menu-list li {
  padding: 15px 20px;
  border-bottom: 1px solid var(--gris-bg);
  font-size: 1.25rem;
  font-weight: 600;
  color: var(--gris-fonce);
  cursor: default;
  transition: background-color 0.2s ease;

  display: grid;
  grid-template-columns: 1fr 80px;
  align-items: center;
  column-gap: 20px;
}

.menu-list li:last-child {
  border-bottom: none;
}

.menu-list li:hover {
  background-color: var(--gris-bg);
}

/* Nom du plat et description */
.menu-list li .name-desc {
  display: flex;
  flex-direction: column;
}

.menu-list li .name {
  font-weight: 700;
  font-size: 1.3rem;
  color: var(--bleu-fonce);
}

.menu-list li .description {
  font-weight: 400;
  font-size: 1rem;
  color: var(--gris-clair);
  margin-top: 4px;
  font-style: italic;
}

/* Prix à droite, aligné */
.menu-list li .price {
  color: var(--bleu-fonce);
  font-weight: 700;
  text-align: right;
  white-space: nowrap;
}

/* Plat du jour - mise en avant */
#plat-du-jour {
  background-color: #eaf3fc;
  border-radius: 12px;
  padding: 30px 40px;
  max-width: 700px;
  margin: 30px auto 60px auto;
  box-shadow: 0 4px 12px rgba(10, 61, 98, 0.15);
  font-size: 1.4rem;
  font-weight: 700;
  color: var(--bleu-fonce);
  line-height: 1.4;
}

/* Galerie */
#galerie {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
}

#galerie img {
  max-width: 320px;
  width: 100%;
  border-radius: 12px;
  box-shadow: 0 6px 18px var(--ombre);
  cursor: pointer;
  transition: transform 0.3s ease;
}

#galerie img:hover,
#galerie img:focus {
  transform: scale(1.05);
  outline: none;
}

/* Barre infos */
#infos p {
  font-size: 1.2rem;
  margin-bottom: 18px;
  color: var(--gris-fonce);
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
  line-height: 1.5;
}

#infos a {
  color: var(--bleu-fonce);
  text-decoration: none;
  font-weight: 600;
}

#infos a:hover,
#infos a:focus {
  text-decoration: underline;
}

/* Avis Google */
#avis-google {
  max-width: 600px;
  margin: 40px auto;
  padding: 20px 40px;
  background-color: #f9faff;
  border: 1px solid var(--bleu-fonce);
  border-radius: 10px;
  color: var(--bleu-fonce);
  font-weight: 600;
  font-size: 1.2rem;
  font-style: italic;
  text-align: center;
  box-shadow: 0 4px 10px rgba(10, 61, 98, 0.15);
}

/* Footer */
footer {
  margin-top: 60px;
  padding: 20px 10px;
  font-size: 1rem;
  color: var(--gris-clair);
  border-top: 3px solid var(--bleu-fonce);
  text-align: center;
  font-style: italic;
}

/* Responsive */
@media (max-width: 750px) {
  body > * {
    padding: 30px 25px;
  }

  nav#navbar ul {
    flex-direction: column;
    gap: 12px;
  }

  .menu-list {
    max-width: 100%;
    padding: 0 15px;
  }

  /* Sur mobile, on passe en flex-col pour la liste des plats */
  .menu-list li {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }

  .menu-list li .price {
    text-align: left;
    min-width: auto;
    margin-top: 8px;
    color: var(--gris-clair);
    font-weight: 600;
  }
}

</html>
