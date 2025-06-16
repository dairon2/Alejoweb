<!DOCTYPE html>
<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alejandro Mosquera | Contador Público</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts: Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">

    <!-- Estilos personalizados y Animaciones -->
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc; /* gris claro */
            color: #1f2947; /* gris oscuro */
        }


        .animate-on-scroll {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease-out, transform 0.6s ease-out;
        }

        .animate-on-scroll.is-visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Estilo para el header al hacer scroll */
        .header-scrolled {
            background-color: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
            box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
        }
        
        /* Iconos para redes sociales (ejemplo) */
        .social-icon svg {
            width: 24px;
            height: 24px;
            transition: transform 0.3s ease;
        }
        .social-icon:hover svg {
            transform: scale(1.2);
        }
    </style>
</head>
<body class="antialiased">

    <!-- Encabezado y Navegación -->
    <header id="main-header" class="fixed top-0 left-0 right-0 z-50 transition-all duration-300">
        <div class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-xl md:text-2xl font-bold text-gray-800">Alejandro Mosquera</a>
            <nav class="hidden md:flex space-x-8">
                <a href="#servicios" class="text-gray-600 hover:text-blue-600 transition-colors">Servicios</a>
                <a href="#auditorias" class="text-gray-600 hover:text-blue-600 transition-colors">Auditorías</a>
                <a href="#contacto" class="text-gray-600 hover:text-blue-600 transition-colors">Contacto</a>
            </nav>
            <a href="#contacto" class="hidden md:inline-block bg-blue-600 text-white font-semibold px-5 py-2 rounded-lg shadow-md hover:bg-blue-700 transition-all transform hover:scale-105">
                Contactar
            </a>
            <!-- Menú hamburguesa para móviles -->
            <button id="mobile-menu-button" class="md:hidden text-gray-700">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
            </button>
        </div>
        <!-- Menú móvil desplegable -->
        <div id="mobile-menu" class="hidden md:hidden bg-white px-6 pb-4">
             <a href="#servicios" class="block py-2 text-gray-600 hover:text-blue-600">Servicios</a>
             <a href="#auditorias" class="block py-2 text-gray-600 hover:text-blue-600">Auditorías</a>
             <a href="#contacto" class="block py-2 text-gray-600 hover:text-blue-600">Contacto</a>
             <a href="#contacto" class="block mt-4 w-full text-center bg-blue-600 text-white font-semibold px-5 py-2 rounded-lg shadow-md hover:bg-blue-700">Contactar</a>
        </div>
    </header>

    <main>
        <!-- Sección Héroe -->
        <section id="hero" class="bg-white pt-32 pb-20 md:pt-40 md:pb-28">
            <div class="container mx-auto px-6 text-center">
                <div class="animate-on-scroll">
                    <h1 class="text-4xl md:text-6xl font-bold text-gray-800 leading-tight mb-2">ALEJANDRO MOSQUERA</h1>
                    <p class="text-2xl md:text-3xl font-semibold text-blue-600 mb-6">CONTADOR PÚBLICO</p>
                    <p class="text-lg md:text-xl text-gray-600 max-w-3xl mx-auto mb-8">"Ofrecemos oportunidades más brillantes"</p>
                    <a href="#servicios" class="bg-blue-600 text-white font-bold px-8 py-4 rounded-lg shadow-xl hover:bg-blue-700 transition-all transform hover:scale-105 inline-block">
                        Conoce Nuestros Servicios
                    </a>
                </div>
            </div>
        </section>

        <!-- Sección de Servicios -->
        <section id="servicios" class="py-20 bg-gray-50">
            <div class="container mx-auto px-6">
                <div class="text-center mb-16 animate-on-scroll">
                    <h2 class="text-3xl md:text-4xl font-bold text-gray-800">Portafolio de Servicios</h2>
                    <p class="text-lg text-gray-600 mt-2 max-w-3xl mx-auto">Nuestra completa oferta en contabilidad, finanzas, tributación y auditoría, diseñada para brindarle soluciones efectivas y personalizadas.</p>
                </div>
                
                <!-- Servicios Contables y Administrativos -->
                <div class="mb-16">
                    <h3 class="text-2xl md:text-3xl font-bold text-gray-800 mb-8 text-center animate-on-scroll">Servicios Contables y Administrativos</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                        <!-- Asesoría contable -->
                        <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl transition-shadow duration-300 animate-on-scroll transform hover:-translate-y-2">
                            <h4 class="text-xl font-bold mb-3">Asesoría contable</h4>
                            <p class="text-gray-600">Somos su aliado para resolver cualquier inquietud sobre el proceso contable mensual de su empresa, garantizando el cumplimiento de normativas y mejores prácticas.</p>
                        </div>
                        <!-- Outsourcing contable -->
                        <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl transition-shadow duration-300 animate-on-scroll transform hover:-translate-y-2" style="transition-delay: 100ms;">
                            <h4 class="text-xl font-bold mb-3">Outsourcing contable</h4>
                            <p class="text-gray-600">Equipo altamente capacitado y recursos tecnológicos de vanguardia para gestionar sus operaciones contables diarias, asegurando un manejo eficiente y preciso.</p>
                        </div>
                        <!-- Tesorería -->
                        <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl transition-shadow duration-300 animate-on-scroll transform hover:-translate-y-2" style="transition-delay: 200ms;">
                            <h4 class="text-xl font-bold mb-3">Tesorería</h4>
                            <p class="text-gray-600">Gestionamos eficientemente los recursos financieros de su empresa, asegurando un control óptimo de ingresos, egresos y disponibilidad de fondos.</p>
                        </div>
                         <!-- Nómina -->
                        <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl transition-shadow duration-300 animate-on-scroll transform hover:-translate-y-2" style="transition-delay: 300ms;">
                            <h4 class="text-xl font-bold mb-3">Nómina</h4>
                            <p class="text-gray-600">Ofrecemos un manejo preciso y confiable del pago de salarios, garantizando el cumplimiento de normativas laborales y fiscales.</p>
                        </div>
                         <!-- Seguridad Social -->
                        <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl transition-shadow duration-300 animate-on-scroll transform hover:-translate-y-2" style="transition-delay: 400ms;">
                            <h4 class="text-xl font-bold mb-3">Seguridad Social</h4>
                            <p class="text-gray-600">Administramos y gestionamos las obligaciones de seguridad social, asegurando el bienestar y la tranquilidad de sus empleados.</p>
                        </div>
                    </div>
                </div>

                <!-- Servicios Tributarios -->
                <div>
                    <h3 class="text-2xl md:text-3xl font-bold text-gray-800 mb-8 text-center animate-on-scroll">Servicios Tributarios</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                        <!-- Consultoría tributaria -->
                        <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl transition-shadow duration-300 animate-on-scroll transform hover:-translate-y-2">
                            <h4 class="text-xl font-bold mb-3">Consultoría tributaria</h4>
                            <p class="text-gray-600">Brindamos asesoramiento experto para garantizar el cumplimiento de sus obligaciones fiscales de manera eficiente y oportuna.</p>
                        </div>
                        <!-- Planeación tributaria -->
                        <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl transition-shadow duration-300 animate-on-scroll transform hover:-translate-y-2" style="transition-delay: 100ms;">
                            <h4 class="text-xl font-bold mb-3">Planeación tributaria</h4>
                            <p class="text-gray-600">Diseñamos estrategias fiscales a la medida, permitiéndole optimizar su carga impositiva y mejorar la salud financiera de su empresa.</p>
                        </div>
                        <!-- Outsourcing tributario -->
                        <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl transition-shadow duration-300 animate-on-scroll transform hover:-translate-y-2" style="transition-delay: 200ms;">
                            <h4 class="text-xl font-bold mb-3">Outsourcing tributario</h4>
                            <p class="text-gray-600">Nos encargamos de la gestión integral de sus procesos tributarios, para que pueda enfocarse en el crecimiento de su negocio.</p>
                        </div>
                        <!-- Planeación patrimonial -->
                        <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl transition-shadow duration-300 animate-on-scroll transform hover:-translate-y-2 md:col-start-2" style="transition-delay: 300ms;">
                            <h4 class="text-xl font-bold mb-3">Planeación patrimonial</h4>
                            <p class="text-gray-600">Asesoramos a personas naturales en la estructuración societaria, financiera y fiscal de su patrimonio, asegurando su estabilidad y crecimiento.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Sección Auditorías Internas -->
        <section id="auditorias" class="py-20 bg-white">
            <div class="container mx-auto px-6">
                <div class="flex flex-col md:flex-row items-center gap-12">
                    <div class="md:w-1/2 animate-on-scroll">
                         <img src="https://placehold.co/600x450/e0f2fe/0ea5e9?text=Auditorías" alt="Imagen sobre auditorías y análisis financiero" class="rounded-xl shadow-xl w-full">
                    </div>
                    <div class="md:w-1/2 animate-on-scroll" style="transition-delay: 150ms;">
                        <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-6">Auditorías Internas</h2>
                        <ul class="space-y-4">
                            <li>
                                <h4 class="text-xl font-semibold text-gray-700">Análisis de estados financieros</h4>
                                <p class="text-gray-600">Evaluamos la situación económica de su empresa a través de un estudio detallado de sus estados financieros, facilitando la toma de decisiones estratégicas.</p>
                            </li>
                            <li>
                                <h4 class="text-xl font-semibold text-gray-700">Revisión de procedimientos</h4>
                                <p class="text-gray-600">Analizamos y optimizamos los procesos internos para garantizar mayor eficiencia, cumplimiento normativo y mejores prácticas operativas.</p>
                            </li>
                            <li>
                                <h4 class="text-xl font-semibold text-gray-700">Verificación de información contable</h4>
                                <p class="text-gray-600">Validamos la exactitud y confiabilidad de la información contable, asegurando su cumplimiento con los principios y normativas vigentes.</p>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- Sección Contacto -->
        <section id="contacto" class="py-20 bg-gray-50">
            <div class="container mx-auto px-6">
                <div class="text-center mb-12 animate-on-scroll">
                    <h2 class="text-3xl md:text-4xl font-bold text-gray-800">Contacto</h2>
                    <p class="text-lg text-gray-600 mt-2">¿Listo para empezar? ¡Hablemos!</p>
                </div>
                <div class="max-w-4xl mx-auto flex flex-col md:flex-row gap-8 md:gap-12">
                    <div class="md:w-1/2 bg-white p-8 md:p-10 rounded-xl shadow-2xl animate-on-scroll">
                        <h3 class="text-2xl font-bold mb-6">Envíanos un mensaje</h3>
                        <form id="contact-form">
                            <div class="mb-5">
                                <label for="name" class="block text-gray-700 font-semibold mb-2">Nombre</label>
                                <input type="text" id="name" name="name" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 transition" required>
                            </div>
                            <div class="mb-5">
                                <label for="email" class="block text-gray-700 font-semibold mb-2">Correo Electrónico</label>
                                <input type="email" id="email" name="email" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 transition" required>
                            </div>
                            <div class="mb-5">
                                <label for="message" class="block text-gray-700 font-semibold mb-2">Mensaje</label>
                                <textarea id="message" name="message" rows="4" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 transition" required></textarea>
                            </div>
                            <button type="submit" class="w-full bg-blue-600 text-white font-bold px-8 py-3 rounded-lg shadow-lg hover:bg-blue-700 transition-all transform hover:scale-105">
                                Enviar Mensaje
                            </button>
                        </form>
                        <div id="form-feedback" class="text-center mt-5"></div>
                    </div>
                     <div class="md:w-1/2 animate-on-scroll" style="transition-delay: 150ms;">
                        <div class="bg-white p-8 md:p-10 rounded-xl shadow-2xl h-full">
                            <h3 class="text-2xl font-bold mb-6">Información de Contacto</h3>
                            <div class="space-y-4 text-gray-700">
                                <p class="flex items-center">
                                    <svg class="w-6 h-6 mr-3 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path></svg>
                                    <span>304 203 0298</span>
                                </p>
                                 <p class="flex items-center">
                                    <svg class="w-6 h-6 mr-3 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path></svg>
                                    <span>300 319 4120</span>
                                </p>
                                <p class="flex items-center">
                                   <svg class="w-6 h-6 mr-3 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                                    <span>ALEJOM2003@GMAIL.COM</span>
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-6 text-center">
            <p class="text-2xl font-bold mb-4">Alejandro Mosquera</p>
            <div class="flex justify-center space-x-6 mb-8">
                <a href="#servicios" class="hover:text-blue-400 transition-colors">Servicios</a>
                <a href="#auditorias" class="hover:text-blue-400 transition-colors">Auditorías</a>
                <a href="#contacto" class="hover:text-blue-400 transition-colors">Contacto</a>
            </div>
            <p class="text-gray-400 text-sm">&copy; <span id="year"></span> Alejandro Mosquera. Todos los derechos reservados.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // --- Animaciones al hacer scroll ---
            const observer = new IntersectionObserver(entries => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('is-visible');
                    }
                });
            }, {
                threshold: 0.1
            });

            document.querySelectorAll('.animate-on-scroll').forEach(element => {
                observer.observe(element);
            });

            // --- Lógica del menú móvil ---
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });
            
            mobileMenu.querySelectorAll('a').forEach(link => {
                link.addEventListener('click', () => {
                    mobileMenu.classList.add('hidden');
                });
            });

            // --- Estilo del header al hacer scroll ---
            const header = document.getElementById('main-header');
            window.addEventListener('scroll', () => {
                if (window.scrollY > 50) {
                    header.classList.add('header-scrolled');
                } else {
                    header.classList.remove('header-scrolled');
                }
            });

            // --- Formulario de contacto ---
            const contactForm = document.getElementById('contact-form');
            const formFeedback = document.getElementById('form-feedback');
            contactForm.addEventListener('submit', function(e) {
                e.preventDefault();
                
                formFeedback.textContent = 'Enviando...';
                formFeedback.className = 'text-blue-600';
                
                setTimeout(() => {
                    formFeedback.textContent = '¡Gracias! Su mensaje ha sido enviado.';
                    formFeedback.className = 'text-green-600 font-semibold';
                    contactForm.reset();
                }, 1500);
            });

            // --- Actualizar año en el footer ---
            document.getElementById('year').textContent = new Date().getFullYear();
        });
    </script>
</body>
</html>
