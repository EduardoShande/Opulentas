/* ===================================
   PAULA NAILS STUDIO - STYLES
   Paleta: Rosa dusty, lila, nude, champagne
   =================================== */

/* Variables CSS */
:root {
    /* Colores principales */
    --color-primary: #d4a5a5;      /* Rosa dusty */
    --color-secondary: #c9b8d4;    /* Lila suave */
    --color-accent: #e8c4c4;       /* Rosa claro */
    --color-gold: #d4af37;         /* Dorado champagne */
    --color-nude: #e5d4c0;         /* Nude beige */
    
    /* Colores de fondo */
    --bg-cream: #fdfbf9;
    --bg-light: #faf7f5;
    --bg-soft: #f5ebe0;
    
    /* Colores de texto */
    --text-dark: #2d2a26;
    --text-medium: #5c564f;
    --text-light: #8a8279;
    
    /* Gradientes */
    --gradient-primary: linear-gradient(135deg, #d4a5a5 0%, #c9b8d4 50%, #e8c4c4 100%);
    --gradient-soft: linear-gradient(180deg, #fdfbf9 0%, #f5ebe0 100%);
    --gradient-hero: linear-gradient(135deg, #fdfbf9 0%, #f5ebe0 30%, #faf7f5 70%, #fdfbf9 100%);
    
    /* Tipografías */
    --font-display: 'Cormorant Garamond', serif;
    --font-body: 'Outfit', sans-serif;
    
    /* Espaciado */
    --space-xs: 0.5rem;
    --space-sm: 1rem;
    --space-md: 1.5rem;
    --space-lg: 2.5rem;
    --space-xl: 4rem;
    --space-2xl: 6rem;
    
    /* Bordes */
    --radius-sm: 8px;
    --radius-md: 16px;
    --radius-lg: 24px;
    --radius-full: 9999px;
    
    /* Sombras */
    --shadow-soft: 0 4px 20px rgba(212, 165, 165, 0.15);
    --shadow-medium: 0 8px 40px rgba(212, 165, 165, 0.2);
    --shadow-strong: 0 20px 60px rgba(212, 165, 165, 0.25);
    
    /* Transiciones */
    --transition-fast: 0.2s ease;
    --transition-normal: 0.3s ease;
    --transition-slow: 0.5s cubic-bezier(0.4, 0, 0.2, 1);
}

/* Reset y base */
*, *::before, *::after {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    font-size: 16px;
}

body {
    font-family: var(--font-body);
    font-weight: 400;
    color: var(--text-dark);
    background: var(--bg-cream);
    line-height: 1.6;
    overflow-x: hidden;
    cursor: none;
}

/* Cursor personalizado */
.cursor {
    width: 12px;
    height: 12px;
    background: var(--color-primary);
    border-radius: 50%;
    position: fixed;
    pointer-events: none;
    z-index: 10000;
    mix-blend-mode: difference;
    transform: translate(-50%, -50%);
    transition: transform 0.1s ease, width 0.3s ease, height 0.3s ease;
}

.cursor-follower {
    width: 40px;
    height: 40px;
    border: 1px solid var(--color-primary);
    border-radius: 50%;
    position: fixed;
    pointer-events: none;
    z-index: 9999;
    transform: translate(-50%, -50%);
    transition: transform 0.15s ease-out, width 0.3s ease, height 0.3s ease, border-color 0.3s ease;
}

body.cursor-hover .cursor {
    transform: translate(-50%, -50%) scale(2);
    background: var(--color-gold);
}

body.cursor-hover .cursor-follower {
    width: 60px;
    height: 60px;
    border-color: var(--color-gold);
}

@media (max-width: 768px) {
    .cursor, .cursor-follower {
        display: none;
    }
    body {
        cursor: auto;
    }
}

/* Selección de texto */
::selection {
    background: var(--color-primary);
    color: white;
}

/* Links y botones base */
a {
    text-decoration: none;
    color: inherit;
    transition: var(--transition-normal);
}

button {
    border: none;
    background: none;
    cursor: pointer;
    font-family: inherit;
}

img {
    max-width: 100%;
    height: auto;
    display: block;
}

/* ===================================
   NAVEGACIÓN
   =================================== */
.navbar {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1000;
    padding: var(--space-sm) var(--space-md);
    background: rgba(253, 251, 249, 0.85);
    backdrop-filter: blur(20px);
    -webkit-backdrop-filter: blur(20px);
    border-bottom: 1px solid rgba(212, 165, 165, 0.1);
    transition: var(--transition-normal);
}

.navbar.scrolled {
    padding: var(--space-xs) var(--space-md);
    box-shadow: var(--shadow-soft);
}

.nav-container {
    max-width: 1400px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    display: flex;
    align-items: center;
    gap: var(--space-xs);
}

.logo-icon {
    font-size: 1.5rem;
    color: var(--color-primary);
    animation: sparkle 2s ease-in-out infinite;
}

@keyframes sparkle {
    0%, 100% { opacity: 1; transform: scale(1); }
    50% { opacity: 0.7; transform: scale(1.1); }
}

.logo-text {
    font-family: var(--font-display);
    font-size: 1.5rem;
    font-weight: 500;
    letter-spacing: 0.02em;
}

.nav-links {
    display: flex;
    align-items: center;
    gap: var(--space-lg);
}

.nav-link {
    font-size: 0.9rem;
    font-weight: 500;
    color: var(--text-medium);
    position: relative;
    padding: var(--space-xs) 0;
}

.nav-link::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 0;
    height: 2px;
    background: var(--gradient-primary);
    transition: var(--transition-normal);
    border-radius: var(--radius-full);
}

.nav-link:hover::after {
    width: 100%;
}

.nav-link:hover {
    color: var(--text-dark);
}

.cta-nav {
    background: var(--gradient-primary);
    color: white !important;
    padding: var(--space-xs) var(--space-md) !important;
    border-radius: var(--radius-full);
}

.cta-nav::after {
    display: none;
}

.cta-nav:hover {
    transform: translateY(-2px);
    box-shadow: var(--shadow-medium);
}

/* Menú móvil toggle */
.menu-toggle {
    display: none;
    flex-direction: column;
    gap: 5px;
    padding: var(--space-xs);
}

.menu-toggle span {
    width: 24px;
    height: 2px;
    background: var(--text-dark);
    border-radius: var(--radius-full);
    transition: var(--transition-normal);
}

.menu-toggle.active span:nth-child(1) {
    transform: rotate(45deg) translate(5px, 5px);
}

.menu-toggle.active span:nth-child(2) {
    opacity: 0;
}

.menu-toggle.active span:nth-child(3) {
    transform: rotate(-45deg) translate(5px, -5px);
}

/* Menú móvil */
.mobile-menu {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(253, 251, 249, 0.98);
    backdrop-filter: blur(20px);
    z-index: 999;
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    visibility: hidden;
    transition: var(--transition-slow);
}

.mobile-menu.active {
    opacity: 1;
    visibility: visible;
}

.mobile-menu-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: var(--space-lg);
}

.mobile-link {
    font-family: var(--font-display);
    font-size: 2rem;
    font-weight: 500;
    color: var(--text-dark);
    opacity: 0;
    transform: translateY(20px);
    transition: var(--transition-normal);
}

.mobile-menu.active .mobile-link {
    opacity: 1;
    transform: translateY(0);
}

.mobile-menu.active .mobile-link:nth-child(1) { transition-delay: 0.1s; }
.mobile-menu.active .mobile-link:nth-child(2) { transition-delay: 0.2s; }
.mobile-menu.active .mobile-link:nth-child(3) { transition-delay: 0.3s; }
.mobile-menu.active .mobile-link:nth-child(4) { transition-delay: 0.4s; }

@media (max-width: 768px) {
    .nav-links {
        display: none;
    }
    .menu-toggle {
        display: flex;
    }
}

/* ===================================
   HERO SECTION
   =================================== */
.hero {
    min-height: 100vh;
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    padding: calc(80px + var(--space-xl)) var(--space-lg) var(--space-xl);
    position: relative;
    overflow: hidden;
}

.hero-bg {
    position: absolute;
    inset: 0;
    background: var(--gradient-hero);
    z-index: -1;
}

/* Orbes de gradiente animados */
.gradient-orb {
    position: absolute;
    border-radius: 50%;
    filter: blur(80px);
    opacity: 0.6;
    animation: float 20s ease-in-out infinite;
}

.orb-1 {
    width: 600px;
    height: 600px;
    background: radial-gradient(circle, var(--color-primary) 0%, transparent 70%);
    top: -200px;
    right: -100px;
    animation-delay: 0s;
}

.orb-2 {
    width: 400px;
    height: 400px;
    background: radial-gradient(circle, var(--color-secondary) 0%, transparent 70%);
    bottom: -100px;
    left: -100px;
    animation-delay: -7s;
}

.orb-3 {
    width: 300px;
    height: 300px;
    background: radial-gradient(circle, var(--color-accent) 0%, transparent 70%);
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    animation-delay: -14s;
}

@keyframes float {
    0%, 100% { transform: translate(0, 0) scale(1); }
    25% { transform: translate(30px, -30px) scale(1.05); }
    50% { transform: translate(-20px, 20px) scale(0.95); }
    75% { transform: translate(20px, 30px) scale(1.02); }
}

/* Elementos flotantes */
.floating-elements {
    position: absolute;
    inset: 0;
    pointer-events: none;
}

.float-element {
    position: absolute;
    font-size: 1.5rem;
    opacity: 0.3;
    animation: floatElement 15s ease-in-out infinite;
}

.el-1 { top: 15%; left: 10%; animation-delay: 0s; color: var(--color-primary); }
.el-2 { top: 25%; right: 15%; animation-delay: -3s; color: var(--color-secondary); }
.el-3 { bottom: 30%; left: 20%; animation-delay: -6s; color: var(--color-gold); }
.el-4 { bottom: 20%; right: 25%; animation-delay: -9s; color: var(--color-primary); }
.el-5 { top: 50%; left: 5%; animation-delay: -12s; color: var(--color-accent); }

@keyframes floatElement {
    0%, 100% { transform: translateY(0) rotate(0deg); }
    50% { transform: translateY(-20px) rotate(180deg); }
}

/* Contenido del hero */
.hero-content {
    position: relative;
    z-index: 2;
    padding-right: var(--space-xl);
}

.hero-badge {
    display: inline-flex;
    align-items: center;
    gap: var(--space-xs);
    background: rgba(212, 165, 165, 0.15);
    border: 1px solid rgba(212, 165, 165, 0.3);
    padding: var(--space-xs) var(--space-md);
    border-radius: var(--radius-full);
    font-size: 0.85rem;
    color: var(--text-medium);
    margin-bottom: var(--space-md);
}

.badge-icon {
    color: var(--color-primary);
    animation: pulse 2s ease-in-out infinite;
}

@keyframes pulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.2); }
}

