SeusFios
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FiosDeOuros - Cuidados Especiais para Cabelos</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;600;700&family=Great+Vibes&family=Libre+Baskerville:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            box-sizing: border-box;
        }
        
        .red-gradient-bg {
            background: linear-gradient(135deg, #fef2f2 0%, #fee2e2 30%, #fecaca 70%, #fca5a5 100%);
        }
        
        .elegant-serif {
            font-family: 'Cormorant Garamond', serif;
        }
        
        .script-elegant {
            font-family: 'Great Vibes', cursive;
        }
        
        .classic-serif {
            font-family: 'Libre Baskerville', serif;
        }
        
        .card-hover {
            transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .card-hover:hover {
            transform: translateY(-12px) scale(1.03);
            box-shadow: 0 30px 60px -12px rgba(220, 38, 38, 0.3);
        }
        
        .fade-in {
            animation: fadeInUp 1.2s ease-out;
        }
        
        @keyframes fadeInUp {
            from { 
                opacity: 0; 
                transform: translateY(40px);
            }
            to { 
                opacity: 1; 
                transform: translateY(0);
            }
        }
        
        .floating-gentle {
            animation: floatingGentle 4s ease-in-out infinite;
        }
        
        @keyframes floatingGentle {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-8px) rotate(1deg); }
        }
        
        .text-shadow-elegant {
            text-shadow: 3px 3px 6px rgba(220, 38, 38, 0.2);
        }
        
        .red-border-elegant {
            border: 3px solid rgba(220, 38, 38, 0.3);
            border-radius: 20px;
        }
        
        .gradient-text-red {
            background: linear-gradient(45deg, #dc2626, #ef4444, #f87171, #fca5a5);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .hair-image {
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(220, 38, 38, 0.2);
        }
        
        .overlay-red {
            background: linear-gradient(45deg, rgba(220, 38, 38, 0.1), rgba(239, 68, 68, 0.1));
        }
    </style>
</head>
<body class="red-gradient-bg min-h-screen">
    <!-- Header -->
    <header class="bg-white/80 backdrop-blur-lg shadow-xl sticky top-0 z-50 red-border-elegant border-t-0 border-l-0 border-r-0">
        <nav class="container mx-auto px-8 py-6">
            <div class="flex items-center justify-between">
                <div class="flex items-center space-x-5">
                    <div class="w-14 h-14 bg-gradient-to-br from-red-300 to-red-500 rounded-full flex items-center justify-center floating-gentle shadow-lg">
                        <span class="text-4xl">👑</span>
                    </div>
                    <h1 class="text-4xl font-bold text-red-800 script-elegant text-shadow-elegant">FiosDeOuros</h1>
                </div>
                <div class="hidden md:flex space-x-10">
                    <a href="#home" class="text-red-700 hover:text-red-900 transition-colors classic-serif text-lg font-bold">Início</a>
                    <a href="#servicos" class="text-red-700 hover:text-red-900 transition-colors classic-serif text-lg font-bold">Serviços</a>
                    <a href="#tratamentos" class="text-red-700 hover:text-red-900 transition-colors classic-serif text-lg font-bold">Tratamentos</a>
                    <a href="#galeria" class="text-red-700 hover:text-red-900 transition-colors classic-serif text-lg font-bold">Galeria</a>
                </div>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="py-28 px-8">
        <div class="container mx-auto">
            <div class="grid lg:grid-cols-2 gap-16 items-center">
                <div class="fade-in">
                    <h2 class="text-7xl font-bold text-red-900 mb-8 elegant-serif text-shadow-elegant">
                        Seus <span class="script-elegant gradient-text-red">Fios</span>
                    </h2>
                    <h3 class="text-4xl text-red-800 mb-8 script-elegant">merecem ouro</h3>
                    <p class="text-2xl text-red-700 mb-12 classic-serif leading-relaxed">
                        Transformamos cada fio em uma obra de arte. Cuidados profissionais que revelam a verdadeira beleza dos seus cabelos.
                    </p>
                    <button onclick="scrollToSection('servicos')" class="bg-red-600 hover:bg-red-700 text-white px-12 py-6 rounded-full text-2xl font-bold transition-all shadow-2xl hover:shadow-3xl elegant-serif">
                        Descobrir Cuidados
                    </button>
                </div>
                <div class="fade-in">
                    <div class="hair-image h-96 overlay-red" style="background-image: url('https://images.unsplash.com/photo-1522337360788-8b13dee7a37e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1000&q=80');">
                        <div class="h-full flex items-end p-8">
                            <div class="bg-white/90 p-6 rounded-2xl">
                                <p class="text-red-800 classic-serif text-lg font-bold">Cabelos saudáveis e radiantes</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Serviços -->
    <section id="servicos" class="py-24 px-8">
        <div class="container mx-auto">
            <h3 class="text-6xl font-bold text-center text-red-900 mb-20 elegant-serif text-shadow-elegant">Nossos Serviços</h3>
            
            <div class="grid md:grid-cols-3 gap-12">
                <!-- Hidratação -->
                <div class="bg-white/90 rounded-3xl p-10 shadow-2xl card-hover red-border-elegant">
                    <div class="hair-image h-48 mb-8" style="background-image: url('https://images.unsplash.com/photo-1560066984-138dadb4c035?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1000&q=80');">
                        <div class="overlay-red h-full flex items-center justify-center">
                            <span class="text-5xl floating-gentle">💧</span>
                        </div>
                    </div>
                    <h4 class="text-3xl font-bold text-red-800 mb-6 text-center elegant-serif">Hidratação Profunda</h4>
                    <ul class="space-y-4 text-red-700 classic-serif text-lg">
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Máscaras nutritivas intensivas</span>
                        </li>
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Óleos naturais premium</span>
                        </li>
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Tratamento com vapor</span>
                        </li>
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Resultados duradouros</span>
                        </li>
                    </ul>
                </div>

                <!-- Reconstrução -->
                <div class="bg-white/90 rounded-3xl p-10 shadow-2xl card-hover red-border-elegant">
                    <div class="hair-image h-48 mb-8" style="background-image: url('https://images.unsplash.com/photo-1519699047748-de8e457a634e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1000&q=80');">
                        <div class="overlay-red h-full flex items-center justify-center">
                            <span class="text-5xl floating-gentle">🔧</span>
                        </div>
                    </div>
                    <h4 class="text-3xl font-bold text-red-800 mb-6 text-center elegant-serif">Reconstrução Capilar</h4>
                    <ul class="space-y-4 text-red-700 classic-serif text-lg">
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Proteínas de alta qualidade</span>
                        </li>
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Reparação de danos químicos</span>
                        </li>
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Fortalecimento da fibra</span>
                        </li>
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Resistência e elasticidade</span>
                        </li>
                    </ul>
                </div>

                <!-- Nutrição -->
                <div class="bg-white/90 rounded-3xl p-10 shadow-2xl card-hover red-border-elegant">
                    <div class="hair-image h-48 mb-8" style="background-image: url('https://images.unsplash.com/photo-1487412947147-5cebf100ffc2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1000&q=80');">
                        <div class="overlay-red h-full flex items-center justify-center">
                            <span class="text-5xl floating-gentle">🌿</span>
                        </div>
                    </div>
                    <h4 class="text-3xl font-bold text-red-800 mb-6 text-center elegant-serif">Nutrição Intensiva</h4>
                    <ul class="space-y-4 text-red-700 classic-serif text-lg">
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Vitaminas e minerais essenciais</span>
                        </li>
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Extratos botânicos puros</span>
                        </li>
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Brilho e maciez incomparáveis</span>
                        </li>
                        <li class="flex items-start">
                            <span class="text-red-500 mr-4 text-2xl">•</span>
                            <span>Proteção antioxidante</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Tratamentos Especiais -->
    <section id="tratamentos" class="py-24 px-8 bg-white/40">
        <div class="container mx-auto">
            <h3 class="text-6xl font-bold text-center text-red-900 mb-20 elegant-serif text-shadow-elegant">Tratamentos Exclusivos</h3>
            
            <div class="grid lg:grid-cols-2 gap-16">
                <div class="bg-white/95 rounded-3xl p-12 shadow-2xl card-hover">
                    <div class="hair-image h-64 mb-8" style="background-image: url('https://images.unsplash.com/photo-1562322140-8baeececf3df?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1000&q=80');">
                        <div class="overlay-red h-full flex items-center justify-center">
                            <span class="text-6xl floating-gentle">✨</span>
                        </div>
                    </div>
                    <h4 class="text-4xl font-bold text-red-800 mb-8 text-center script-elegant">Cronograma Capilar</h4>
                    <div class="space-y-6 classic-serif text-lg text-red-700">
                        <div class="bg-red-50 p-6 rounded-2xl red-border-elegant">
                            <h5 class="font-bold text-red-900 mb-3 elegant-serif text-xl">Semana 1: Hidratação</h5>
                            <p>Reposição intensa de água e nutrientes</p>
                        </div>
                        <div class="bg-red-50 p-6 rounded-2xl red-border-elegant">
                            <h5 class="font-bold text-red-900 mb-3 elegant-serif text-xl">Semana 2: Nutrição</h5>
                            <p>Vitaminas e óleos para brilho natural</p>
                        </div>
                        <div class="bg-red-50 p-6 rounded-2xl red-border-elegant">
                            <h5 class="font-bold text-red-900 mb-3 elegant-serif text-xl">Semana 3: Reconstrução</h5>
                            <p>Proteínas para força e resistência</p>
                        </div>
                    </div>
                </div>

                <div class="bg-white/95 rounded-3xl p-12 shadow-2xl card-hover">
                    <div class="hair-image h-64 mb-8" style="background-image: url('https://images.unsplash.com/photo-1526045478516-99145907023c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1000&q=80');">
                        <div class="overlay-red h-full flex items-center justify-center">
                            <span class="text-6xl floating-gentle">💎</span>
                        </div>
                    </div>
                    <h4 class="text-4xl font-bold text-red-800 mb-8 text-center script-elegant">Tratamentos Premium</h4>
                    <div class="space-y-6 classic-serif text-lg text-red-700">
                        <div class="bg-red-50 p-6 rounded-2xl red-border-elegant">
                            <h5 class="font-bold text-red-900 mb-3 elegant-serif text-xl">Botox Capilar Gold</h5>
                            <p>Rejuvenescimento completo dos fios</p>
                        </div>
                        <div class="bg-red-50 p-6 rounded-2xl red-border-elegant">
                            <h5 class="font-bold text-red-900 mb-3 elegant-serif text-xl">Cauterização Diamante</h5>
                            <p>Selagem perfeita das cutículas</p>
                        </div>
                        <div class="bg-red-50 p-6 rounded-2xl red-border-elegant">
                            <h5 class="font-bold text-red-900 mb-3 elegant-serif text-xl">Olaplex Therapy</h5>
                            <p>Reconstrução molecular avançada</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Galeria -->
    <section id="galeria" class="py-24 px-8">
        <div class="container mx-auto">
            <h3 class="text-6xl font-bold text-center text-red-900 mb-20 elegant-serif text-shadow-elegant">Transformações</h3>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="card-hover">
                    <div class="hair-image h-80" style="background-image: url('https://images.unsplash.com/photo-1580618672591-eb180b1a973f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1000&q=80');">
                        <div class="overlay-red h-full flex items-end p-6">
                            <div class="bg-white/95 p-4 rounded-xl">
                                <p class="text-red-800 classic-serif font-bold">Hidratação Profunda</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="card-hover">
                    <div class="hair-image h-80" style="background-image: url('https://images.unsplash.com/photo-1595475038665-8de2a4b72174?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1000&q=80');">
                        <div class="overlay-red h-full flex items-end p-6">
                            <div class="bg-white/95 p-4 rounded-xl">
                                <p class="text-red-800 classic-serif font-bold">Reconstrução Capilar</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="card-hover">
                    <div class="hair-image h-80" style="background-image: url('https://images.unsplash.com/photo-1522338242992-e1a54906a8da?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1000&q=80');">
                        <div class="overlay-red h-full flex items-end p-6">
                            <div class="bg-white/95 p-4 rounded-xl">
                                <p class="text-red-800 classic-serif font-bold">Nutrição Intensiva</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Dicas Especiais -->
    <section class="py-24 px-8 bg-white/40">
        <div class="container mx-auto">
            <h3 class="text-6xl font-bold text-center text-red-900 mb-20 elegant-serif text-shadow-elegant">Dicas de Ouro</h3>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-10">
                <div class="bg-white/95 p-8 rounded-2xl shadow-xl text-center card-hover red-border-elegant">
                    <span class="text-6xl mb-6 block floating-gentle">🌡️</span>
                    <h5 class="font-bold text-red-900 mb-4 elegant-serif text-2xl">Temperatura Ideal</h5>
                    <p class="text-red-700 classic-serif text-lg">Água morna para lavar, fria para selar</p>
                </div>
                
                <div class="bg-white/95 p-8 rounded-2xl shadow-xl text-center card-hover red-border-elegant">
                    <span class="text-6xl mb-6 block floating-gentle">🛡️</span>
                    <h5 class="font-bold text-red-900 mb-4 elegant-serif text-2xl">Proteção Térmica</h5>
                    <p class="text-red-700 classic-serif text-lg">Sempre antes do calor</p>
                </div>
                
                <div class="bg-white/95 p-8 rounded-2xl shadow-xl text-center card-hover red-border-elegant">
                    <span class="text-6xl mb-6 block floating-gentle">✂️</span>
                    <h5 class="font-bold text-red-900 mb-4 elegant-serif text-2xl">Corte Regular</h5>
                    <p class="text-red-700 classic-serif text-lg">A cada 2-3 meses</p>
                </div>
                
                <div class="bg-white/95 p-8 rounded-2xl shadow-xl text-center card-hover red-border-elegant">
                    <span class="text-6xl mb-6 block floating-gentle">🌙</span>
                    <h5 class="font-bold text-red-900 mb-4 elegant-serif text-2xl">Fronha de Seda</h5>
                    <p class="text-red-700 classic-serif text-lg">Menos atrito, mais brilho</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-red-900 text-red-100 py-20 px-8">
        <div class="container mx-auto text-center">
            <div class="mb-10 floating-gentle">
                <span class="text-5xl">👑</span>
                <span class="text-5xl mx-8">✨</span>
                <span class="text-5xl">💎</span>
            </div>
            <h4 class="text-5xl font-bold mb-8 script-elegant text-shadow-elegant">FiosDeOuros</h4>
            <p class="text-red-300 mb-10 classic-serif text-2xl">Onde cada fio se transforma em ouro</p>
            <div class="script-elegant text-3xl text-red-200 mb-8">
                "A beleza dos seus cabelos é nossa especialidade"
            </div>
            <p class="text-red-400 classic-serif text-lg">© 2024 FiosDeOuros - Todos os direitos reservados</p>
        </div>
    </footer>

    <script>
        function scrollToSection(sectionId) {
            document.getElementById(sectionId).scrollIntoView({
                behavior: 'smooth'
            });
        }

        // Animação de entrada para elementos
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -100px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('fade-in');
                }
            });
        }, observerOptions);

        // Observar todas as seções
        document.querySelectorAll('section').forEach(section => {
            observer.observe(section);
        });

        // Efeito parallax suave
        window.addEventListener('scroll', () => {
            const scrolled = window.pageYOffset;
            const parallaxElements = document.querySelectorAll('.floating-gentle');
            parallaxElements.forEach(element => {
                const speed = scrolled * 0.3;
                element.style.transform = `translateY(${speed}px)`;
            });
        });

        // Efeito hover nas imagens
        document.querySelectorAll('.hair-image').forEach(image => {
            image.addEventListener('mouseenter', function() {
                this.style.transform = 'scale(1.05)';
                this.style.transition = 'transform 0.5s ease';
            });
            
            image.addEventListener('mouseleave', function() {
                this.style.transform = 'scale(1)';
            });
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'98a5c952442ec20f',t:'MTc1OTc2MDI4OS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
