[index.html](https://github.com/user-attachments/files/33308290/index.html)
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agencia ADEN | Estrategia, Web, Redes e Inteligencia Artificial</title>
    <style>
        :root {
            --primary: #0f172a;
            --accent: #2563eb;
            --accent-hover: #1d4ed8;
            --whatsapp: #25d366;
            --bg-light: #f8fafc;
            --text-main: #334155;
            --text-light: #64748b;
            --white: #ffffff;
            --border: #e2e8f0;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
        }

        body {
            background-color: var(--bg-light);
            color: var(--text-main);
            line-height: 1.6;
        }

        header {
            background-color: var(--white);
            border-bottom: 1px solid var(--border);
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 800;
            color: var(--primary);
            text-decoration: none;
        }

        .logo span {
            color: var(--accent);
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-main);
            font-weight: 600;
            transition: color 0.2s;
        }

        .nav-links a:hover {
            color: var(--accent);
        }

        /* HERO SECTION */
        .hero {
            background: linear-gradient(135deg, var(--primary) 0%, #1e293b 100%);
            color: var(--white);
            padding: 6rem 2rem;
            text-align: center;
        }

        .hero-container {
            max-width: 900px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 3rem;
            font-weight: 800;
            margin-bottom: 1.5rem;
            line-height: 1.2;
        }

        .hero h1 span {
            color: #60a5fa;
        }

        .hero p {
            font-size: 1.25rem;
            color: #94a3b8;
            margin-bottom: 2.5rem;
            max-width: 750px;
            margin-left: auto;
            margin-right: auto;
        }

        .hero-buttons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 0.85rem 2rem;
            font-size: 1rem;
            font-weight: 700;
            border-radius: 8px;
            text-decoration: none;
            transition: all 0.2s;
            cursor: pointer;
            text-align: center;
        }

        .btn-primary {
            background-color: var(--accent);
            color: var(--white);
        }

        .btn-primary:hover {
            background-color: var(--accent-hover);
            transform: translateY(-2px);
        }

        .btn-outline {
            background-color: transparent;
            color: var(--white);
            border: 2px solid #475569;
        }

        .btn-outline:hover {
            border-color: var(--white);
            background-color: rgba(255,255,255,0.05);
        }

        .hero-features {
            margin-top: 3rem;
            display: flex;
            justify-content: center;
            gap: 2rem;
            flex-wrap: wrap;
            font-size: 0.95rem;
            color: #cbd5e1;
        }

        /* SERVICES SECTION */
        .section {
            padding: 5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            font-size: 2.25rem;
            font-weight: 800;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .section-subtitle {
            text-align: center;
            color: var(--text-light);
            font-size: 1.1rem;
            margin-bottom: 4rem;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }

        .grid-4 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 2rem;
        }

        .card {
            background: var(--white);
            padding: 2.5rem 2rem;
            border-radius: 12px;
            border: 1px solid var(--border);
            box-shadow: 0 4px 6px -1px rgba(0,0,0,0.02);
            transition: transform 0.2s, box-shadow 0.2s;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(0,0,0,0.05);
        }

        .card-icon {
            font-size: 2.5rem;
            margin-bottom: 1.25rem;
        }

        .card h3 {
            font-size: 1.25rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 0.75rem;
        }

        .card p {
            color: var(--text-light);
            font-size: 0.95rem;
        }

        /* DEMOS SECTION */
        .demos-section {
            background-color: #f1f5f9;
        }

        .grid-3 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2rem;
        }

        .demo-card {
            background: var(--white);
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid var(--border);
            box-shadow: 0 4px 6px rgba(0,0,0,0.02);
            display: flex;
            flex-direction: column;
        }

        .demo-body {
            padding: 2rem;
            flex-grow: 1;
        }

        .demo-tag {
            display: inline-block;
            background-color: #dbeafe;
            color: #1e40af;
            font-size: 0.75rem;
            font-weight: 700;
            text-transform: uppercase;
            padding: 0.25rem 0.75rem;
            border-radius: 20px;
            margin-bottom: 1rem;
        }

        .demo-card h3 {
            font-size: 1.35rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 0.75rem;
        }

        .demo-card p {
            color: var(--text-light);
            font-size: 0.95rem;
            margin-bottom: 1.5rem;
        }

        .demo-footer {
            padding: 1.25rem 2rem;
            background-color: var(--bg-light);
            border-top: 1px solid var(--border);
        }

        .btn-demo {
            display: block;
            width: 100%;
            text-align: center;
            background-color: var(--primary);
            color: var(--white);
            padding: 0.75rem;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            transition: background 0.2s;
        }

        .btn-demo:hover {
            background-color: var(--accent);
        }

        /* PRICING SECTION */
        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 2rem;
        }

        .pricing-card {
            background: var(--white);
            border: 1px solid var(--border);
            border-radius: 12px;
            padding: 2.5rem 2rem;
            position: relative;
            display: flex;
            flex-direction: column;
        }

        .pricing-card.featured {
            border-color: var(--accent);
            box-shadow: 0 10px 25px -5px rgba(37,99,235,0.1);
        }

        .badge-featured {
            position: absolute;
            top: -12px;
            left: 50%;
            transform: translateX(-50%);
            background-color: var(--accent);
            color: var(--white);
            font-size: 0.75rem;
            font-weight: 700;
            padding: 0.25rem 1rem;
            border-radius: 20px;
            text-transform: uppercase;
        }

        .pricing-card h3 {
            font-size: 1.35rem;
            color: var(--primary);
            margin-bottom: 0.25rem;
            text-align: center;
        }

        .pricing-card .badge-plan {
            display: inline-block;
            margin: 0 auto 1rem;
            font-size: 0.75rem;
            font-weight: 700;
            text-transform: uppercase;
            padding: 0.2rem 0.6rem;
            border-radius: 4px;
            background: #e2e8f0;
            color: #475569;
            text-align: center;
        }

        .price-box {
            background: #f8fafc;
            border: 1px solid #f1f5f9;
            border-radius: 8px;
            padding: 1rem;
            margin-bottom: 1.5rem;
            text-align: center;
        }

        .price-option {
            font-size: 0.9rem;
            color: var(--text-main);
            margin-bottom: 0.25rem;
        }

        .price-option strong {
            font-size: 1.25rem;
            color: var(--primary);
        }

        .price-subtext {
            font-size: 0.75rem;
            color: var(--text-light);
        }

        .pricing-features {
            list-style: none;
            margin-bottom: 2rem;
            text-align: left;
            flex-grow: 1;
        }

        .pricing-features li {
            padding: 0.5rem 0;
            border-bottom: 1px solid var(--bg-light);
            font-size: 0.9rem;
            color: var(--text-main);
            display: flex;
            align-items: flex-start;
            gap: 0.5rem;
        }

        .pricing-features li::before {
            content: "✓";
            color: var(--accent);
            font-weight: bold;
        }

        /* FOOTER */
        footer {
            background-color: var(--primary);
            color: var(--white);
            padding: 4rem 2rem 2rem;
        }

        .footer-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 2rem;
            border-bottom: 1px solid #334155;
            padding-bottom: 3rem;
        }

        .footer-brand h2 {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
        }

        .footer-brand p {
            color: #94a3b8;
            font-size: 0.95rem;
        }

        .social-links {
            display: flex;
            gap: 1rem;
            align-items: center;
            flex-wrap: wrap;
        }

        .social-btn {
            background-color: #1e293b;
            color: var(--white);
            padding: 0.6rem 1.25rem;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.9rem;
            border: 1px solid #475569;
            transition: all 0.2s;
        }

        .social-btn:hover {
            background-color: var(--accent);
            border-color: var(--accent);
        }

        .footer-bottom {
            max-width: 1200px;
            margin: 2rem auto 0;
            text-align: center;
            color: #64748b;
            font-size: 0.85rem;
        }

        /* WHATSAPP FLOAT */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background-color: var(--whatsapp);
            color: var(--white);
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 30px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.3);
            z-index: 1000;
            transition: transform 0.2s;
            text-decoration: none;
        }

        .whatsapp-float:hover {
            transform: scale(1.1);
        }

        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.25rem;
            }
            .nav-links {
                display: none;
            }
            .footer-container {
                flex-direction: column;
                text-align: center;
            }
            .social-links {
                justify-content: center;
            }
        }
    </style>