.hero-title {
    font-family: var(--font-display);
    font-weight: 500;
    line-height: 1.1;
    margin-bottom: var(--space-md);
}

.title-line {
    display: block;
    font-size: clamp(2.5rem, 6vw, 4.5rem);
    color: var(--text-dark);
}

.title-accent {
    background: var(--gradient-primary);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    font-style: italic;
}

.hero-subtitle {
    font-size: 1.1rem;
    color: var(--text-medium);
    max-width: 500px;
    margin-bottom: var(--space-lg);
    line-height: 1.7;
}

/* Botones CTA */
.hero-cta {
    display: flex;
    flex-wrap: wrap;
    gap: var(--space-sm);
    margin-bottom: var(--space-xl);
}

.btn {
    display: inline-flex;
    align-items: center;
    gap: var(--space-xs);
    padding: var(--space-sm) var(--space-lg);
    border-radius: var(--radius-full);
    font-weight: 500;
    font-size: 0.95rem;
    transition: var(--transition-normal);
    position: relative;
    overflow: hidden;
}

.btn::before {
    content: '';
    position: absolute;
    inset: 0;
    background: rgba(255, 255, 255, 0.2);
    transform: translateX(-100%);
    transition: var(--transition-normal);
}

.btn:hover::before {
    transform: translateX(0);
}

