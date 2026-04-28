<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>4G Infinito | Internet Ilimitada no iPhone</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet"> 
    <style>
:root {
    --bg-color: #050507;
    --card-bg: rgba(21, 21, 24, 0.7);
    --card-border: rgba(255, 255, 255, 0.08);
    --primary-color: #00d2ff;
    --secondary-color: #7000ff;
    --accent-glow: rgba(112, 0, 255, 0.2);
    --text-main: #ffffff;
    --text-muted: #a0a0a5;
    --container-width: 1200px;
    --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: "Inter", sans-serif;
    background-color: var(--bg-color);
    color: var(--text-main);
    line-height: 1.6;
    overflow-x: hidden;
}

.container {
    max-width: var(--container-width);
    margin: 0 auto;
    padding: 0 24px;
}

/* Navbar */
.navbar {
    height: 90px;
    display: flex;
    align-items: center;
    border-bottom: 1px solid var(--card-border);
    position: sticky;
    top: 0;
    background: rgba(5, 5, 7, 0.85);
    backdrop-filter: blur(12px);
    z-index: 100;
}

.navbar .container {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 1.6rem;
    font-weight: 900;
    letter-spacing: -1.5px;
    cursor: default;
}

.logo span {
    background: linear-gradient(90deg, var(--primary-color), var(--secondary-color));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

/* Buttons */
.btn-primary {
    background: linear-gradient(90deg, var(--primary-color), var(--secondary-color));
    color: white;
    text-decoration: none;
    padding: 12px 28px;
    border-radius: 12px;
    font-weight: 700;
    transition: var(--transition);
    display: inline-block;
    border: none;
    text-align: center;
}

.btn-primary:hover {
    transform: translateY(-3px) scale(1.02);
    box-shadow: 0 15px 30px var(--accent-glow);
    filter: brightness(1.1);
}

.btn-primary.lg {
    padding: 20px 42px;
    font-size: 1.15rem;
    border-radius: 16px;
}

.btn-primary.full-width {
    width: 100%;
    margin-top: 20px;
}

/* Hero Section */
.hero {
    padding: 120px 0 80px;
    text-align: center;
    position: relative;
}

.hero::before {
    content: "";
    position: absolute;
    top: -150px;
    left: 50%;
    transform: translateX(-50%);
    width: 800px;
    height: 800px;
    background: radial-gradient(circle, var(--accent-glow) 0%, transparent 70%);
    z-index: -1;
    pointer-events: none;
}

.badge {
    display: inline-block;
    padding: 8px 20px;
    background: rgba(0, 210, 255, 0.08);
    border: 1px solid rgba(0, 210, 255, 0.15);
    color: var(--primary-color);
    border-radius: 100px;
    font-size: 0.9rem;
    font-weight: 700;
    margin-bottom: 32px;
}

.hero h1 {
    font-size: 4rem;
    font-weight: 900;
    line-height: 1.1;
    margin-bottom: 24px;
    letter-spacing: -3px;
}

.hero h1 span {
    color: var(--text-muted);
}

.hero p {
    font-size: 1.3rem;
    color: var(--text-muted);
    max-width: 650px;
    margin: 0 auto 48px;
}

.cta-note {
    font-size: 0.95rem;
    color: var(--text-muted);
    margin-top: 18px;
}

/* Sections */
.features, .pricing, .how-it-works, .compatibility {
    padding: 100px 0;
}

.section-title {
    text-align: center;
    margin-bottom: 70px;
}

.section-title h2 {
    font-size: 2.8rem;
    font-weight: 800;
    letter-spacing: -1.5px;
    margin-bottom: 16px;
}

.section-title h2 span {
    color: var(--primary-color);
}

.section-title p {
    color: var(--text-muted);
    font-size: 1.1rem;
}

/* Features Grid */
.features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 32px;
}

.feature-card {
    background: var(--card-bg);
    padding: 48px 32px;
    border-radius: 24px;
    border: 1px solid var(--card-border);
    backdrop-filter: blur(8px);
    transition: var(--transition);
}

.feature-card:hover {
    transform: translateY(-10px);
    border-color: var(--primary-color);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4);
}

.feature-card .icon {
    font-size: 2.5rem;
    margin-bottom: 24px;
}

.feature-card h3 {
    font-size: 1.4rem;
    margin-bottom: 14px;
    font-weight: 700;
}

.feature-card p {
    color: var(--text-muted);
    font-size: 1rem;
}

/* Pricing Section */
.pricing-grid {
    display: flex;
    justify-content: center;
    max-width: 500px;
    margin: 0 auto;
}

