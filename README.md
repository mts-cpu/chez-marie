<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
  <title>Chez Marie - Restaurant de la Mer</title>
  <style>
    /* Reset et variables */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    :root {
      --primary: #1e3a8a;
      --secondary: #3b82f6;
      --accent: #f59e0b;
      --text-dark: #1f2937;
      --text-light: #6b7280;
      --bg-light: #f8fafc;
      --white: #ffffff;
      --shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
      --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
    }

    body {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      background: var(--bg-light);
      color: var(--text-dark);
      line-height: 1.6;
      overflow-x: hidden;
    }

    /* Header mobile-first */
    .header {
      background: linear-gradient(135deg, var(--primary), var(--secondary));
      color: var(--white);
      padding: 0.75rem;
      text-align: center;
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      z-index: 100;
      box-shadow: var(--shadow-lg);
    }

    .header h1 {
      font-size: 1.2rem;
      font-weight: 700;
      margin-bottom: 0.25rem;
    }

    .header p {
      font-size: 0.8rem;
      opacity: 0.9;
    }

    /* Navigation mobile */
    .nav {
      background: var(--white);
      padding: 0.5rem 1rem;
      box-shadow: var(--shadow);
      position: fixed;
      top: 70px;
      left: 1rem;
      right: 1rem;
      z-index: 99;
      border-radius: 12px;
      max-width: calc(100% - 2rem);
    }

    .nav-list {
      display: flex;
      justify-content: space-around;
      list-style: none;
      gap: 0.25rem;
    }

    .nav-link {
      color: var(--text-dark);
      text-decoration: none;
      padding: 0.4rem 0.6rem;
      border-radius: 8px;
      font-size: 0.75rem;
      font-weight: 600;
      transition: all 0.2s ease;
      white-space: nowrap;
      min-height: 36px;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .nav-link:hover,
    .nav-link.active {
      background: var(--primary);
      color: var(--white);
    }

    /* Conteneur principal */
    .container {
      max-width: 100%;
      padding: 0.75rem;
      margin-top: 120px;
    }

    /* Sections */
    .section {
      background: var(--white);
      border-radius: 12px;
      padding: 1rem;
      margin-bottom: 0.75rem;
      box-shadow: var(--shadow);
      animation: fadeInUp 0.6s ease-out;
    }

    .section h2 {
      color: var(--primary);
      font-size: 1rem;
      font-weight: 700;
      margin-bottom: 0.75rem;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    /* Plat du jour - mise en avant */
    .plat-jour {
      background: linear-gradient(135deg, #fef3c7, #fde68a);
      border: 2px solid var(--accent);
      border-radius: 10px;
      padding: 0.75rem;
      margin-bottom: 0.75rem;
    }

    .plat-jour h3 {
      color: var(--text-dark);
      font-size: 0.9rem;
      font-weight: 700;
      margin-bottom: 0.25rem;
    }

    .plat-jour p {
      color: var(--text-light);
      font-size: 0.75rem;
    }

    /* Menu items */
    .menu-item {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      padding: 0.75rem 0;
      border-bottom: 1px solid #e5e7eb;
    }

    .menu-item:last-child {
      border-bottom: none;
    }

    .menu-content {
      flex: 1;
    }

    .menu-name {
      font-weight: 700;
      color: var(--text-dark);
      font-size: 0.85rem;
      margin-bottom: 0.2rem;
    }

    .menu-desc {
      color: var(--text-light);
      font-size: 0.7rem;
      line-height: 1.3;
    }

    .menu-price {
      color: var(--primary);
      font-weight: 700;
      font-size: 0.85rem;
      margin-left: 0.75rem;
      white-space: nowrap;
    }

    /* Catégories de menu */
    .menu-category {
      margin-bottom: 1.5rem;
    }

    .menu-category h3 {
      color: var(--secondary);
      font-size: 0.9rem;
      font-weight: 600;
      margin-bottom: 0.75rem;
      padding-bottom: 0.25rem;
      border-bottom: 2px solid var(--secondary);
    }

    /* Infos */
    .info-item {
      display: flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.5rem 0;
      border-bottom: 1px solid #e5e7eb;
    }

    .info-item:last-child {
      border-bottom: none;
    }

    .info-icon {
      width: 16px;
      height: 16px;
      background: var(--primary);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      color: var(--white);
      font-size: 0.6rem;
      flex-shrink: 0;
    }

    .info-text {
      flex: 1;
      font-size: 0.75rem;
    }

    .info-text a {
      color: var(--primary);
      text-decoration: none;
      font-weight: 600;
    }

    /* Avis */
    .avis {
      background: linear-gradient(135deg, #dbeafe, #bfdbfe);
      border-radius: 10px;
      padding: 0.75rem;
      margin: 0.75rem 0;
    }

    .avis blockquote {
      font-style: italic;
      color: var(--text-dark);
      margin-bottom: 0.5rem;
      font-size: 0.75rem;
    }

    .avis footer {
      color: var(--text-light);
      font-size: 0.65rem;
      font-weight: 600;
    }

    /* Footer */
    .footer {
      background: var(--primary);
      color: var(--white);
      text-align: center;
      padding: 1rem;
      margin-top: 1.5rem;
      border-radius: 12px 12px 0 0;
    }

    .footer p {
      font-size: 0.75rem;
      opacity: 0.9;
    }

    /* Boutons d'action */
    .action-buttons {
      display: flex;
      gap: 0.5rem;
      margin: 0.75rem 0;
      flex-wrap: wrap;
    }

    .btn {
      background: var(--primary);
      color: var(--white);
      border: none;
      padding: 0.5rem 1rem;
      border-radius: 8px;
      font-weight: 600;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 0.4rem;
      transition: all 0.2s ease;
      font-size: 0.75rem;
      min-height: 36px;
      justify-content: center;
    }

    .btn:hover {
      background: var(--secondary);
      transform: translateY(-1px);
    }

    .btn-secondary {
      background: var(--white);
      color: var(--primary);
      border: 2px solid var(--primary);
    }

    .btn-secondary:hover {
      background: var(--primary);
      color: var(--white);
    }

    /* Animations */
    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    /* Scroll smooth */
    html {
      scroll-behavior: smooth;
    }

    /* Amélioration de l'accessibilité */
    .nav-link:focus,
    .btn:focus {
      outline: 2px solid var(--accent);
      outline-offset: 2px;
    }

    /* Responsive */
    @media (min-width: 768px) {
      .container {
        max-width: 768px;
        margin: 0 auto;
      }

      .header h1 {
        font-size: 2rem;
      }

      .header p {
        font-size: 1rem;
      }

      .nav-list {
        justify-content: center;
        gap: 2rem;
      }

      .nav-link {
        font-size: 1rem;
        padding: 0.75rem 1.25rem;
      }

      .section {
        padding: 2rem;
      }

      .section h2 {
        font-size: 1.5rem;
      }

      .menu-item {
        padding: 1.25rem 0;
      }

      .menu-name {
        font-size: 1.1rem;
      }

      .menu-desc {
        font-size: 0.9rem;
      }

      .menu-price {
        font-size: 1.1rem;
      }
    }
  </style>
</head>
<body>

  <header class="header">
    <h1>Chez Marie</h1>
    <p>Restaurant familial - Cuisine créole & produits frais de la mer</p>
  </header>

  <nav class="nav">
    <ul class="nav-list">
      <li><a href="#infos" class="nav-link">📍 Infos</a></li>
      <li><a href="#plats-du-jour" class="nav-link">🌟 Plat du jour</a></li>
      <li><a href="#menu" class="nav-link">🍽️ Menu</a></li>
    </ul>
  </nav>

  <main class="container">

    <section id="infos" class="section">
      <h2>📍 Informations</h2>
      
      <div class="action-buttons">
        <a href="tel:+262692123456" class="btn">📞 Appeler</a>
        <a href="https://www.google.com/maps/place/Chez+marie" target="_blank" class="btn btn-secondary">🗺️ Itinéraire</a>
      </div>

      <div class="info-item">
        <div class="info-icon">📍</div>
        <div class="info-text">
          <strong>Adresse :</strong> 3 Rue des Sables, Saint-Gilles les Bains, La Réunion
        </div>
      </div>

      <div class="info-item">
        <div class="info-icon">📞</div>
        <div class="info-text">
          <strong>Téléphone :</strong> <a href="tel:+262692123456">06 92 12 34 56</a>
        </div>
      </div>

      <div class="info-item">
        <div class="info-icon">🕒</div>
        <div class="info-text">
          <strong>Horaires :</strong> Lun-Sam : 11h30-14h30 et 18h00-21h30
        </div>
      </div>

      <div class="info-item">
        <div class="info-icon">⭐</div>
        <div class="info-text">
          <strong>Avis Google :</strong> ⭐⭐⭐⭐⭐ (4.8/5) - <a href="https://www.google.com/search?q=chez+marie+saint-gilles+avis" target="_blank">Voir les avis</a>
        </div>
      </div>

      <div class="info-item">
        <div class="info-icon">📱</div>
        <div class="info-text">
          <strong>Réseaux :</strong> <a href="https://www.facebook.com/p/Chez-Marie-100070266363415" target="_blank">Facebook</a>
        </div>
      </div>
    </section>

    <section id="plats-du-jour" class="section">
      <h2>🌟 Plat du jour</h2>
      
      <div class="plat-jour">
        <h3>Érou su poivre vert, frites et fondue de poireaux - 23€</h3>
        <p>Poisson frais du jour, mariné au poivre vert, servi avec des frites maison croustillantes et une fondue de poireaux onctueuse.</p>
      </div>

      <div class="plat-jour">
        <h3>Langouste grillée beurre d'ail - 39,50€</h3>
        <p>Langouste pêchée localement, grillée à la perfection, nappée d'un beurre d'ail savoureux et parfumé.</p>
      </div>
    </section>

    <section id="menu" class="section">
      <h2>🍽️ Menu</h2>

      <div class="menu-category">
        <h3>🍹 Boissons</h3>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Jus de canne frais</div>
            <div class="menu-desc">Pressé à froid, sucré naturellement, saveur exotique intense.</div>
          </div>
          <div class="menu-price">4,50€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Bière locale</div>
            <div class="menu-desc">Brassée à La Réunion, légère et rafraîchissante.</div>
          </div>
          <div class="menu-price">5,00€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Softs</div>
            <div class="menu-desc">Bouteille d'eau, coca, sprite, etc...</div>
          </div>
          <div class="menu-price">-</div>
        </div>
      </div>

      <div class="menu-category">
        <h3>🍤 Apéritifs</h3>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Accras de morue</div>
            <div class="menu-desc">Beignets croustillants à la morue, recette traditionnelle créole.</div>
          </div>
          <div class="menu-price">7,50€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Samoussas crevettes</div>
            <div class="menu-desc">Pâté fin et croustillant, farci aux crevettes fraîches épicées.</div>
          </div>
          <div class="menu-price">8,00€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Ti punch</div>
            <div class="menu-desc">Cocktail créole au rhum, citron vert et sucre de canne.</div>
          </div>
          <div class="menu-price">6,00€</div>
        </div>
      </div>

      <div class="menu-category">
        <h3>🐟 Poissons & fruits de mer</h3>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Espadon grillé, sauce vanille</div>
            <div class="menu-desc">Poisson frais pêché localement, accompagné d'une sauce crémeuse à la vanille Bourbon.</div>
          </div>
          <div class="menu-price">22€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Fricassée de la mer aux agrumes</div>
            <div class="menu-desc">Espadon, camarons, calamars cuisinés aux zestes d'agrumes frais.</div>
          </div>
          <div class="menu-price">26€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Voilier rôti</div>
            <div class="menu-desc">Filet de voilier cuit au four avec un mélange d'épices réunionnaises.</div>
          </div>
          <div class="menu-price">21€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Thon banane</div>
            <div class="menu-desc">Thon frais servi avec une compotée de bananes épicées.</div>
          </div>
          <div class="menu-price">24€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Thazard à la créole</div>
            <div class="menu-desc">Poisson local mijoté avec tomates, oignons et curcuma.</div>
          </div>
          <div class="menu-price">23,50€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Tartare de thon</div>
            <div class="menu-desc">Thon frais coupé au couteau, assaisonné à la perfection.</div>
          </div>
          <div class="menu-price">20,50€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Tartare de thon à l'ancienne (moutarde)</div>
            <div class="menu-desc">Version traditionnelle avec une pointe de moutarde locale.</div>
          </div>
          <div class="menu-price">21,50€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Civet de zourites</div>
            <div class="menu-desc">Ragoût de poulpe mijoté au vin rouge et épices.</div>
          </div>
          <div class="menu-price">23€</div>
        </div>
      </div>

      <div class="menu-category">
        <h3>🥩 Viandes rouges</h3>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Entrecôte (France)</div>
            <div class="menu-desc">Viande française de qualité, grillée à la demande.</div>
          </div>
          <div class="menu-price">24€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Côte de bœuf (France)</div>
            <div class="menu-desc">Côte de bœuf tendre et juteuse, cuisson au charbon.</div>
          </div>
          <div class="menu-price">26€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Kangourou (Australie)</div>
            <div class="menu-desc">Viande maigre et savoureuse, marinée aux épices locales.</div>
          </div>
          <div class="menu-price">23€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Magret (France)</div>
            <div class="menu-desc">Magret de canard rosé, cuisson parfaite.</div>
          </div>
          <div class="menu-price">25€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Magret aux letchis</div>
            <div class="menu-desc">Magret de canard tendre, nappé d'une sauce sucrée aux letchis de saison.</div>
          </div>
          <div class="menu-price">26,50€</div>
        </div>
      </div>

      <div class="menu-category">
        <h3>🍗 Viandes blanches</h3>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Poulet à la créole</div>
            <div class="menu-desc">Poulet mariné et rôti aux épices traditionnelles.</div>
          </div>
          <div class="menu-price">18€</div>
        </div>
      </div>

      <div class="menu-category">
        <h3>🍰 Desserts</h3>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Flan coco maison</div>
            <div class="menu-desc">Flan onctueux à la noix de coco fraîche, recette authentique.</div>
          </div>
          <div class="menu-price">6,50€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Tarte aux fruits tropicaux</div>
            <div class="menu-desc">Pâte sablée croustillante, garnie de fruits frais de La Réunion.</div>
          </div>
          <div class="menu-price">7,00€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Gâteau patate</div>
            <div class="menu-desc">Spécialité réunionnaise à base de patate douce.</div>
          </div>
          <div class="menu-price">6€</div>
        </div>
        <div class="menu-item">
          <div class="menu-content">
            <div class="menu-name">Salade de fruits frais</div>
            <div class="menu-desc">Fruits de saison coupés et servis frais.</div>
          </div>
          <div class="menu-price">5,50€</div>
        </div>
      </div>
    </section>

    <section class="section">
      <h2>⭐ Avis clients</h2>
      
      <div class="avis">
        <blockquote>
          "Un accueil chaleureux et une cuisine délicieuse, tout est frais et authentique!"
        </blockquote>
        <footer>- Marie D.</footer>
      </div>

      <div class="avis">
        <blockquote>
          "Meilleur restaurant de fruits de mer de Saint-Gilles, je recommande vivement."
        </blockquote>
        <footer>- Jean P.</footer>
      </div>
    </section>

  </main>

  <footer class="footer">
    <p>© 2025 Chez Marie - Réalisé avec ❤ à La Réunion 🌴</p>
  </footer>

  <script>
    // Navigation active
    const navLinks = document.querySelectorAll('.nav-link');
    const sections = document.querySelectorAll('.section');

    // Observer pour détecter la section active
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          const id = entry.target.getAttribute('id');
          navLinks.forEach(link => {
            link.classList.remove('active');
            if (link.getAttribute('href') === `#${id}`) {
              link.classList.add('active');
            }
          });
        }
      });
    }, { threshold: 0.5 });

    sections.forEach(section => {
      observer.observe(section);
    });

    // Smooth scroll pour les liens de navigation
    navLinks.forEach(link => {
      link.addEventListener('click', (e) => {
        e.preventDefault();
        const targetId = link.getAttribute('href');
        const targetSection = document.querySelector(targetId);
        
        if (targetSection) {
          targetSection.scrollIntoView({
            behavior: 'smooth',
            block: 'start'
          });
        }
      });
    });

    // Animation au scroll
    const observerAnim = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.style.opacity = '1';
          entry.target.style.transform = 'translateY(0)';
        }
      });
    }, { threshold: 0.1 });

    document.querySelectorAll('.menu-item, .plat-jour, .avis').forEach(el => {
      el.style.opacity = '0';
      el.style.transform = 'translateY(20px)';
      el.style.transition = 'all 0.6s ease-out';
      observerAnim.observe(el);
    });
  </script>

</body>
</html> 