.btn-primary {
    background: var(--gradient-primary);
    color: white;
    box-shadow: var(--shadow-medium);
}

.btn-primary:hover {
    transform: translateY(-3px);
    box-shadow: var(--shadow-strong);
}

.btn-arrow {
    width: 20px;
    height: 20px;
    stroke-width: 2;
    transition: var(--transition-normal);
}

.btn-primary:hover .btn-arrow {
    transform: translateX(5px);
}

.btn-secondary {
    background: white;
    color: var(--text-dark);
    border: 1px solid rgba(212, 165, 165, 0.3);
}

.btn-secondary:hover {
    background: var(--bg-soft);
    border-color: var(--color-primary);
}

/* Estadísticas */
.hero-stats {
    display: flex;
    align-items: center;
    gap: var(--space-lg);
}

.stat {
    text-align: center;
}

.stat-number {
    font-family: var(--font-display);
    font-size: 2rem;
    font-weight: 600;
    color: var(--text-dark);
    display: block;
}

.stat-number::after {
    content: '+';
    color: var(--color-primary);
}

.stat-label {
    font-size: 0.8rem;
    color: var(--text-light);
    text-transform: uppercase;
    letter-spacing: 0.1em;
}

.stat-divider {
    width: 1px;
    height: 40px;
    background: rgba(212, 165, 165, 0.3);
}