</head>
<body>

    <!-- HEADER -->
    <header>
        <div class="nav-container">
            <a href="#" class="logo">AGENCIA <span>ADEN</span></a>
            <ul class="nav-links">
                <li><a href="#servicios">Servicios</a></li>
                <li><a href="#demos">Demos en Vivo</a></li>
                <li><a href="#precios">Planes y Precios</a></li>
            </ul>
            <a href="https://wa.me/573215467418?text=Hola,%20quisiera%20solicitar%20informacion%20sobre%20los%20servicios%20de%20Agencia%20ADEN" class="btn btn-primary" target="_blank">Hablar con un Asesor</a>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="hero">
        <div class="hero-container">
            <h1>Impulsamos tu Negocio con <span>Infraestructura Web, Redes e IA</span></h1>
            <p>Deja de perder clientes por una presencia digital obsoleta. En Agencia ADEN diseñamos tu sitio web profesional, gestionamos tus redes sociales y automatizamos tu agendamiento 24/7 para convertir visitas en ventas reales.</p>
            <div class="hero-buttons">
                <a href="#demos" class="btn btn-primary">Explorar Demos en Vivo 🚀</a>
                <a href="https://wa.me/573215467418?text=Hola,%20quisiera%20solicitar%20informacion%20sobre%20los%20servicios%20de%20Agencia%20ADEN" class="btn btn-outline" target="_blank">Hablar con un Asesor 💬</a>
            </div>
            <div class="hero-features">
                <span>✅ Diseño & Redes Sociales</span>
                <span>✅ Automatización e IA 24/7</span>
                <span>✅ Facilidades de Pago (Pago único o Suscripción Hotmart)</span>
            </div>
        </div>
    </section>

    <!-- 4 PILARES DE SERVICIO -->
    <section class="section" id="servicios">
        <h2 class="section-title">Nuestras Soluciones B2B</h2>
        <p class="section-subtitle">Ofrecemos un servicio integral adaptado a las necesidades de tu empresa, clínica o marca personal.</p>
        
        <div class="grid-4">
            <div class="card">
                <div class="card-icon">🌐</div>
                <h3>Infraestructura Web</h3>
                <p>Páginas web corporativas y landing pages de alta conversión, adaptadas a móviles y enfocadas en cerrar ventas y captar prospectos.</p>
            </div>
            <div class="card">
                <div class="card-icon">📲</div>
                <h3>Redes Sociales</h3>
                <p>Gestión estratégica, creación de contenido, branding y pauta publicitaria para conectar con tu audiencia en Instagram, Facebook y TikTok.</p>
            </div>
            <div class="card">
                <div class="card-icon">🤖</div>
                <h3>IA & Automatización</h3>
                <p>Embudos inteligentes conectados a WhatsApp que responden preguntas frecuentes y agendan citas automáticas las 24 horas del día.</p>
            </div>
            <div class="card">
                <div class="card-icon">🎨</div>
                <h3>Diseño & Eventos</h3>
                <p>Identidad corporativa, piezas publicitarias y experiencias digitales o impresas para eventos especiales y bodas.</p>
            </div>
        </div>
    </section>

    <!-- DEMOS EN VIVO -->
    <section class="section demos-section" id="demos">
        <h2 class="section-title">Galería de Demos en Vivo</h2>
        <p class="section-subtitle">Haz clic y prueba el estándar de calidad y velocidad que implementamos para nuestros clientes.</p>

        <div class="grid-3">
            <!-- Demo Odontología -->
            <div class="demo-card">
                <div class="demo-body">
                    <span class="demo-tag">Sector Salud</span>
                    <h3>Clínicas & Odontología</h3>
                    <p>Ecosistema web especializado para odontólogos y especialistas con catálogo de tratamientos y agendamiento directo.</p>
                </div>
                <div class="demo-footer">
                    <a href="https://demo-cl-nica-sonrisas-est-tica.vercel.app/" class="btn-demo" target="_blank">Probar Demo Odontología 🦷</a>
                </div>
            </div>

            <!-- Demo Estética -->
            <div class="demo-card">
                <div class="demo-body">
                    <span class="demo-tag">Belleza & Bienestar</span>
                    <h3>Centros de Estética</h3>
                    <p>Plataforma moderna diseñada para mostrar servicios de estética corporal, facial y reservas de citas en línea.</p>
                </div>
                <div class="demo-footer">
                    <a href="https://demo-estetica-aden.netlify.app/" class="btn-demo" target="_blank">Probar Demo Estética ✨</a>
                </div>
            </div>

            <!-- Demo Productos de Belleza -->
            <div class="demo-card">
                <div class="demo-body">
                    <span class="demo-tag">E-commerce / Retail</span>
                    <h3>Productos de Belleza</h3>
                    <p>Landing y catálogo interactivo optimizado para la venta de productos de belleza, cosmética y cuidado personal.</p>
                </div>
                <div class="demo-footer">
                    <a href="https://aura-skin-blush.vercel.app/" class="btn-demo" target="_blank">Probar Demo E-commerce 🛍️</a>
                </div>
            </div>

            <!-- Espacio Abogados -->
            <div class="demo-card">
                <div class="demo-body">
                    <span class="demo-tag">Servicios Profesionales</span>
                    <h3>Abogados & Consultorías</h3>
                    <p>Estructura enfocada en proyectar autoridad, confianza corporativa y captación de clientes institucionales.</p>
                </div>
                <div class="demo-footer">
                    <a href="https://wa.me/573215467418?text=Hola,%20me%20interesa%20la%20demo%20para%20abogados" class="btn-demo" target="_blank">Consultar Disponibilidad ⚖️</a>
                </div>
            </div>

            <!-- Espacio Paquete Eventos -->
            <div class="demo-card">
                <div class="demo-body">
                    <span class="demo-tag">Sociales & Bodas</span>
                    <h3>Paquete Eventos y Diseño</h3>
                    <p>Invitaciones digitales interactivas (web/PDF) y papelería física personalizada para bodas, grados y eventos.</p>
                </div>
                <div class="demo-footer">
                    <a href="https://wa.me/573215467418?text=Hola,%20me%20interesa%20solicitar%20informacion%20del%20paquete%20de%20eventos%20y%20tarjetas" class="btn-demo" target="_blank">Solicitar Información Eventos 💌</a>
                </div>
            </div>
        </div>
    </section>

    <!-- PRECIOS Y PLANES -->
    <section class="section" id="precios">
        <h2 class="section-title">Nuestros Paquetes Comerciales</h2>
        <p class="section-subtitle">Elige el paquete y la modalidad de pago que mejor se adapte a tu presupuesto (vía Hotmart en pago único diferible o suscripción mensual)[cite: 1, 2, 3].</p>

        <div class="pricing-grid">
            <!-- Plan 1 -->
            <div class="pricing-card">
                <div style="text-align: center;"><span class="badge-plan">Básico</span></div>
                <h3>Landing Exprés</h3>
                <div class="price-box">
                    <div class="price-option">Suscripción: <strong>$37 USD/mes</strong></div>
                    <div class="price-option">Pago único: <strong>$300 USD</strong></div>
                    <div class="price-subtext">(Diferible a cuotas con tarjeta de crédito)</div>
                </div>
                <ul class="pricing-features">
                    <li>1 página con diseño profesional[cite: 2]</li>
                    <li>Enfocada en agendar citas o contactos[cite: 2]</li>
                    <li>Botón directo a WhatsApp[cite: 2]</li>
                    <li>1 ronda de ajustes incluidos[cite: 2]</li>
                    <li>Ideal para iniciar presencia digital[cite: 2]</li>
                </ul>
                <a href="https://wa.me/573215467418?text=Hola,%20quisiera%20solicitar%20informacion%20sobre%20el%20paquete%20Landing%20Expres" class="btn btn-primary" target="_blank">Hablar con un Asesor</a>
            </div>

            <!-- Plan 2 -->
            <div class="pricing-card featured">
                <div class="badge-featured">Recomendado</div>
                <div style="text-align: center;"><span class="badge-plan" style="background:#dbeafe; color:#1e40af;">Institucional</span></div>
                <h3>Sitio Web Corporativo</h3>
                <div class="price-box">
                    <div class="price-option">Suscripción: <strong>$57 USD/mes</strong></div>
                    <div class="price-option">Pago único: <strong>$1,200 USD</strong></div>
                    <div class="price-subtext">(Diferible a cuotas con tarjeta de crédito)</div>
                </div>
                <ul class="pricing-features">
                    <li>Hasta 5 páginas (servicios, equipo, ubicación, etc.)[cite: 2]</li>
                    <li>Diseño institucional completo[cite: 2]</li>
                    <li>Integración con WhatsApp y redes sociales[cite: 2]</li>
                    <li>2 rondas de ajustes incluidos[cite: 2]</li>
                    <li>Ideal para negocios ya establecidos[cite: 2]</li>
                </ul>
                <a href="https://wa.me/573215467418?text=Hola,%20quisiera%20solicitar%20informacion%20sobre%20el%20paquete%20Sitio%20Web%20Corporativo" class="btn btn-primary" target="_blank">Hablar con un Asesor</a>
            </div>

            <!-- Plan 3 -->
            <div class="pricing-card">
                <div style="text-align: center;"><span class="badge-plan" style="background:#fef3c7; color:#92400e;">Escalabilidad PRO</span></div>
                <h3>Embudo + IA PRO</h3>
                <div class="price-box">
                    <div class="price-option">Suscripción: <strong>$77 USD/mes</strong></div>
                    <div class="price-option">Pago único: <strong>$3,500 USD</strong></div>
                    <div class="price-subtext">(Diferible a cuotas con tarjeta de crédito)</div>
                </div>
                <ul class="pricing-features">
                    <li>Todo lo del plan Corporativo[cite: 3]</li>
                    <li>Agente de IA en WhatsApp para agendar citas[cite: 3]</li>
                    <li>Automatización de seguimiento a clientes[cite: 3]</li>
                    <li>3 rondas de ajustes + 30 días de soporte[cite: 3]</li>
                    <li>Ideal para negocios que quieren escalar[cite: 3]</li>
                </ul>
                <a href="https://wa.me/573215467418?text=Hola,%20quisiera%20solicitar%20informacion%20sobre%20el%20paquete%20Embudo%20IA%20PRO" class="btn btn-primary" target="_blank">Hablar con un Asesor</a>
            </div>

            <!-- Plan 4 -->
            <div class="pricing-card">
                <div style="text-align: center;"><span class="badge-plan">Sociales & Bodas</span></div>
                <h3>Eventos & Diseño</h3>
                <div class="price-box">
                    <div class="price-option">Inversión: <strong>Desde $120k COP</strong></div>
                    <div class="price-subtext">(Paquetes a la medida según requerimiento)</div>
                </div>
                <ul class="pricing-features">
                    <li>Invitaciones digitales interactivas</li>
                    <li>Diseño de papelería para imprenta</li>
                    <li>Paquetes físicos de tarjetas de boda</li>
                    <li>Diseño 100% personalizado</li>
                </ul>
                <a href="https://wa.me/573215467418?text=Hola,%20quisiera%20solicitar%20informacion%20sobre%20el%20servicio%20de%20Eventos%20y%20Diseno" class="btn btn-primary" target="_blank">Solicitar Información</a>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <div class="footer-container">
            <div class="footer-brand">
                <h2>Agencia ADEN</h2>
                <p>Estrategia, Soluciones Digitales y Automatización con Visión Empresarial.</p>
            </div>
            <div class="footer-social-box">
                <p style="margin-bottom: 0.75rem; color: #cbd5e1; font-weight: 600;">¡Síguenos en nuestras redes sociales!</p>
                <div class="social-links">
                    <a href="https://www.linkedin.com/in/henrry-david-arroyo-lopez-97a874411" class="social-btn" target="_blank">LinkedIn</a>
                    <a href="https://www.facebook.com/share/1GiFomgXHG/" class="social-btn" target="_blank">Facebook</a>
                    <a href="https://www.instagram.com/aden_academia?igsi=M3VtZ21nNTV5cTBl" class="social-btn" target="_blank">Instagram</a>
                    <a href="https://www.tiktok.com/@adenacademia?_r=1&_t=ZS-9AHWPqMJree" class="social-btn" target="_blank">TikTok</a>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2026 Agencia ADEN — Todos los derechos reservados.</p>
        </div>
    </footer>

    <!-- BOTÓN FLOTANTE DE WHATSAPP -->
    <a href="https://wa.me/573215467418?text=Hola,%20quisiera%20solicitar%20informacion%20sobre%20los%20servicios%20de%20Agencia%20ADEN" class="whatsapp-float" target="_blank" title="Escríbenos por WhatsApp">
        💬
    </a>

</body>
</html>