.pricing-card {
    background: linear-gradient(180deg, rgba(255, 255, 255, 0.05) 0%, rgba(255, 255, 255, 0.01) 100%);
    padding: 50px 40px;
    border-radius: 32px;
    border: 1px solid var(--card-border);
    position: relative;
    transition: var(--transition);
    width: 100%;
}

.pricing-card:hover {
    transform: scale(1.03);
    border-color: var(--secondary-color);
    box-shadow: 0 30px 60px rgba(0, 0, 0, 0.5), 0 0 20px var(--accent-glow);
}

.card-badge {
    position: absolute;
    top: -15px;
    left: 50%;
    transform: translateX(-50%);
    background: var(--secondary-color);
    color: white;
    padding: 6px 18px;
    border-radius: 50px;
    font-size: 0.8rem;
    font-weight: 800;
    letter-spacing: 1px;
}

.pricing-card h3 {
    font-size: 1.6rem;
    margin-bottom: 24px;
    text-align: center;
}

.price {
    text-align: center;
    margin-bottom: 40px;
}

.price .currency {
    font-size: 1.5rem;
    vertical-align: top;
    margin-right: 4px;
    font-weight: 600;
}

.price .amount {
    font-size: 4.5rem;
    font-weight: 900;
    line-height: 1;
}

.price .period {
    font-size: 1.1rem;
    color: var(--text-muted);
}

.plan-features {
    list-style: none;
    margin-bottom: 40px;
}

.plan-features li {
    margin-bottom: 16px;
    display: flex;
    align-items: center;
    gap: 12px;
    font-weight: 500;
}

.plan-features li .check {
    color: var(--primary-color);
    font-weight: 900;
    font-size: 1.2rem;
}

/* Compatibility */
.comp-box {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.03) 0%, rgba(255, 255, 255, 0.01) 100%);
    padding: 60px 40px;
    border-radius: 32px;
    border: 1px solid var(--card-border);
    text-align: center;
    transition: var(--transition);
}

.comp-box:hover {
    border-color: rgba(255, 255, 255, 0.15);
}

.operators {
    display: flex;
    justify-content: center;
    gap: 24px;
    margin-top: 32px;
    flex-wrap: wrap;
}

.op-card {
    padding: 16px 48px;
    border-radius: 16px;
    font-weight: 900;
    font-size: 1.4rem;
    transition: var(--transition);
    cursor: default;
}

.op-card:hover {
    transform: translateY(-5px) rotate(2deg);
    filter: brightness(1.2);
}

.op-card.vivo {
    background: #660099;
    box-shadow: 0 10px 20px rgba(102, 0, 153, 0.3);
}

.op-card.tim {
    background: #003399;
    box-shadow: 0 10px 20px rgba(0, 51, 153, 0.3);
}

/* How it Works */
.steps {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 48px;
    margin-top: 20px;
}

.step {
    text-align: center;
    transition: var(--transition);
    padding: 20px;
    border-radius: 24px;
}

.step:hover {
    background: rgba(255, 255, 255, 0.02);
}

.step-num {
    width: 60px;
    height: 60px;
    background: linear-gradient(45deg, var(--secondary-color), var(--primary-color));
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 24px;
    font-weight: 900;
    font-size: 1.5rem;
    transform: rotate(-10deg);
    transition: var(--transition);
}

.step:hover .step-num {
    transform: rotate(0deg) scale(1.1);
}

.step h4 {
    font-size: 1.3rem;
    margin-bottom: 12px;
}

.step p {
    color: var(--text-muted);
}

/* Footer */
.footer {
    padding: 80px 0;
    border-top: 1px solid var(--card-border);
    text-align: center;
}

.footer p {
    color: var(--text-muted);
    margin: 32px 0;
    font-size: 1rem;
}

.socials a {
    color: var(--primary-color);
    text-decoration: none;
    font-weight: 700;
    transition: var(--transition);
    padding-bottom: 2px;
    border-bottom: 2px solid transparent;
}

.socials a:hover {
    border-bottom-color: var(--primary-color);
}

/* Responsive */
@media (max-width: 992px) {
    .hero h1 {
        font-size: 3.2rem;
    }
}

@media (max-width: 768px) {
    .navbar {
        height: 80px;
    }
    
    .hero h1 {
        font-size: 2.8rem;
        letter-spacing: -2px;
    }

    .desktop-only {
        display: none;
    }

    .section-title h2 {
        font-size: 2.2rem;
    }

    .pricing-card {
        padding: 40px 24px;
    }
}


    </style>