/* Visual del hero */
.hero-visual {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
}

.hero-image-wrapper {
    position: relative;
    width: 100%;
    max-width: 450px;
}

.hero-image-frame {
    aspect-ratio: 3/4;
    background: white;
    border-radius: var(--radius-lg);
    box-shadow: var(--shadow-strong);
    overflow: hidden;
    position: relative;
}

.image-placeholder {
    width: 100%;
    height: 100%;
    background: var(--gradient-soft);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: var(--space-sm);
}

.placeholder-icon {
    font-size: 4rem;
    animation: bounce 2s ease-in-out infinite;
}

@keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
}

.placeholder-text {
    font-family: var(--font-display);
    font-size: 1.2rem;
    color: var(--text-light);
    font-style: italic;
}

/* Decoraciones del hero */
.hero-decoration {
    position: absolute;
    border-radius: 50%;
    z-index: -1;
}

.dec-1 {
    width: 200px;
    height: 200px;
    border: 2px dashed var(--color-primary);
    opacity: 0.3;
    top: -30px;
    right: -30px;
    animation: rotate 30s linear infinite;
}

.dec-2 {
    width: 150px;
    height: 150px;
    background: var(--color-secondary);
    opacity: 0.2;
    bottom: -20px;
    left: -20px;
}

@keyframes rotate {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
}

/* Indicador de scroll */
.scroll-indicator {
    position: absolute;
    bottom: var(--space-lg);
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: var(--space-xs);
    color: var(--text-light);
    font-size: 0.8rem;
    animation: fadeInUp 1s ease-out 1.5s both;
}

.scroll-line {
    width: 1px;
    height: 40px;
    background: linear-gradient(to bottom, var(--color-primary), transparent);
    animation: scrollLine 2s ease-in-out infinite;
}

@keyframes scrollLine {
    0%, 100% { transform: scaleY(1); opacity: 1; }
    50% { transform: scaleY(0.5); opacity: 0.5; }
}

/* Hero responsive */
@media (max-width: 1024px) {
    .hero {
        grid-template-columns: 1fr;
        text-align: center;
        padding-top: calc(80px + var(--space-lg));
    }
    
    .hero-content {
        padding-right: 0;
        order: 2;
    }
    
    .hero-visual {
        order: 1;
        margin-bottom: var(--space-lg);
    }
    
    .hero-image-wrapper {
        max-width: 300px;
    }
    
    .hero-subtitle {
        margin-left: auto;
        margin-right: auto;
    }
    
    .hero-cta {
        justify-content: center;
    }
    
    .hero-stats {
        justify-content: center;
    }
}

@media (max-width: 480px) {
    .hero-stats {
        flex-direction: column;
        gap: var(--space-md);
    }
    
    .stat-divider {
        width: 60px;
        height: 1px;
    }
}

/* ===================================
   SECCIÓN SOBRE MÍ
   =================================== */
.about {
    padding: var(--space-2xl) var(--space-lg);
    background: white;
    position: relative;
}

