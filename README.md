!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Flores Dannas</title>
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background-color: #fffafc;
      color: #333;
    }
    header {
      background-color: #e05d8f;
      color: white;
      text-align: center;
      padding: 20px;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }
    section {
      padding: 30px;
      text-align: center;
    }
    h2 {
      color: #e05d8f;
      margin-bottom: 20px;
    }
    .catalogo {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
    }
    .producto {
      background-color: white;
      border-radius: 15px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      width: 250px;
      padding: 15px;
      transition: transform 0.2s;
    }
    .producto:hover {
      transform: scale(1.05);
    }
    .producto img {
      width: 100%;
      border-radius: 15px;
    }
    .boton {
      background-color: #e05d8f;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 8px;
      cursor: pointer;
      margin-top: 10px;
    }
    .boton:hover {
      background-color: #c94e7e;
    }
    footer {
      background-color: #e05d8f;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 30px;
    }
    form {
      max-width: 400px;
      margin: auto;
      display: flex;
      flex-direction: column;
      gap: 10px;
    }
    input, textarea {
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 8px;
      width: 100%;
    }
  </style>
</head>
<body>
  <header>
    <h1>🌸 Flores Dannas 🌸</h1>
    <nav>
      <a href="#inicio">Inicio</a>
      <a href="#catalogo">Catálogo</a>
      <a href="#contacto">Contacto</a>
    </nav>
  </header>

  <section id="inicio">
    <h2>Bienvenidos a Flores Dannas</h2>
    <p>Tu mejor opción para regalar amor, alegría y belleza natural. 💐</p>
  </section>

  <section id="catalogo">
    <h2>Nuestros Productos</h2>
    <div class="catalogo">
      <div class="producto">
        <img src="https://images.unsplash.com/photo-1509042239860-f550ce710b93" alt="Rosas rojas">
        <h3>Rosas Rojas</h3>
        <p>Ramo de 12 rosas rojas para ocasiones especiales.</p>
        <p><strong>Precio:</strong> Bs. 80</p>
        <button class="boton">Encargar</button>
      </div>

      <div class="producto">
        <img src="https://images.unsplash.com/photo-1587815070922-7c68b15a31c5" alt="Tulipanes">
        <h3>Tulipanes Amarillos</h3>
        <p>Perfectos para transmitir alegría y amistad.</p>
        <p><strong>Precio:</strong> Bs. 70</p>
        <button class="boton">Encargar</button>
      </div>

      <div class="producto">
        <img src="https://images.unsplash.com/photo-1615486364160-2c6b3e60e6f1" alt="Lirios">
        <h3>Lirios Blancos</h3>
        <p>Elegancia y pureza en un hermoso arreglo floral.</p>
        <p><strong>Precio:</strong> Bs. 90</p>
        <button class="boton">Encargar</button>
      </div>
    </div>
  </section>

  <section id="contacto">
    <h2>Contáctanos</h2>
    <p>¿Tienes un pedido especial? Escríbenos aquí 👇</p>
    <form onsubmit="enviarFormulario(event)">
      <input type="text" placeholder="Tu nombre" required>
      <input type="email" placeholder="Tu correo" required>
      <textarea rows="4" placeholder="Tu mensaje o pedido" required></textarea>
      <button class="boton" type="submit">Enviar mensaje</button>
    </form>
  </section>

  <footer>
    <p>© 2025 Flores Dannas | Todos los derechos reservados</p>
  </footer>

  <script>
    function enviarFormulario(e) {
      e.preventDefault();
      alert("¡Gracias por contactarte con Flores Dannas! 🌸 Te responderemos pronto.");
      e.target.reset();
    }
  </script>
</body>