</head>
<body>
    <header class="navbar">
        <div class="container">
            <div class="logo">4G <span>Infinito</span></div>
            <a href="https://wa.me/5513981083680?text=Olá! Vim pelo site e quero minha internet ilimitada." class="btn-primary desktop-only">Assinar Agora</a>
        </div>
    </header>

    <main>
        <section class="hero">
            <div class="container">
                <div class="hero-content">
                    <span class="badge">Conexão 5G Habilitada</span>
                    <h1>Internet Ilimitada no seu iPhone <span>sem Complicação.</span></h1>
                    <p>A melhor experiência de navegação ilimitada do Brasil. Sem limites, sem travar e direto no seu app.</p>
                    <div class="hero-actions">
                        <a href="#planos" class="btn-primary lg">Ver Planos Ilimitados</a>
                        <p class="cta-note">Ativação instantânea via App</p>
                    </div>
                </div>
            </div>
        </section>

        <section class="features">
            <div class="container">
                <div class="section-title">
                    <h2>Por que escolher o <span>4G Infinito?</span></h2>
                </div>
                <div class="features-grid">
                    <div class="feature-card">
                        <div class="icon">🚀</div>
                        <h3>Sem Travamentos</h3>
                        <p>Velocidade constante para vídeos, jogos e redes sociais sem interrupções.</p>     
                    </div>
                    <div class="feature-card">
                        <div class="icon">♾️</div>
                        <h3>Sem Limites</h3>
                        <p>Navegue o quanto quiser. Não reduzimos sua velocidade após o uso.</p>
                    </div>
                    <div class="feature-card">
                        <div class="icon">📱</div>
                        <h3>Via App</h3>
                        <p>Fácil instalação e configuração rápida diretamente pelo aplicativo.</p>        
                    </div>
                    <div class="feature-card">
                        <div class="icon">🎟️</div>
                        <h3>Sem Trocar Chip</h3>
                        <p>Mantenha seu chip atual e seu número. Funciona via configuração interna.</p>      
                    </div>
                </div>
            </div>
        </section>

        <section id="planos" class="pricing">
            <div class="container">
                <div class="section-title">
                    <h2>O Plano <span>Perfeito</span> para Você</h2>
                    <p>Transforme seu iPhone com conexão verdadeiramente ilimitada.</p>
                </div>
                
                <div class="pricing-grid">
                    <div class="pricing-card">
                        <div class="card-badge">MAIS VENDIDO</div>
                        <h3>Plano 4G/5G Infinito</h3>
                        <div class="price">
                            <span class="currency">R$</span>
                            <span class="amount">28,90</span>
                            <span class="period">/mês</span>
                        </div>
                        <ul class="plan-features">
                            <li><span class="check">✓</span> Internet 4G e 5G ilimitada</li>
                            <li><span class="check">✓</span> Funciona em qualquer iPhone</li>
                            <li><span class="check">✓</span> Sem trocar de chip</li>
                            <li><span class="check">✓</span> Sem travamentos ou redução</li>
                            <li><span class="check">✓</span> Configuração via app em minutos</li>
                            <li><span class="check">✓</span> Compatível com TIM e Vivo</li>
                            <li><span class="check">✓</span> Suporte rápido no WhatsApp</li>
                        </ul>
                        <a href="https://wa.me/5513981083680?text=Olá! Vim pelo site e quero minha internet ilimitada." class="btn-primary full-width">Assinar via WhatsApp</a>
                    </div>
                </div>
            </div>
        </section>

        <section class="compatibility">
            <div class="container">
                <div class="comp-box">
                    <p>Suporte total para as operadoras:</p>
                    <div class="operators">
                        <div class="op-card vivo">VIVO</div>
                        <div class="op-card tim">TIM</div>
                    </div>
                </div>
            </div>
        </section>

        <section class="how-it-works">
            <div class="container">
                <div class="section-title">
                    <h2>Como funciona?</h2>
                </div>
                <div class="steps">
                    <div class="step">
                        <div class="step-num">1</div>
                        <h4>Contato</h4>
                        <p>Entre em contato pelo WhatsApp</p>
                    </div>
                    <div class="step">
                        <div class="step-num">2</div>
                        <h4>Instalação</h4>
                        <p>Baixe nosso aplicativo exclusivo</p>
                    </div>
                    <div class="step">
                        <div class="step-num">3</div>
                        <h4>Navegação</h4>
                        <p>Navegue sem limites onde estiver</p>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <footer class="footer">
        <div class="container">
            <div class="logo">4G <span>Infinito</span></div>
            <p>© 2026 Todos os direitos reservados. Conexão segura e ilimitada.</p>
            <div class="socials">
                <a href="https://wa.me/5513981083680">Suporte WhatsApp</a>
            </div>
        </div>
    </footer>
</body>
</html>