.about-container {
    max-width: 1200px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 1fr 1.2fr;
    gap: var(--space-xl);
    align-items: center;
}

.about-image {
    position: relative;
}

.about-image .image-frame {
    aspect-ratio: 4/5;
    background: var(--gradient-soft);
    border-radius: var(--radius-lg);
    overflow: hidden;
    box-shadow: var(--shadow-medium);
}

.about-placeholder {
    background: linear-gradient(135deg, var(--color-accent) 0%, var(--color-secondary) 100%);
}

.about-badge {
    position: absolute;
    bottom: -20px;
    right: -20px;
    background: white;
    padding: var(--space-md);
    border-radius: var(--radius-md);
    box-shadow: var(--shadow-medium);
    text-align: center;
}

.badge-year {
    font-family: var(--font-display);
    font-size: 2.5rem;
    font-weight: 600;
    color: var(--color-primary);
    display: block;
    line-height: 1;
}

.badge-text {
    font-size: 0.75rem;
    color: var(--text-light);
    text-transform: uppercase;
    letter-spacing: 0.1em;
}

/* Tags de sección */
.section-tag {
    display: inline-block;
    font-size: 0.85rem;
    color: var(--color-primary);
    text-transform: uppercase;
    letter-spacing: 0.15em;
    margin-bottom: var(--space-sm);
}

.section-title {
    font-family: var(--font-display);
    font-size: clamp(2rem, 4vw, 3rem);
    font-weight: 500;
    line-height: 1.2;
    color: var(--text-dark);
    margin-bottom: var(--space-md);
}

.text-accent {
    background: var(--gradient-primary);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.about-text {
    margin-bottom: var(--space-lg);
}

.about-text p {
    color: var(--text-medium);
    margin-bottom: var(--space-sm);
    line-height: 1.8;
}

.about-text strong {
    color: var(--text-dark);
}

.about-text em {
    color: var(--color-primary);
    font-style: italic;
}

/* Valores */
.about-values {
    display: flex;
    flex-wrap: wrap;
    gap: var(--space-md);
}

.value {
    display: flex;
    align-items: center;
    gap: var(--space-xs);
    background: var(--bg-soft);
    padding: var(--space-xs) var(--space-md);
    border-radius: var(--radius-full);
    font-size: 0.9rem;
    color: var(--text-medium);
}

.value-icon {
    color: var(--color-primary);
}

@media (max-width: 768px) {
    .about-container {
        grid-template-columns: 1fr;
        text-align: center;
    }
    
    .about-image {
        max-width: 350px;
        margin: 0 auto;
    }
    
    .about-badge {
        right: 0;
    }
    
    .about-values {
        justify-content: center;
    }
}

/* ===================================
   SECCIÓN BENEFICIOS
   =================================== */
.benefits {
    padding: var(--space-2xl) var(--space-lg);
    position: relative;
    overflow: hidden;
}

.benefits-bg {
    position: absolute;
    inset: 0;
    background: var(--gradient-soft);
    z-index: -1;
}

.benefits-pattern {
    position: absolute;
    inset: 0;
    background-image: radial-gradient(circle at 2px 2px, var(--color-primary) 1px, transparent 0);
    background-size: 40px 40px;
    opacity: 0.05;
}

.benefits-container {
    max-width: 1200px;
    margin: 0 auto;
}

.benefits-header {
    text-align: center;
    margin-bottom: var(--space-xl);
}

.benefits-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: var(--space-md);
}

.benefit-card {
    background: white;
    padding: var(--space-lg);
    border-radius: var(--radius-lg);
    box-shadow: var(--shadow-soft);
    transition: var(--transition-normal);
    position: relative;
    overflow: hidden;
}

.benefit-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: var(--gradient-primary);
    transform: scaleX(0);
    transform-origin: left;
    transition: var(--transition-normal);
}

.benefit-card:hover {
    transform: translateY(-5px);
    box-shadow: var(--shadow-medium);
}

.benefit-card:hover::before {
    transform: scaleX(1);
}

.benefit-icon {
    width: 60px;
    height: 60px;
    background: var(--bg-soft);
    border-radius: var(--radius-md);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.8rem;
    margin-bottom: var(--space-md);
    transition: var(--transition-normal);
}

