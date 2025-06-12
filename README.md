<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>YOSHITAKA - Dojo de Karate</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Custom styles for mobile menu */
        .mobile-menu {
            display: none;
        }
        .mobile-menu.active {
            display: block;
        }
        
        /* Custom animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .fade-in {
            animation: fadeIn 1s ease-out forwards;
        }
        
        /* Custom gradient for hero section */
        .hero-gradient {
            background: linear-gradient(135deg, rgba(0,0,0,0.8) 0%, rgba(100,0,0,0.7) 100%);
        }
    </style>
</head>
<body class="font-sans bg-gray-50">
    <!-- Header/Navigation -->
    <header class="fixed w-full bg-white shadow-md z-50">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center">
                <a href="#" class="flex items-center">
                    <div class="w-12 h-12 bg-red-600 rounded-full flex items-center justify-center mr-3">
                        <span class="text-white font-bold text-xl">Y</span>
                    </div>
                    <h1 class="text-2xl font-bold text-gray-800">YOSHITAKA</h1>
                </a>
            </div>
            
            <!-- Desktop Navigation -->
            <nav class="hidden md:flex space-x-8">
                <a href="#home" class="text-red-600 font-semibold hover:text-red-700 transition">Inicio</a>
                <a href="#about" class="text-gray-700 hover:text-red-600 transition">Nosotros</a>
                <a href="#classes" class="text-gray-700 hover:text-red-600 transition">Clases</a>
                <a href="#schedule" class="text-gray-700 hover:text-red-600 transition">Horarios</a>
                <a href="#instructors" class="text-gray-700 hover:text-red-600 transition">Instructores</a>
                <a href="#contact" class="text-gray-700 hover:text-red-600 transition">Contacto</a>
            </nav>
            
            <!-- Mobile menu button -->
            <button id="mobile-menu-button" class="md:hidden text-gray-700 focus:outline-none">
                <i class="fas fa-bars text-2xl"></i>
            </button>
        </div>
        
        <!-- Mobile Navigation -->
        <div id="mobile-menu" class="mobile-menu md:hidden bg-white w-full border-t">
            <div class="container mx-auto px-4 py-2 flex flex-col">
                <a href="#home" class="py-2 text-red-600 font-semibold">Inicio</a>
                <a href="#about" class="py-2 text-gray-700 hover:text-red-600">Nosotros</a>
                <a href="#classes" class="py-2 text-gray-700 hover:text-red-600">Clases</a>
                <a href="#schedule" class="py-2 text-gray-700 hover:text-red-600">Horarios</a>
                <a href="#instructors" class="py-2 text-gray-700 hover:text-red-600">Instructores</a>
                <a href="#contact" class="py-2 text-gray-700 hover:text-red-600">Contacto</a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="pt-24 pb-16 md:pt-32 md:pb-24 hero-gradient text-white">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-10 md:mb-0 fade-in">
                    <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-4">DOJO YOSHITAKA</h1>
                    <p class="text-xl mb-8">Disciplina, respeto y excelencia en el arte del Karate</p>
                    <div class="flex flex-wrap gap-4">
                        <a href="#classes" class="bg-red-600 hover:bg-red-700 text-white font-bold py-3 px-6 rounded-lg transition duration-300 transform hover:scale-105">
                            Ver Clases
                        </a>
                        <a href="#contact" class="bg-transparent border-2 border-white text-white font-bold py-3 px-6 rounded-lg transition duration-300 transform hover:scale-105 hover:bg-white hover:text-gray-800">
                            Contacto
                        </a>
                    </div>
                </div>
                <div class="md:w-1/2 flex justify-center fade-in" style="animation-delay: 0.3s;">
                    <img src="https://images.unsplash.com/photo-1565992441121-4367c2967103?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=627&q=80" 
                         alt="Karate Dojo" 
                         class="rounded-lg shadow-2xl max-w-md w-full">
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Sobre Nuestro Dojo</h2>
            
            <div class="flex flex-col md:flex-row items-center gap-8">
                <div class="md:w-1/2 mb-8 md:mb-0">
                    <img src="https://images.unsplash.com/photo-1594913615593-e4b8c44625be?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Dojo YOSHITAKA" 
                         class="rounded-lg shadow-lg w-full">
                </div>
                
                <div class="md:w-1/2">
                    <h3 class="text-2xl font-semibold mb-4 text-gray-800">Tradición y Modernidad</h3>
                    <p class="text-gray-600 mb-4">
                        Fundado en 1985, el Dojo YOSHITAKA ha formado generaciones de karatecas bajo los principios del respeto, disciplina y superación personal. 
                        Seguimos las enseñanzas tradicionales del Karate Shotokan, adaptándolas a la vida moderna.
                    </p>
                    <p class="text-gray-600 mb-6">
                        Nuestro dojo cuenta con instructores certificados por la Federación Internacional de Karate, garantizando una enseñanza de calidad 
                        tanto para principiantes como para avanzados.
                    </p>
                    
                    <div class="grid grid-cols-2 gap-4">
                        <div class="p-4 bg-red-50 rounded-lg">
                            <i class="fas fa-medal text-red-600 text-2xl mb-2"></i>
                            <h4 class="font-semibold">Más de 30 años</h4>
                            <p class="text-sm text-gray-600">De experiencia formando karatecas</p>
                        </div>
                        <div class="p-4 bg-red-50 rounded-lg">
                            <i class="fas fa-user-shield text-red-600 text-2xl mb-2"></i>
                            <h4 class="font-semibold">Instructores</h4>
                            <p class="text-sm text-gray-600">Certificados internacionalmente</p>
                        </div>
                        <div class="p-4 bg-red-50 rounded-lg">
                            <i class="fas fa-trophy text-red-600 text-2xl mb-2"></i>
                            <h4 class="font-semibold">Campeones</h4>
                            <p class="text-sm text-gray-600">Formamos competidores destacados</p>
                        </div>
                        <div class="p-4 bg-red-50 rounded-lg">
                            <i class="fas fa-heart text-red-600 text-2xl mb-2"></i>
                            <h4 class="font-semibold">Comunidad</h4>
                            <p class="text-sm text-gray-600">Ambiente familiar y de respeto</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Classes Section -->
    <section id="classes" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Nuestras Clases</h2>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Class 1 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden transition-transform duration-300 hover:scale-105 hover:shadow-xl">
                    <div class="h-48 bg-red-600 flex items-center justify-center">
                        <i class="fas fa-child text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Karate Infantil</h3>
                        <p class="text-gray-600 mb-4">Clases para niños de 5 a 12 años, enfocadas en disciplina, coordinación y valores.</p>
                        <ul class="text-sm text-gray-600 space-y-1 mb-4">
                            <li><i class="fas fa-check text-red-600 mr-2"></i> Lunes y Miércoles 16:00 - 17:00</li>
                            <li><i class="fas fa-check text-red-600 mr-2"></i> Grupos por edades</li>
                            <li><i class="fas fa-check text-red-600 mr-2"></i> Desarrollo psicomotor</li>
                        </ul>
                        <a href="#contact" class="text-red-600 font-medium hover:text-red-700">Más información →</a>
                    </div>
                </div>
                
                <!-- Class 2 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden transition-transform duration-300 hover:scale-105 hover:shadow-xl">
                    <div class="h-48 bg-red-700 flex items-center justify-center">
                        <i class="fas fa-user text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Karate Adultos</h3>
                        <p class="text-gray-600 mb-4">Para jóvenes y adultos a partir de 13 años. Técnica, katas y combate.</p>
                        <ul class="text-sm text-gray-600 space-y-1 mb-4">
                            <li><i class="fas fa-check text-red-600 mr-2"></i> Martes y Jueves 19:00 - 20:30</li>
                            <li><i class="fas fa-check text-red-600 mr-2"></i>Sábados 10:00 - 11:30</li>
                            <li><i class="fas fa-check text-red-600 mr-2"></i> Preparación para competencias</li>
                        </ul>
                        <a href="#contact" class="text-red-600 font-medium hover:text-red-700">Más información →</a>
                    </div>
                </div>
                
                <!-- Class 3 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden transition-transform duration-300 hover:scale-105 hover:shadow-xl">
                    <div class="h-48 bg-red-800 flex items-center justify-center">
                        <i class="fas fa-shield-alt text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Defensa Personal</h3>
                        <p class="text-gray-600 mb-4">Técnicas prácticas de autodefensa para situaciones reales.</p>
                        <ul class="text-sm text-gray-600 space-y-1 mb-4">
                            <li><i class="fas fa-check text-red-600 mr-2"></i> Viernes 18:00 - 19:30</li>
                            <li><i class="fas fa-check text-red-600 mr-2"></i> Para hombres y mujeres</li>
                            <li><i class="fas fa-check text-red-600 mr-2"></i> Sin necesidad de experiencia</li>
                        </ul>
                        <a href="#contact" class="text-red-600 font-medium hover:text-red-700">Más información →</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Schedule Section -->
    <section id="schedule" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Horarios</h2>
            
            <div class="overflow-x-auto">
                <table class="min-w-full bg-white rounded-lg overflow-hidden">
                    <thead>
                        <tr class="bg-red-600 text-white">
                            <th class="py-3 px-4 text-left">Clase</th>
                            <th class="py-3 px-4 text-left">Lunes</th>
                            <th class="py-3 px-4 text-left">Martes</th>
                            <th class="py-3 px-4 text-left">Miércoles</th>
                            <th class="py-3 px-4 text-left">Jueves</th>
                            <th class="py-3 px-4 text-left">Viernes</th>
                            <th class="py-3 px-4 text-left">Sábado</th>
                        </tr>
                    </thead>
                    <tbody class="divide-y divide-gray-200">
                        <tr>
                            <td class="py-3 px-4 font-medium">Infantil (5-8)</td>
                            <td class="py-3 px-4">16:00 - 17:00</td>
                            <td class="py-3 px-4">-</td>
                            <td class="py-3 px-4">16:00 - 17:00</td>
                            <td class="py-3 px-4">-</td>
                            <td class="py-3 px-4">-</td>
                            <td class="py-3 px-4">10:00 - 11:00</td>
                        </tr>
                        <tr class="bg-gray-50">
                            <td class="py-3 px-4 font-medium">Infantil (9-12)</td>
                            <td class="py-3 px-4">17:00 - 18:00</td>
                            <td class="py-3 px-4">-</td>
                            <td class="py-3 px-4">17:00 - 18:00</td>
                            <td class="py-3 px-4">-</td>
                            <td class="py-3 px-4">-</td>
                            <td class="py-3 px-4">11:00 - 12:00</td>
                        </tr>
                        <tr>
                            <td class="py-3 px-4 font-medium">Adultos Inicial</td>
                            <td class="py-3 px-4">19:00 - 20:30</td>
                            <td class="py-3 px-4">18:00 - 19:30</td>
                            <td class="py-3 px-4">19:00 - 20:30</td>
                            <td class="py-3 px-4">18:00 - 19:30</td>
                            <td class="py-3 px-4">19:30 - 21:00</td>
                            <td class="py-3 px-4">12:00 - 13:30</td>
                        </tr>
                        <tr class="bg-gray-50">
                            <td class="py-3 px-4 font-medium">Adultos Avanzado</td>
                            <td class="py-3 px-4">20:30 - 22:00</td>
                            <td class="py-3 px-4">19:30 - 21:00</td>
                            <td class="py-3 px-4">20:30 - 22:00</td>
                            <td class="py-3 px-4">19:30 - 21:00</td>
                            <td class="py-3 px-4">19:30 - 21:00</td>
                            <td class="py-3 px-4">13:30 - 15:00</td>
                        </tr>
                        <tr>
                            <td class="py-3 px-4 font-medium">Defensa Personal</td>
                            <td class="py-3 px-4">-</td>
                            <td class="py-3 px-4">-</td>
                            <td class="py-3 px-4">-</td>
                            <td class="py-3 px-4">-</td>
                            <td class="py-3 px-4">18:00 - 19:30</td>
                            <td class="py-3 px-4">15:00 - 16:30</td>
                        </tr>
                    </tbody>
                </table>
            </div>
            
            <div class="mt-8 text-center">
                <a href="#contact" class="bg-red-600 hover:bg-red-700 text-white font-bold py-3 px-8 rounded-lg inline-block transition duration-300 transform hover:scale-105">
                    ¡Inscríbete Ahora!
                </a>
            </div>
        </div>
    </section>

    <!-- Instructors Section -->
    <section id="instructors" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Nuestros Instructores</h2>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Instructor 1 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="h-64 bg-gray-200 overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1600180758890-6b94519e8dd6?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                             alt="Sensei Tanaka" 
                             class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-1">Sensei Hiroshi Tanaka</h3>
                        <p class="text-red-600 font-medium mb-3">7mo Dan - Fundador</p>
                        <p class="text-gray-600 mb-4">Con más de 40 años de experiencia, el Sensei Tanaka formó parte de la selección japonesa de Karate y ha entrenado a varios campeones nacionales.</p>
                        <div class="flex space-x-4">
                            <a href="#" class="text-gray-500 hover:text-red-600"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="text-gray-500 hover:text-red-600"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="text-gray-500 hover:text-red-600"><i class="fas fa-envelope"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Instructor 2 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="h-64 bg-gray-200 overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1594381898411-846e7d193883?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=687&q=80" 
                             alt="Sensei Martínez" 
                             class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-1">Sensei Carlos Martínez</h3>
                        <p class="text-red-600 font-medium mb-3">5to Dan - Instructor Principal</p>
                        <p class="text-gray-600 mb-4">Ex-campeón nacional en kata y kumite, especializado en la enseñanza para jóvenes y adultos con más de 15 años de experiencia docente.</p>
                        <div class="flex space-x-4">
                            <a href="#" class="text-gray-500 hover:text-red-600"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="text-gray-500 hover:text-red-600"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="text-gray-500 hover:text-red-600"><i class="fas fa-envelope"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Instructor 3 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="h-64 bg-gray-200 overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1573497491765-dccce02b29df?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=687&q=80" 
                             alt="Sempai Lucía" 
                             class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-1">Sempai Lucía Fernández</h3>
                        <p class="text-red-600 font-medium mb-3">3er Dan - Instructora</p>
                        <p class="text-gray-600 mb-4">Especialista en clases infantiles y defensa personal femenina. Psicóloga infantil con amplia experiencia en el desarrollo de habilidades a través del karate.</p>
                        <div class="flex space-x-4">
                            <a href="#" class="text-gray-500 hover:text-red-600"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="text-gray-500 hover:text-red-600"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="text-gray-500 hover:text-red-600"><i class="fas fa-envelope"></i></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Testimonios</h2>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Testimonial 1 -->
                <div class="bg-gray-50 p-6 rounded-lg shadow-md border-l-4 border-red-600">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/65.jpg" alt="María G." class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-semibold">María González</h4>
                            <p class="text-sm text-gray-500">Madre de alumno</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">
                        "El cambio en mi hijo ha sido increíble desde que empezó en YOSHITAKA. No solo aprende karate, sino valores y disciplina que aplica en casa y en la escuela."
                    </p>
                    <div class="mt-3 text-red-600">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="bg-gray-50 p-6 rounded-lg shadow-md border-l-4 border-red-600">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="José M." class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-semibold">José Martínez</h4>
                            <p class="text-sm text-gray-500">Alumno adulto</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">
                        "A los 40 años decidí comenzar karate y eligí YOSHITAKA. Los instructores son pacientes y adaptan las clases a tu nivel. En un año ya obtuve mi cinturón amarillo."
                    </p>
                    <div class="mt-3 text-red-600">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="bg-gray-50 p-6 rounded-lg shadow-md border-l-4 border-red-600">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Ana L." class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-semibold">Ana López</h4>
                            <p class="text-sm text-gray-500">Clase de defensa personal</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">
                        "Las clases de defensa personal me han dado mucha más confianza. La Sempai Lucía es increíble, explica técnicas prácticas en un ambiente de respeto y camaradería."
                    </p>
                    <div class="mt-3 text-red-600">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star-half-alt"></i>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Galería</h2>
            
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
                <div class="h-48 overflow-hidden rounded-lg hover:opacity-90 transition cursor-pointer">
                    <img src="https://images.unsplash.com/photo-1540206276207-3af25c08abc4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Clase de karate" 
                         class="w-full h-full object-cover">
                </div>
                <div class="h-48 overflow-hidden rounded-lg hover:opacity-90 transition cursor-pointer">
                    <img src="https://images.unsplash.com/photo-1565992441121-4367c2967103?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=627&q=80" 
                         alt="Katá en competición" 
                         class="w-full h-full object-cover">
                </div>
                <div class="h-48 overflow-hidden rounded-lg hover:opacity-90 transition cursor-pointer">
                    <img src="https://images.unsplash.com/photo-1526401722134-e62656b121e2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Niños en clase" 
                         class="w-full h-full object-cover">
                </div>
                <div class="h-48 overflow-hidden rounded-lg hover:opacity-90 transition cursor-pointer">
                    <img src="https://images.unsplash.com/photo-1600721391689-2564bb8055de?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80" 
                         alt="Premiación" 
                         class="w-full h-full object-cover">
                </div>
                <div class="h-48 overflow-hidden rounded-lg hover:opacity-90 transition cursor-pointer">
                    <img src="https://images.unsplash.com/photo-1594381898411-846e7d193883?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=687&q=80" 
                         alt="Entrenamiento individual" 
                         class="w-full h-full object-cover">
                </div>
                <div class="h-48 overflow-hidden rounded-lg hover:opacity-90 transition cursor-pointer">
                    <img src="https://images.unsplash.com/photo-1594913615593-e4b8c44625be?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Dojo" 
                         class="w-full h-full object-cover">
                </div>
                <div class="h-48 overflow-hidden rounded-lg hover:opacity-90 transition cursor-pointer">
                    <img src="https://images.unsplash.com/photo-1565995048260-7645f1ab8322?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Grupo meditando" 
                         class="w-full h-full object-cover">
                </div>
                <div class="h-48 overflow-hidden rounded-lg hover:opacity-90 transition cursor-pointer">
                    <img src="https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                         alt="Examen de grados" 
                         class="w-full h-full object-cover">
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 bg-red-600 text-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Contáctanos</h2>
            
            <div class="flex flex-col lg:flex-row gap-8">
                <div class="lg:w-1/2">
                    <h3 class="text-2xl font-semibold mb-4">Visítanos</h3>
                    <p class="mb-6">Estamos ubicados en el corazón de la ciudad, con amplias instalaciones y estacionamiento gratuito.</p>
                    
                    <div class="space-y-4">
                        <div class="flex items-start">
                            <i class="fas fa-map-marker-alt mt-1 mr-4"></i>
                            <div>
                                <h4 class="font-medium">Dirección</h4>
                                <p>Calle del Karate 123, Dojoville</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <i class="fas fa-phone-alt mt-1 mr-4"></i>
                            <div>
                                <h4 class="font-medium">Teléfono</h4>
                                <p>+123 456 7890</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <i class="fas fa-envelope mt-1 mr-4"></i>
                            <div>
                                <h4 class="font-medium">Email</h4>
                                <p>info@yoshitakadojo.com</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <i class="fas fa-clock mt-1 mr-4"></i>
                            <div>
                                <h4 class="font-medium">Horario de atención</h4>
                                <p>Lunes a Viernes: 15:00 - 22:00<br>Sábados: 9:00 - 17:00</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="mt-8">
                        <h3 class="text-2xl font-semibold mb-4">Síguenos</h3>
                        <div class="flex space-x-4 text-2xl">
                            <a href="#" class="hover:text-red-200 transition"><i class="fab fa-facebook"></i></a>
                            <a href="#" class="hover:text-red-200 transition"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="hover:text-red-200 transition"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="hover:text-red-200 transition"><i class="fab fa-whatsapp"></i></a>
                        </div>
                    </div>
                </div>
                
                <div class="lg:w-1/2 bg-white text-gray-800 rounded-lg p-6 shadow-xl">
                    <h3 class="text-2xl font-semibold mb-6 text-red-600">Formulario de contacto</h3>
                    <form id="contactForm">
                        <div class="mb-4">
                            <label for="name" class="block mb-2 font-medium">Nombre completo</label>
                            <input type="text" id="name" name="name" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-red-600" required>
                        </div>
                        <div class="mb-4">
                            <label for="email" class="block mb-2 font-medium">Correo electrónico</label>
                            <input type="email" id="email" name="email" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-red-600" required>
                        </div>
                        <div class="mb-4">
                            <label for="phone" class="block mb-2 font-medium">Teléfono</label>
                            <input type="tel" id="phone" name="phone" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-red-600">
                        </div>
                        <div class="mb-4">
                            <label for="class" class="block mb-2 font-medium">Interés en clase</label>
                            <select id="class" name="class" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-red-600">
                                <option value="">Seleccione una opción</option>
                                <option value="infantil">Karate Infantil</option>
                                <option value="adultos">Karate Adultos</option>
                                <option value="defensa">Defensa Personal</option>
                                <option value="otro">Otro</option>
                            </select>
                        </div>
                        <div class="mb-4">
                            <label for="message" class="block mb-2 font-medium">Mensaje</label>
                            <textarea id="message" name="message" rows="4" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-red-600"></textarea>
                        </div>
                        <button type="submit" class="w-full bg-red-600 hover:bg-red-700 text-white font-bold py-3 px-6 rounded-lg transition duration-300">
                            Enviar Mensaje
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-8">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-4 md:mb-0">
                    <a href="#" class="flex items-center">
                        <div class="w-10 h-10 bg-red-600 rounded-full flex items-center justify-center mr-3">
                            <span class="text-white font-bold text-lg">Y</span>
                        </div>
                        <h1 class="text-xl font-bold">YOSHITAKA</h1>
                    </a>
                    <p class="mt-2 text-gray-400">Karate Dojo desde 1985</p>
                </div>
                
                <div class="flex flex-wrap gap-6 justify-center">
                    <a href="#home" class="text-gray-400 hover:text-white transition">Inicio</a>
                    <a href="#about" class="text-gray-400 hover:text-white transition">Nosotros</a>
                    <a href="#classes" class="text-gray-400 hover:text-white transition">Clases</a>
                    <a href="#schedule" class="text-gray-400 hover:text-white transition">Horarios</a>
                    <a href="#instructors" class="text-gray-400 hover:text-white transition">Instructores</a>
                    <a href="#contact" class="text-gray-400 hover:text-white transition">Contacto</a>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-8 pt-6 text-center text-gray-500 text-sm">
                <p>© 2023 Dojo YOSHITAKA. Todos los derechos reservados.</p>
            </div>
        </div>
    </footer>

    <!-- Back to top button -->
    <button id="backToTop" class="fixed bottom-6 right-6 bg-red-600 text-white w-12 h-12 rounded-full shadow-lg flex items-center justify-center hover:bg-red-700 transition opacity-0 invisible">
        <i class="fas fa-arrow-up"></i>
    </button>

    <script>
        // Mobile menu toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            document.getElementById('mobile-menu').classList.toggle('active');
        });
        
        // Form submission
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            // Here you would typically send the form data to a server
            alert('Gracias por tu mensaje. Nos pondremos en contacto contigo pronto.');
            this.reset();
        });
        
        // Back to top button
        window.addEventListener('scroll', function() {
            const backToTopButton = document.getElementById('backToTop');
            if (window.pageYOffset > 300) {
                backToTopButton.classList.remove('opacity-0', 'invisible');
                backToTopButton.classList.add('opacity-100', 'visible');
            } else {
                backToTopButton.classList.remove('opacity-100', 'visible');
                backToTopButton.classList.add('opacity-0', 'invisible');
            }
        });
        
        document.getElementById('backToTop').addEventListener('click', function() {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
                
                // Close mobile menu if open
                document.getElementById('mobile-menu').classList.remove('active');
            });
        });
    </script>
</body>
</html>
