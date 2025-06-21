
AGENCIA DE VIAJES SAN ANDRÉS VIBES AND CHILL
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AGENCIA DE VIAJES SAN ANDRÉS VIBES AND CHILL</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    .carousel-item { display: none; }
    .carousel-item.active { display: block; }
  </style>
</head>
<body class="bg-white text-gray-800">

  <!-- Encabezado -->
  <header class="relative h-screen bg-cover bg-center" style="background-image: url('https://images.unsplash.com/photo-1608302690273-2b67e63a16a2');">
    <div class="bg-black bg-opacity-50 h-full flex flex-col justify-center items-center text-white text-center px-4">
      <h1 class="text-5xl font-bold mb-4">AGENCIA DE VIAJES<br>SAN ANDRÉS VIBES AND CHILL</h1>
      <p class="text-xl">Tu viaje soñado comienza aquí</p>
    </div>
  </header>

  <!-- Carrusel -->
  <section class="my-10 max-w-5xl mx-auto">
    <div class="relative">
      <div class="carousel-item active">
        <img src="https://images.unsplash.com/photo-1596896904024-f85f14cfc131" class="w-full h-96 object-cover rounded-xl">
      </div>
      <div class="carousel-item">
        <img src="https://images.unsplash.com/photo-1611601185386-d5abcf2f5e18" class="w-full h-96 object-cover rounded-xl">
      </div>
      <div class="carousel-item">
        <img src="https://images.unsplash.com/photo-1565639876335-91c02c9471f2" class="w-full h-96 object-cover rounded-xl">
      </div>
      <div class="absolute inset-0 flex justify-between items-center px-4">
        <button onclick="prevSlide()" class="bg-black bg-opacity-50 text-white p-2 rounded-full">⟨</button>
        <button onclick="nextSlide()" class="bg-black bg-opacity-50 text-white p-2 rounded-full">⟩</button>
      </div>
    </div>
  </section>

  <!-- Servicios -->
  <section class="bg-gray-100 py-10">
    <div class="text-center mb-8">
      <h2 class="text-3xl font-bold">Nuestros Servicios</h2>
    </div>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-6xl mx-auto px-4">
      <a href="paquetes.html" class="bg-white rounded-xl shadow-md p-6 hover:shadow-xl transition text-center">
        <h3 class="text-xl font-semibold mb-2">Paquetes Turísticos</h3>
        <p>Planes todo incluido para explorar San Andrés.</p>
      </a>
      <a href="hospedaje.html" class="bg-white rounded-xl shadow-md p-6 hover:shadow-xl transition text-center">
        <h3 class="text-xl font-semibold mb-2">Hospedaje</h3>
        <p>Hoteles, hostales y alojamientos a tu medida.</p>
      </a>
      <a href="tours.html" class="bg-white rounded-xl shadow-md p-6 hover:shadow-xl transition text-center">
        <h3 class="text-xl font-semibold mb-2">Tours y Actividades</h3>
        <p>Paseos, buceo, excursiones y experiencias únicas.</p>
      </a>
    </div>
  </section>

  <script>
    let slideIndex = 0;
    const slides = document.querySelectorAll('.carousel-item');

    function showSlide(index) {
      slides.forEach((slide, i) => {
        slide.classList.toggle('active', i === index);
      });
    }

    function nextSlide() {
      slideIndex = (slideIndex + 1) % slides.length;
      showSlide(slideIndex);
    }

    function prevSlide() {
      slideIndex = (slideIndex - 1 + slides.length) % slides.length;
      showSlide(slideIndex);
    }

    setInterval(nextSlide, 5000);
  </script>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Paquetes Turísticos</title>
</head>
<body>
  <h1>Paquetes Turísticos</h1>
  <p>Explora San Andrés con planes personalizados y todo incluido.</p>
  <a href="index.html">← Volver al inicio</a>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Hospedaje</title>
</head>
<body>
  <h1>Hospedaje</h1>
  <p>Reserva en los mejores hoteles, hostales y apartamentos de San Andrés.</p>
  <a href="index.html">← Volver al inicio</a>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Tours y Actividades</title>
</head>
<body>
  <h1>Tours y Actividades</h1>
  <p>Disfruta de snorkel, paseos en lancha, buceo y más aventuras en San Andrés.</p>
  <a href="index.html">← Volver al inicio</a>
</body>
</html>