.benefit-card:hover .benefit-icon {
    background: var(--gradient-primary);
    transform: scale(1.1) rotate(5deg);
}

.benefit-title {
    font-family: var(--font-display);
    font-size: 1.3rem;
    font-weight: 500;
    color: var(--text-dark);
    margin-bottom: var(--space-xs);
}

.benefit-text {
    font-size: 0.9rem;
    color: var(--text-medium);
    line-height: 1.7;
}

/* Card CTA especial */
.benefit-cta {
    background: var(--gradient-primary);
    display: flex;
    align-items: center;
    justify-content: center;
}

.benefit-cta::before {
    display: none;
}

.benefit-cta-content {
    text-align: center;
    color: white;
}

.benefit-cta-icon {
    font-size: 2rem;
    display: block;
    margin-bottom: var(--space-xs);
    transition: var(--transition-normal);
}

.benefit-cta:hover .benefit-cta-icon {
    transform: translateX(10px);
}

.benefit-cta-title {
    font-family: var(--font-display);
    font-size: 1.3rem;
    margin-bottom: var(--space-sm);
}

.benefit-cta-link {
    display: inline-block;
    background: white;
    color: var(--color-primary);
    padding: var(--space-xs) var(--space-md);
    border-radius: var(--radius-full);
    font-weight: 500;
    font-size: 0.9rem;
    transition: var(--transition-normal);
}

.benefit-cta-link:hover {
    transform: scale(1.05);
    box-shadow: var(--shadow-soft);
}

@media (max-width: 1024px) {
    .benefits-grid {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (max-width: 640px) {
    .benefits-grid {
        grid-template-columns: 1fr;
    }
}

/* ===================================
   SECCIÓN GALERÍA
   =================================== */
.gallery {
    padding: var(--space-2xl) var(--space-lg);
    background: white;
}

.gallery-container {
    max-width: 1200px;
    margin: 0 auto;
}

.gallery-header {
    text-align: center;
    margin-bottom: var(--space-xl);
}

.gallery-subtitle {
    font-size: 1.1rem;
    color: var(--text-medium);
    max-width: 500px;
    margin: 0 auto;
}

.gallery-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 280px);
    gap: var(--space-md);
}

.gallery-item {
    position: relative;
    border-radius: var(--radius-lg);
    overflow: hidden;
    cursor: pointer;
}

.gallery-item.item-1 {
    grid-row: span 2;
}

.gallery-image {
    width: 100%;
    height: 100%;
}

.gallery-placeholder {
    background: var(--gradient-soft);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: var(--space-xs);
    transition: var(--transition-slow);
}

.gallery-placeholder .placeholder-icon {
    font-size: 3rem;
}

.gallery-placeholder .placeholder-text {
    font-size: 0.9rem;
}

.gallery-overlay {
    position: absolute;
    inset: 0;
    background: linear-gradient(to top, rgba(45, 42, 38, 0.8), transparent 60%);
    padding: var(--space-md);
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    opacity: 0;
    transition: var(--transition-normal);
}

.gallery-item:hover .gallery-overlay {
    opacity: 1;
}

.gallery-item:hover .gallery-placeholder {
    transform: scale(1.05);
}

.gallery-tag {
    display: inline-block;
    background: var(--color-primary);
    color: white;
    padding: 4px 12px;
    border-radius: var(--radius-full);
    font-size: 0.75rem;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    margin-bottom: var(--space-xs);
    width: fit-content;
}

.gallery-overlay h4 {
    color: white;
    font-family: var(--font-display);
    font-size: 1.2rem;
    font-weight: 500;
}

.gallery-cta {
    text-align: center;
    margin-top: var(--space-xl);
}

.gallery-cta p {
    color: var(--text-medium);
    margin-bottom: var(--space-md);
}

.btn-outline {
    background: transparent;
    border: 2px solid var(--color-primary);
    color: var(--color-primary);
}

.btn-outline:hover {
    background: var(--color-primary);
    color: white;
}

.btn-outline .social-icon {
    width: 18px;
    height: 18px;
}

@media (max-width: 768px) {
    .gallery-grid {
        grid-template-columns: repeat(2, 1fr);
        grid-template-rows: auto;
    }
    
    .gallery-item.item-1 {
        grid-row: span 1;
    }
}

