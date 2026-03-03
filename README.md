<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alex | Desarrollador Android</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Space+Grotesk:wght@500;600;700&display=swap" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Space+Grotesk:wght@500;600;700&display=swap');
        
        :root {
            --android-green: #3DDC84;
        }
        
        .tail-container {
            font-family: 'Inter', system-ui, sans-serif;
        }
        
        .logo-font {
            font-family: 'Space Grotesk', sans-serif;
        }

        .hero-bg {
            background: linear-gradient(135deg, #0a0a0a 0%, #111827 50%, #052e16 100%);
        }

        .android-glow {
            box-shadow: 0 0 40px -10px #3DDC84;
        }

        .card-hover {
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .card-hover:hover {
            transform: translateY(-12px) scale(1.03);
            box-shadow: 0 25px 50px -12px rgb(0 0 0 / 0.4);
        }

        .skill-bar {
            height: 6px;
            background: linear-gradient(to right, #3DDC84, #10b981);
            transition: width 1.5s ease-out;
        }
    </style>
</head>
<body class="tail-container bg-zinc-950 text-zinc-200 overflow-x-hidden">

    <!-- NAVBAR -->
    <nav class="fixed top-0 w-full bg-zinc-950/80 backdrop-blur-lg border-b border-zinc-800 z-50">
        <div class="max-w-7xl mx-auto px-6 py-5 flex items-center justify-between">
            <div class="flex items-center gap-3">
                <div class="w-9 h-9 bg-emerald-500 rounded-2xl flex items-center justify-center text-2xl shadow-lg android-glow">
                    🤖
                </div>
                <span class="logo-font text-2xl font-semibold tracking-tighter text-white">AlexDev</span>
            </div>
            
            <div class="hidden md:flex items-center gap-10 text-sm font-medium">
                <a href="#sobre" class="hover:text-emerald-400 transition-colors">Sobre mí</a>
                <a href="#habilidades" class="hover:text-emerald-400 transition-colors">Habilidades</a>
                <a href="#proyectos" class="hover:text-emerald-400 transition-colors">Proyectos</a>
                <a href="#contacto" class="hover:text-emerald-400 transition-colors">Contacto</a>
            </div>
            
            <a href="#contacto" 
               class="px-6 py-3 bg-emerald-500 hover:bg-emerald-600 text-black font-semibold rounded-2xl flex items-center gap-2 transition-all active:scale-95">
                <i class="fa-solid fa-paper-plane"></i>
                <span>Hablar conmigo</span>
            </a>
        </div>
    </nav>

    <!-- HERO -->
    <section class="hero-bg min-h-screen flex items-center pt-20">
        <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-2 gap-16 items-center">
            <div class="space-y-8">
                <div class="inline-flex items-center gap-2 px-5 py-2 bg-zinc-900 border border-emerald-500/30 rounded-3xl text-sm">
                    <div class="w-2 h-2 bg-emerald-500 rounded-full animate-pulse"></div>
                    Disponible para nuevos proyectos
                </div>
                
                <h1 class="text-6xl md:text-7xl font-bold leading-none logo-font tracking-tighter">
                    Hola, soy <span class="text-emerald-400">Alex</span><br>
                    Desarrollador<br>Android
                </h1>
                
                <p class="text-xl text-zinc-400 max-w-md">
                    Creo aplicaciones móviles rápidas, bonitas y escalables con Kotlin y Jetpack Compose. 
                    Apasionado por el Material You y las experiencias que enamoran a los usuarios.
                </p>
                
                <div class="flex flex-wrap gap-4">
                    <a href="#proyectos" 
                       class="px-8 py-4 bg-emerald-500 hover:bg-emerald-600 text-black font-semibold rounded-3xl flex items-center gap-3 group transition-all">
                        Ver mis apps
                        <i class="fa-solid fa-arrow-right group-active:rotate-45 transition-transform"></i>
                    </a>
                    
                    <a href="https://github.com/tuusuario" target="_blank"
                       class="px-8 py-4 border border-zinc-700 hover:border-emerald-500 hover:text-emerald-400 font-medium rounded-3xl flex items-center gap-3 transition-all">
                        <i class="fa-brands fa-github"></i>
                        GitHub
                    </a>
                </div>
                
                <div class="flex items-center gap-8 text-sm pt-6">
                    <div>
                        <div class="text-emerald-400 font-mono text-3xl font-bold">50+</div>
                        <div class="text-zinc-500">Apps publicadas</div>
                    </div>
                    <div>
                        <div class="text-emerald-400 font-mono text-3xl font-bold">4.9★</div>
                        <div class="text-zinc-500">Calificación Play Store</div>
                    </div>
                    <div>
                        <div class="text-emerald-400 font-mono text-3xl font-bold">8</div>
                        <div class="text-zinc-500">Países con usuarios</div>
                    </div>
                </div>
            </div>
            
            <!-- Imagen hero -->
            <div class="relative flex justify-center">
                <div class="relative">
                    <div class="absolute -inset-10 bg-emerald-500/10 rounded-[4rem] blur-3xl"></div>
                    <img src="https://picsum.photos/id/1015/600/620" 
                         alt="Alex - Desarrollador Android"
                         class="w-full max-w-[420px] rounded-3xl shadow-2xl border border-zinc-800 android-glow">
                    
                    <!-- Badge flotante -->
                    <div class="absolute -top-6 -right-6 bg-zinc-900 border border-emerald-500/50 px-6 py-3 rounded-3xl flex items-center gap-3 shadow-xl">
                        <div class="text-4xl">🚀</div>
                        <div>
                            <div class="font-semibold text-emerald-400">Android 15</div>
                            <div class="text-xs text-zinc-400">Listo para la nueva era</div>
                        </div>
                    </div>
                    
                    <!-- Android robot pequeño -->
                    <div class="absolute -bottom-8 -left-8 bg-zinc-900 p-4 rounded-3xl border border-zinc-700 flex items-center gap-3 shadow-xl">
                        <span class="text-5xl">🤖</span>
                        <div class="text-sm leading-tight">
                            <span class="font-mono text-emerald-400">Kotlin</span><br>
                            <span class="text-zinc-400">+ Jetpack Compose</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Scroll indicator -->
        <div class="absolute bottom-10 left-1/2 -translate-x-1/2 flex flex-col items-center gap-2 text-zinc-500 text-xs">
            <div class="w-px h-12 bg-gradient-to-b from-transparent via-emerald-500 to-transparent"></div>
            Desplázate
        </div>
    </section>

    <!-- SOBRE MÍ -->
    <section id="sobre" class="py-24 bg-zinc-900">
        <div class="max-w-5xl mx-auto px-6">
            <div class="grid md:grid-cols-12 gap-16 items-center">
                <div class="md:col-span-5">
                    <div class="sticky top-24">
                        <span class="text-emerald-400 text-sm font-mono tracking-widest">01 / QUIÉN SOY</span>
                        <h2 class="text-5xl font-bold logo-font tracking-tight mt-3 leading-none">
                            Android no es solo un trabajo,<br>es mi pasión
                        </h2>
                    </div>
                </div>
                
                <div class="md:col-span-7 space-y-8 text-lg text-zinc-300">
                    <p>
                        Soy Alex, desarrollador Android desde 2020. Nacido en Antioquia, Colombia 🇨🇴, he creado más de 15 aplicaciones 
                        que ya suman más de 180 mil descargas en Google Play.
                    </p>
                    <p>
                        Me especializo en arquitectura limpia, Jetpack Compose, Kotlin Multiplatform y Material 3 Design. 
                        Me encanta optimizar el rendimiento y crear interfaces que se sientan "vivas".
                    </p>
                    <div class="pt-6 flex gap-6">
                        <div class="flex items-center gap-4">
                            <div class="w-12 h-12 bg-emerald-900/50 rounded-2xl flex items-center justify-center text-3xl">📍</div>
                            <div>
                                <div class="font-medium">Medellín, Colombia</div>
                                <div class="text-sm text-zinc-500">UTC-5</div>
                            </div>
                        </div>
                        <div class="flex items-center gap-4">
                            <div class="w-12 h-12 bg-emerald-900/50 rounded-2xl flex items-center justify-center text-3xl">🌐</div>
                            <div>
                                <div class="font-medium">Abierto a remoto</div>
                                <div class="text-sm text-emerald-400">Worldwide</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- HABILIDADES -->
    <section id="habilidades" class="py-24">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <span class="text-emerald-400 text-sm font-mono tracking-widest">02 / TECNOLOGÍAS</span>
                <h2 class="text-5xl font-bold logo-font mt-3">Mi stack Android</h2>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Lenguajes -->
                <div class="bg-zinc-900 rounded-3xl p-8 card-hover">
                    <h3 class="flex items-center gap-3 text-xl font-semibold mb-8">
                        <i class="fa-solid fa-code text-emerald-400"></i>
                        Lenguajes & Core
                    </h3>
                    <div class="space-y-8">
                        <div>
                            <div class="flex justify-between text-sm mb-2">
                                <span>Kotlin</span>
                                <span class="text-emerald-400 font-mono">98%</span>
                            </div>
                            <div class="h-1 bg-zinc-800 rounded-full overflow-hidden">
                                <div class="skill-bar w-[98%]"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-sm mb-2">
                                <span>Java</span>
                                <span class="text-emerald-400 font-mono">85%</span>
                            </div>
                            <div class="h-1 bg-zinc-800 rounded-full overflow-hidden">
                                <div class="skill-bar w-[85%]"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-sm mb-2">
                                <span>Kotlin Multiplatform</span>
                                <span class="text-emerald-400 font-mono">75%</span>
                            </div>
                            <div class="h-1 bg-zinc-800 rounded-full overflow-hidden">
                                <div class="skill-bar w-[75%]"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Frameworks -->
                <div class="bg-zinc-900 rounded-3xl p-8 card-hover">
                    <h3 class="flex items-center gap-3 text-xl font-semibold mb-8">
                        <i class="fa-solid fa-layer-group text-emerald-400"></i>
                        Frameworks & Libraries
                    </h3>
                    <div class="grid grid-cols-2 gap-6 text-center">
                        <div class="bg-zinc-950 p-5 rounded-2xl">
                            <div class="text-4xl mb-3">🧩</div>
                            <div class="font-medium">Jetpack Compose</div>
                            <div class="text-xs text-emerald-400">Master</div>
                        </div>
                        <div class="bg-zinc-950 p-5 rounded-2xl">
                            <div class="text-4xl mb-3">📦</div>
                            <div class="font-medium">Room + Hilt</div>
                            <div class="text-xs text-emerald-400">Expert</div>
                        </div>
                        <div class="bg-zinc-950 p-5 rounded-2xl">
                            <div class="text-4xl mb-3">🌐</div>
                            <div class="font-medium">Retrofit + OkHttp</div>
                            <div class="text-xs text-emerald-400">Advanced</div>
                        </div>
                        <div class="bg-zinc-950 p-5 rounded-2xl">
                            <div class="text-4xl mb-3">🔥</div>
                            <div class="font-medium">Firebase</div>
                            <div class="text-xs text-emerald-400">Expert</div>
                        </div>
                    </div>
                </div>
                
                <!-- Herramientas -->
                <div class="bg-zinc-900 rounded-3xl p-8 card-hover">
                    <h3 class="flex items-center gap-3 text-xl font-semibold mb-8">
                        <i class="fa-solid fa-tools text-emerald-400"></i>
                        Herramientas favoritas
                    </h3>
                    <div class="flex flex-wrap gap-3">
                        <div class="bg-zinc-800 hover:bg-emerald-950 transition-colors px-6 py-3 rounded-2xl text-sm font-medium flex items-center gap-2">
                            <i class="fa-brands fa-android"></i> Android Studio
                        </div>
                        <div class="bg-zinc-800 hover:bg-emerald-950 transition-colors px-6 py-3 rounded-2xl text-sm font-medium flex items-center gap-2">
                            <i class="fa-solid fa-git-alt"></i> Git + GitHub
                        </div>
                        <div class="bg-zinc-800 hover:bg-emerald-950 transition-colors px-6 py-3 rounded-2xl text-sm font-medium flex items-center gap-2">
                            <i class="fa-solid fa-bolt"></i> Gradle KTS
                        </div>
                        <div class="bg-zinc-800 hover:bg-emerald-950 transition-colors px-6 py-3 rounded-2xl text-sm font-medium flex items-center gap-2">
                            <i class="fa-solid fa-cloud"></i> Firebase
                        </div>
                        <div class="bg-zinc-800 hover:bg-emerald-950 transition-colors px-6 py-3 rounded-2xl text-sm font-medium flex items-center gap-2">
                            <i class="fa-solid fa-chart-simple"></i> App Center
                        </div>
                        <div class="bg-zinc-800 hover:bg-emerald-950 transition-colors px-6 py-3 rounded-2xl text-sm font-medium flex items-center gap-2">
                            <i class="fa-solid fa-mobile-screen-button"></i> Figma → Compose
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- PROYECTOS -->
    <section id="proyectos" class="py-24 bg-zinc-900">
        <div class="max-w-7xl mx-auto px-6">
            <div class="flex justify-between items-end mb-12">
                <div>
                    <span class="text-emerald-400 text-sm font-mono tracking-widest">03 / TRABAJOS</span>
                    <h2 class="text-5xl font-bold logo-font mt-3">Proyectos destacados</h2>
                </div>
                <a href="https://github.com/tuusuario?tab=repositories" target="_blank"
                   class="text-sm flex items-center gap-2 hover:text-emerald-400 transition-colors">
                    Ver todos en GitHub <i class="fa-solid fa-arrow-up-right-from-square"></i>
                </a>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Proyecto 1 -->
                <div class="bg-zinc-950 rounded-3xl overflow-hidden card-hover">
                    <div class="h-56 bg-gradient-to-br from-emerald-900 to-teal-900 flex items-center justify-center text-8xl">
                        💰
                    </div>
                    <div class="p-8">
                        <div class="font-semibold text-xl mb-2">FinTrack - Finanzas personales</div>
                        <div class="text-zinc-400 text-sm mb-6 line-clamp-3">
                            App de control de gastos con gráficos animados, sincronización en tiempo real y modo oscuro automático.
                        </div>
                        <div class="flex flex-wrap gap-2">
                            <span class="text-xs bg-zinc-900 px-3 py-1 rounded-full">Kotlin</span>
                            <span class="text-xs bg-zinc-900 px-3 py-1 rounded-full">Compose</span>
                            <span class="text-xs bg-zinc-900 px-3 py-1 rounded-full">Room</span>
                            <span class="text-xs bg-zinc-900 px-3 py-1 rounded-full">Firebase</span>
                        </div>
                        <div class="flex gap-4 mt-8">
                            <a href="#" class="text-xs flex-1 text-center py-3 border border-emerald-500 text-emerald-400 hover:bg-emerald-500 hover:text-black rounded-2xl transition-colors">Play Store</a>
                            <a href="#" class="text-xs flex-1 text-center py-3 bg-white text-black rounded-2xl hover:bg-zinc-200 transition-colors">GitHub</a>
                        </div>
                    </div>
                </div>
                
                <!-- Proyecto 2 -->
                <div class="bg-zinc-950 rounded-3xl overflow-hidden card-hover">
                    <div class="h-56 bg-gradient-to-br from-purple-900 to-indigo-900 flex items-center justify-center text-8xl">
                        🏋️
                    </div>
                    <div class="p-8">
                        <div class="font-semibold text-xl mb-2">FitForge - Gimnasio personal</div>
                        <div class="text-zinc-400 text-sm mb-6 line-clamp-3">
                            Entrenamientos personalizados con IA, seguimiento de progreso y integración con Wear OS.
                        </div>
                        <div class="flex flex-wrap gap-2">
                            <span class="text-xs bg-zinc-900 px-3 py-1 rounded-full">Kotlin</span>
                            <span class="text-xs bg-zinc-900 px-3 py-1 rounded-full">Wear OS</span>
                            <span class="text-xs bg-zinc-900 px-3 py-1 rounded-full">ML Kit</span>
                        </div>
                        <div class="flex gap-4 mt-8">
                            <a href="#" class="text-xs flex-1 text-center py-3 border border-emerald-500 text-emerald-400 hover:bg-emerald-500 hover:text-black rounded-2xl transition-colors">Play Store</a>
                            <a href="#" class="text-xs flex-1 text-center py-3 bg-white text-black rounded-2xl hover:bg-zinc-200 transition-colors">GitHub</a>
                        </div>
                    </div>
                </div>
                
                <!-- Proyecto 3 -->
                <div class="bg-zinc-950 rounded-3xl overflow-hidden card-hover">
                    <div class="h-56 bg-gradient-to-br from-amber-900 to-orange-900 flex items-center justify-center text-8xl">
                        ☕
                    </div>
                    <div class="p-8">
                        <div class="font-semibold text-xl mb-2">CaféFinder - Mapa de cafeterías</div>
                        <div class="text-zinc-400 text-sm mb-6 line-clamp-3">
                            Descubre cafeterías cercanas con reseñas, menús y realidad aumentada para ver el interior.
                        </div>
                        <div class="flex flex-wrap gap-2">
                            <span class="text-xs bg-zinc-900 px-3 py-1 rounded-full">Kotlin</span>
                            <span class="text-xs bg-zinc-900 px-3 py-1 rounded-full">Maps SDK</span>
                            <span class="text-xs bg-zinc-900 px-3 py-1 rounded-full">ARCore</span>
                        </div>
                        <div class="flex gap-4 mt-8">
                            <a href="#" class="text-xs flex-1 text-center py-3 border border-emerald-500 text-emerald-400 hover:bg-emerald-500 hover:text-black rounded-2xl transition-colors">Play Store</a>
                            <a href="#" class="text-xs flex-1 text-center py-3 bg-white text-black rounded-2xl hover:bg-zinc-200 transition-colors">GitHub</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CONTACTO -->
    <section id="contacto" class="py-24 bg-black">
        <div class="max-w-3xl mx-auto px-6 text-center">
            <span class="text-emerald-400 text-sm font-mono tracking-widest">04 / ÚLTIMO PASO</span>
            <h2 class="text-5xl font-bold logo-font mt-4">¿Hacemos algo increíble juntos?</h2>
            <p class="mt-6 text-zinc-400 text-lg">
                Estoy disponible para freelance, proyectos full-time o simplemente charlar sobre Android.
            </p>
            
            <div class="mt-12 flex flex-col sm:flex-row gap-4 justify-center">
                <a href="mailto:tuemail@ejemplo.com" 
                   class="group px-10 py-6 bg-white text-black font-semibold text-xl rounded-3xl flex items-center justify-center gap-4 hover:scale-105 transition-transform">
                    <i class="fa-solid fa-envelope text-2xl group-hover:rotate-12 transition-transform"></i>
                    Envíame un correo
                </a>
                
                <a href="https://wa.me/573001234567" target="_blank"
                   class="px-10 py-6 border-2 border-emerald-500 hover:bg-emerald-500 hover:text-black font-semibold text-xl rounded-3xl flex items-center justify-center gap-4 transition-all">
                    <i class="fa-brands fa-whatsapp text-3xl"></i>
                    WhatsApp
                </a>
            </div>
            
            <div class="mt-16 flex justify-center gap-8 text-3xl text-zinc-600">
                <a href="https://github.com/tuusuario" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-github"></i></a>
                <a href="https://linkedin.com/in/tuusuario" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-linkedin"></i></a>
                <a href="https://twitter.com/tuusuario" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-x-twitter"></i></a>
                <a href="https://instagram.com/tuusuario" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-instagram"></i></a>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-zinc-950 border-t border-zinc-900 py-12">
        <div class="max-w-7xl mx-auto px-6 text-center text-zinc-500 text-sm">
            <div class="flex items-center justify-center gap-2">
                Hecho con <span class="text-red-500">❤️</span> y mucho Kotlin en Medellín
            </div>
            <div class="mt-2">© 2026 Alex • Todos los derechos reservados</div>
        </div>
    </footer>

    <script>
        // Tailwind script ya cargado via CDN
        
        // Animación suave al scroll para los skill bars
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.querySelectorAll('.skill-bar').forEach(bar => {
                        bar.style.width = bar.parentElement.nextElementSibling ? '0%' : bar.style.width; // ya tiene el width
                    });
                }
            });
        }, { threshold: 0.6 });
        
        document.querySelectorAll('#habilidades .bg-zinc-900').forEach(section => {
            observer.observe(section);
        });
        
        // Smooth scroll para los enlaces del nav
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                if (this.getAttribute('href') !== '#') {
                    e.preventDefault();
                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        console.log('%c✅ Página de Desarrollador Android lista! Personalízala con tus datos reales.', 'color:#3DDC84; font-family:monospace');
    </script>
</body>
</html>
