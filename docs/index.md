<!-- DISEÑO DEFINITIVO CON ENLACE DE DESCARGA CORREGIDO -->
<style>
  /* --- CONFIGURACIÓN Y ESTILOS --- */
  body { background-color: #f4f8fa !important; }
  header, footer { display: none !important; }

  /* ESTILOS PARA LA CAJA DEL ÍNDICE DE CINDER */
  nav[aria-label="Table of contents"] {
    background-color: white !important;
    padding: 20px !important; border: none !important;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
  }
  /* TEXTO DEL ÍNDICE EN ROJO */
  .bs-sidenav > li > a {
    color: #8E2430 !important;
  }
  .bs-sidenav > .active > a {
    color: #8E2430 !important;
    font-weight: bold !important;
    background-color: #f5f5f5 !important;
  }
  
  /* ESTILOS PARA TU DISEÑO PERSONALIZADO */
  .hero-header {
    background-color: #8E2430; color: white; text-align: center;
    padding: 50px 20px 80px 20px; border-bottom: 5px solid #7a1f29;
  }
  .hero-header img {
    width: 160px; height: 160px; border-radius: 50%;
    border: 4px solid white; box-shadow: 0 5px 15px rgba(0,0,0,0.2); object-fit: cover;
  }
  .hero-header h1 { color: white !important; margin: 20px 0 5px 0; font-size: 2.8em; font-weight: 600; }
  .hero-header h3 { color: #e0e0e0 !important; font-size: 1.3em !important; font-weight: 300; margin: 0; }
  .hero-header p { color: #e0e0e0; margin-top: 20px; font-size: 1.1em; }
  .hero-header a { color: white; text-decoration: none; border-bottom: 1px dotted #ffffff80; }

  /* CONTENEDOR PARA ALINEAR BOTÓN E ICONO HORIZONTALMENTE */
  .actions-container {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 25px; /* Espacio entre el icono y el botón */
    margin-top: 25px;
  }
  
  /* Estilos para el icono de GitHub */
  .social-icon {
    display: inline-block;
    border-bottom: none; /* Quitamos el subrayado punteado */
    transition: transform 0.2s ease-in-out;
  }
  .social-icon:hover {
    transform: translateY(-3px);
  }
  .social-icon svg {
    width: 32px;
    height: 32px;
    fill: white;
  }

  /* Estilos para el botón de descarga */
  .download-button {
    display: inline-block;
    padding: 12px 25px;
    border-radius: 25px;
    background-color: white;
    color: #8E2430 !important;
    font-weight: bold;
    text-decoration: none;
    border: none;
    cursor: pointer;
    transition: all 0.2s ease-in-out;
  }
  .download-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 10px rgba(0,0,0,0.2);
  }
  .download-button svg {
    width: 16px; height: 16px;
    margin-right: 8px; vertical-align: middle;
    fill: currentColor;
  }

  /* CLASE QUE AÑADIMOS CON JAVASCRIPT PARA CREAR LA TARJETA */
  .content-card-wrapper {
    background-color: white;
    max-width: 900px;
    margin: -50px auto 50px auto !important;
    border-radius: 8px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.1);
    padding: 2em 3em !important;
    position: relative; z-index: 10;
  }
  
  /* TÍTULOS DE LA PÁGINA (H3) EN ROJO */
  .content-card-wrapper h3 { 
    color: #8E2430 !important; 
    border-bottom: 2px solid #f0f0f0; 
    padding-bottom: 10px; 
    margin-top: 1.5em; 
    font-size: 1.6em !important; 
  }
  
  .content-card-wrapper h4 { color: #333 !important; }
  .content-card-wrapper p, .content-card-wrapper li { color: #333; }
  .custom-block { background-color: #f9fafb; border-left: 4px solid #8E2430; padding: 1em 1.5em; margin: 1.5em 0; border-radius: 4px; }
  .skill-pill { display: inline-block; background-color: #8E2430; color: #ffffff; padding: 8px 18px; border-radius: 20px; font-weight: 500; margin: 5px; }
</style>

<!-- 1. CABECERA ROJA (JavaScript la moverá a su sitio) -->
<div class="hero-header">
  <img src="img/foto-perfil.jpeg" alt="Foto de Oier Cadierno">
  <h1>Oier Cadierno Duñabeitia</h1>
  <h3>Técnico de Sistemas con especialización en IA y Big Data</h3>
  <p>
    <a href="mailto:oiercadierno@gmail.com">oiercadierno@gmail.com</a> &nbsp;|&nbsp;
    688899389 &nbsp;|&nbsp;
    Sestao, Bizkaia
  </p>

  <!-- Contenedor para alinear el botón y el icono -->
  <div class="actions-container">
    <!-- Icono de GitHub (¡Recuerda cambiar TU_USUARIO_AQUI!) -->
    <a href="https://github.com/oier-cadierno" class="social-icon" target="_blank" title="Perfil de GitHub">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12,2A10,10 0 0,0 2,12C2,16.42 4.87,20.17 8.84,21.5C9.34,21.58 9.5,21.27 9.5,21C9.5,20.77 9.5,20.14 9.5,19.31C6.73,19.91 6.14,17.97 6.14,17.97C5.68,16.81 5.03,16.5 5.03,16.5C4.12,15.88 5.1,15.9 5.1,15.9C6.1,15.97 6.63,16.93 6.63,16.93C7.5,18.45 8.97,18 9.54,17.73C9.63,17.11 9.89,16.67 10.17,16.42C7.95,16.17 5.62,15.31 5.62,11.5C5.62,10.39 6,9.5 6.65,8.79C6.55,8.54 6.2,7.5 6.75,6.15C6.75,6.15 7.59,5.88 9.5,7.17C10.29,6.95 11.15,6.84 12,6.84C12.85,6.84 13.71,6.95 14.5,7.17C16.41,5.88 17.25,6.15 17.25,6.15C17.8,7.5 17.45,8.54 17.35,8.79C18,9.5 18.38,10.39 18.38,11.5C18.38,15.32 16.04,16.16 13.83,16.41C14.17,16.72 14.5,17.33 14.5,18.26C14.5,19.6 14.5,20.68 14.5,21C14.5,21.27 14.66,21.59 15.17,21.5C19.14,20.16 22,16.42 22,12A10,10 0 0,0 12,2Z" /></svg>
    </a>
    
    <!--
      ===================================================================
      ==  LA CORRECCIÓN DEFINITIVA: RUTA ABSOLUTA AL PDF               ==
      ===================================================================
      La barra '/' al principio le dice al navegador que busque desde
      la raíz del sitio, lo que evita cualquier error de ruta.
    -->
    <a href="/files/CV-Oier-Cadierno.pdf" class="download-button" download="CV-Oier-Cadierno.pdf">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M19.35 10.04C18.67 6.59 15.64 4 12 4 9.11 4 6.6 5.64 5.35 8.04 2.34 8.36 0 10.91 0 14c0 3.31 2.69 6 6 6h13c2.76 0 5-2.24 5-5 0-2.64-2.05-4.78-4.65-4.96zM17 13l-5 5-5-5h3V9h4v4h3z"/></svg>
      Descargar CV
    </a>
  </div>

</div>

<!--
    ===================================================================
    ==  CONTENIDO EN MARKDOWN CON LOS NUEVOS TEXTOS                  ==
    ===================================================================
-->

### Resumen Profesional
<div class="custom-block">
<p align="justify" style="line-height: 1.7;">
Técnico de sistemas con especialización en IA y Big Data, apasionado por la automatización de infraestructuras y la resolución de problemas complejos. Busco activamente una oportunidad para unirme a un equipo innovador donde pueda aplicar mis habilidades en monitorización de sistemas y análisis de datos para mejorar la eficiencia y aportar valor desde el primer día.
</p>
</div>

---

### Experiencia Profesional
<div class="custom-block">
<h4><strong>Técnico HelpDesk</strong> | Satec <span style="float: right; font-style: italic; color: #666666; font-weight: 400;">(6 meses)</span></h4>
<ul><li>Gestioné un alto volumen de incidencias técnicas para clientes de Euskaltel, reduciendo el tiempo medio de resolución en un 10% mediante la optimización de protocolos de diagnóstico y manteniendo un índice de satisfacción superior al 95%.</li></ul>
<h4 style="margin-top: 1.5em;"><strong>Técnico de Mantenimiento</strong> | Mitae <span style="float: right; font-style: italic; color: #666666; font-weight: 400;">(3 meses)</span></h4>
<ul><li>Diagnostiqué y reparé más de 50 equipos informáticos, mejorando su rendimiento en un promedio del 20% a través de la optimización de software y la actualización de componentes clave.</li></ul>
</div>

---

### Formación Académica
<div class="custom-block">
<h4><strong>Máster en Inteligencia Artificial y Big Data</strong> <span style="float: right; font-style: italic; color: #666666; font-weight: 400;">(Finaliza en 2026)</span></h4>
<p style="margin-top: -10px;"><em>Centro de Formación Somorrostro</em></p>
<h4 style="margin-top: 1.5em;"><strong>Grado Superior en Administración de Sistemas Informáticos en Red</strong> <span style="float: right; font-style: italic; color: #666666; font-weight: 400;">(2024)</span></h4>
<p style="margin-top: -10px;"><em>Centro de Formación Somorrostro</em></p>
</div>

---

### Habilidades Técnicas
<div class="custom-block">
<div style="text-align: center;">
  <span class="skill-pill">Node-Red</span>
  <span class="skill-pill">Grafana</span>
  <span class="skill-pill">InfluxDB</span>
  <span class="skill-pill">Python</span>
  <span class="skill-pill">Administración de Redes</span>
  <span class="skill-pill">Bases de Datos</span>
</div>
</div>

---

### Información Adicional
<div class="custom-block">
<ul>
    <li><strong>Permiso de Conducir:</strong> Licencia tipo B y vehículo propio.</li>
    <li><strong>Idiomas:</strong> Castellano (Nativo), Euskera (Nivel B2), Inglés (Nivel B1).</li>
    <li><strong>Certificaciones (Taekwondo):</strong> Juez Cronometrador y Cinturón Negro 1º DAN.</li>
</ul>
</div>


<!--
    ===================================================================
    ==  EL SCRIPT QUE TRANSFORMA LA PÁGINA EN TU DISEÑO              ==
    ===================================================================
-->
<script>
  document.addEventListener("DOMContentLoaded", function() {
    const heroHeader = document.querySelector('.hero-header');
    const mdContent = document.querySelector('.md-content');
    const mainArea = document.querySelector('.md-main__inner');

    if (heroHeader && mdContent && mainArea) {
      // 1. Mover la cabecera roja para que esté al principio del área principal
      mainArea.insertBefore(heroHeader, mainArea.firstChild);

      // 2. Aplicar la clase 'content-card-wrapper' al contenedor del contenido
      // para convertirlo en la tarjeta blanca flotante.
      mdContent.classList.add('content-card-wrapper');
    }
  });
</script>