@media (max-width: 480px) {
    .gallery-grid {
        grid-template-columns: 1fr;
    }
}

/* ===================================
   SECCIÓN TESTIMONIOS
   =================================== */
.testimonials {
    padding: var(--space-2xl) var(--space-lg);
    background: var(--bg-soft);
    overflow: hidden;
}

.testimonials-container {
    max-width: 1200px;
    margin: 0 auto;
    text-align: center;
}

.testimonials-slider {
    margin-top: var(--space-xl);
    overflow: visible;
}

.testimonial-track {
    display: flex;
    gap: var(--space-md);
    animation: scroll 30s linear infinite;
}

@keyframes scroll {
    0% { transform: translateX(0); }
    100% { transform: translateX(calc(-100% - var(--space-md))); }
}

.testimonial-track:hover {
    animation-play-state: paused;
}

.testimonial-card {
    flex-shrink: 0;
    width: 350px;
    background: white;
    padding: var(--space-lg);
    border-radius: var(--radius-lg);
    box-shadow: var(--shadow-soft);
    text-align: left;
}

.testimonial-stars {
    color: var(--color-gold);
    font-size: 1rem;
    margin-bottom: var(--space-sm);
    letter-spacing: 2px;
}

.testimonial-content p {
    color: var(--text-medium);
    font-style: italic;
    line-height: 1.7;
    margin-bottom: var(--space-md);
}

.testimonial-author {
    display: flex;
    align-items: center;
    gap: var(--space-sm);
}

.author-avatar {
    width: 45px;
    height: 45px;
    background: var(--gradient-primary);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    font-weight: 600;
    font-family: var(--font-display);
}

.author-name {
    display: block;
    font-weight: 500;
    color: var(--text-dark);
}

.author-detail {
    font-size: 0.8rem;
    color: var(--text-light);
}

/* ===================================
   SECCIÓN CTA / CONTACTO
   =================================== */
.cta-section {
    padding: var(--space-2xl) var(--space-lg);
    position: relative;
    overflow: hidden;
}

.cta-bg {
    position: absolute;
    inset: 0;
    z-index: -1;
}

.cta-gradient {
    position: absolute;
    inset: 0;
    background: linear-gradient(135deg, var(--color-primary) 0%, var(--color-secondary) 50%, var(--color-accent) 100%);
    opacity: 0.1;
}

.cta-pattern {
    position: absolute;
    inset: 0;
    background-image: 
        radial-gradient(circle at 20% 50%, var(--color-primary) 0%, transparent 50%),
        radial-gradient(circle at 80% 50%, var(--color-secondary) 0%, transparent 50%);
    opacity: 0.1;
}

.cta-container {
    max-width: 1200px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: var(--space-xl);
    align-items: center;
}

.cta-title {
    font-family: var(--font-display);
    font-size: clamp(2rem, 4vw, 3rem);
    font-weight: 500;
    line-height: 1.2;
    color: var(--text-dark);
    margin-bottom: var(--space-md);
}

.cta-text {
    color: var(--text-medium);
    margin-bottom: var(--space-lg);
    line-height: 1.7;
}

.cta-buttons {
    display: flex;
    flex-direction: column;
    gap: var(--space-sm);
}

.btn-whatsapp {
    background: #25D366;
    color: white;
    justify-content: center;
}

.btn-whatsapp:hover {
    background: #20BD5A;
    transform: translateY(-3px);
    box-shadow: 0 10px 30px rgba(37, 211, 102, 0.3);
}

.btn-instagram {
    background: linear-gradient(45deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888);
    color: white;
    justify-content: center;
}

.btn-instagram:hover {
    transform: translateY(-3px);
    box-shadow: 0 10px 30px rgba(225, 48, 108, 0.3);
}

.btn-icon {
    width: 20px;
    height: 20px;
}

/* Card CTA */
.cta-card {
    background: white;
    border-radius: var(--radius-lg);
    padding: var(--space-xl);
    box-shadow: var(--shadow-strong);
    text-align: center;
    position: relative;
    overflow: hidden;
}

.cta-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: var(--gradient-primary);
}

.cta-card-icon {
    font-size: 3rem;
    margin-bottom: var(--space-md);
}

.cta-card h3 {
    font-family: var(--font-display);
    font-size: 1.8rem;
    color: var(--text-dark);
    margin-bottom: var(--space-xs);
}

.cta-card p {
    color: var(--text-medium);
    margin-bottom: var(--space-md);
}

.cta-card-features {
    display: flex;
    flex-direction: column;
    gap: var(--space-xs);
}

.cta-card-features span {
    color: var(--text-medium);
    font-size: 0.9rem;
}

.cta-card-features span::before {
    color: var(--color-primary);
}

@media (max-width: 768px) {
    .cta-container {
        grid-template-columns: 1fr;
        text-align: center;
    }
    
    .cta-buttons {
        align-items: center;
    }
    
    .cta-buttons .btn {
        width: 100%;
        max-width: 300px;
    }
}

/* ===================================
   FOOTER
   =================================== */
.footer {
    background: var(--text-dark);
    color: white;
    padding: var(--space-xl) var(--space-lg) var(--space-lg);
}

.footer-container {
    max-width: 1200px;
    margin: 0 auto;
}

.footer-main {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-bottom: var(--space-lg);
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    margin-bottom: var(--space-lg);
}

.footer-logo {
    display: flex;
    align-items: center;
    gap: var(--space-xs);
}

.footer-logo .logo-icon {
    color: var(--color-primary);
}

.footer-logo .logo-text {
    font-family: var(--font-display);
    font-size: 1.5rem;
}

.footer-tagline {
    color: rgba(255, 255, 255, 0.6);
    margin-top: var(--space-xs);
    font-size: 0.9rem;
}

.footer-social-label {
    display: block;
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 0.15em;
    color: rgba(255, 255, 255, 0.5);
    margin-bottom: var(--space-sm);
}

.social-links {
    display: flex;
    gap: var(--space-sm);
}

.social-link {
    width: 45px;
    height: 45px;
    background: rgba(255, 255, 255, 0.1);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: var(--transition-normal);
}

.social-link svg {
    width: 20px;
    height: 20px;
    fill: white;
}

.social-link:hover {
    background: var(--color-primary);
    transform: translateY(-3px);
}

.footer-bottom {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: var(--space-sm);
}

.footer-copy {
    font-size: 0.85rem;
    color: rgba(255, 255, 255, 0.5);
}

.footer-quote {
    font-family: var(--font-display);
    font-style: italic;
    color: rgba(255, 255, 255, 0.4);
    font-size: 0.9rem;
}

@media (max-width: 768px) {
    .footer-main {
        flex-direction: column;
        text-align: center;
        gap: var(--space-lg);
    }
    
    .footer-bottom {
        flex-direction: column;
        text-align: center;
    }
}

/* ===================================
   ANIMACIONES DE REVEAL
   =================================== */
.reveal-up,
.reveal-left,
.reveal-scale {
    opacity: 0;
    transition: opacity 0.8s ease, transform 0.8s ease;
}

.reveal-up {
    transform: translateY(30px);
}

.reveal-left {
    transform: translateX(-30px);
}

.reveal-scale {
    transform: scale(0.95);
}

.reveal-up.active,
.reveal-left.active,
.reveal-scale.active {
    opacity: 1;
    transform: translateY(0) translateX(0) scale(1);
}

/* Delays */
.delay-1 { transition-delay: 0.1s; }
.delay-2 { transition-delay: 0.2s; }
.delay-3 { transition-delay: 0.3s; }
.delay-4 { transition-delay: 0.4s; }
.delay-5 { transition-delay: 0.5s; }
.delay-6 { transition-delay: 0.6s; }

/* Animación de entrada inicial */
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

/* ===================================
   UTILIDADES
   =================================== */
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 var(--space-lg);
}

/* Scrollbar personalizada */
::-webkit-scrollbar {
    width: 10px;
}

::-webkit-scrollbar-track {
    background: var(--bg-light);
}

::-webkit-scrollbar-thumb {
    background: var(--color-primary);
    border-radius: var(--radius-full);
}

::-webkit-scrollbar-thumb:hover {
    background: var(--color-secondary);
}
