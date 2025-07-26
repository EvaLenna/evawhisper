<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EvaWhisper - Unveil Your Desires</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0a0a0a;
        }
        .font-serif {
            font-family: 'Playfair Display', serif;
        }
        .card {
            transition: transform 0.4s ease, box-shadow 0.4s ease, border-color 0.4s ease;
            border: 1px solid rgba(255, 255, 255, 0.1);
            opacity: 0;
            transform: translateY(30px);
        }
        .card.is-visible {
            opacity: 1;
            transform: translateY(0);
        }
        .card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 0 40px rgba(220, 38, 38, 0.4);
            border-color: rgba(220, 38, 38, 0.6);
        }
        .btn-primary {
            transition: background-color 0.3s ease, transform 0.3s ease, box-shadow 0.3s ease;
        }
        .btn-primary:hover {
            transform: translateY(-3px) scale(1.05);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
        }
        #age-gate {
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
        }
        #main-content.blurred {
            filter: blur(10px);
            pointer-events: none;
            user-select: none;
        }
        .text-glow {
            text-shadow: 0 0 8px rgba(255, 255, 255, 0.3), 0 0 12px rgba(220, 38, 38, 0.2);
        }
    </style>
</head>
<body class="bg-gradient-to-br from-gray-900 to-black text-gray-300">

    <!-- Age Verification Gate -->
    <div id="age-gate" class="fixed inset-0 z-50 flex items-center justify-center bg-black bg-opacity-80 p-4 transition-opacity duration-500">
        <div class="bg-gray-900 border border-red-800 rounded-2xl shadow-2xl p-8 max-w-md w-full text-center">
            <h2 class="font-serif text-3xl text-white mb-4">Confirm Your Age</h2>
            <p class="text-gray-400 mb-8">This website contains content intended for adults only. You must be 18 years or older to continue.</p>
            <div class="flex flex-col sm:flex-row gap-4">
                <button id="enter-btn" class="btn-primary w-full bg-red-700 hover:bg-red-800 text-white font-bold py-3 px-6 rounded-lg">
                    I am 18 or older - Enter
                </button>
                <button id="exit-btn" class="w-full bg-gray-700 hover:bg-gray-600 text-white font-bold py-3 px-6 rounded-lg transition-colors">
                    I am not 18 - Exit
                </button>
            </div>
        </div>
    </div>

    <!-- Main Content (initially blurred) -->
    <div id="main-content" class="container mx-auto px-4 py-12 md:py-20 transition-filter duration-500 blurred">

        <!-- Header Section -->
        <header class="text-center mb-12 md:mb-16">
            <h1 class="font-serif text-5xl md:text-7xl font-bold text-white mb-4 text-glow">EvaWhisper</h1>
            <p class="text-lg text-gray-300 max-w-2xl mx-auto text-glow">Where your deepest fantasies become reality.</p>
        </header>

        <!-- Featured Video Player -->
        <section class="mb-12 md:mb-20">
            <div class="max-w-4xl mx-auto aspect-video rounded-2xl shadow-lg overflow-hidden border border-red-800/50">
                 <iframe src="https://streamable.com/e/2rynsg?autoplay=1&muted=1" frameborder="0" width="100%" height="100%" allowfullscreen allow="autoplay"></iframe>
            </div>
        </section>


        <!-- Products Grid -->
        <main class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 md:gap-10">

            <!-- Product Card 1 -->
            <div class="card bg-gray-900/80 backdrop-blur-sm rounded-2xl shadow-lg overflow-hidden flex flex-col">
                <img src="https://public-files.gumroad.com/ep2bxn9qlzne64u8bvsn6rfldflc" onerror="this.onerror=null;this.src='https://placehold.co/600x400/1a0000/e0e0e0?text=Temptation';" alt="Cover for Whisper of Temptation" class="w-full h-48 object-cover">
                <div class="p-6 flex-grow flex flex-col">
                    <h2 class="text-2xl font-semibold text-white mb-2">Whisper of Temptation</h2>
                    <p class="text-gray-400 mb-4 flex-grow">A guide to the world of sensual pleasures and hidden desires.</p>
                    <div class="mt-auto pt-4">
                        <a href="https://slawek2094.gumroad.com/l/nqodhm" target="_blank" class="btn-primary block w-full text-center bg-red-700 text-white font-semibold py-3 rounded-lg hover:bg-red-600">Discover the Secret</a>
                    </div>
                </div>
            </div>

            <!-- Product Card 2 -->
            <div class="card bg-gray-900/80 backdrop-blur-sm rounded-2xl shadow-lg overflow-hidden flex flex-col">
                <img src="https://public-files.gumroad.com/ryq89samkt58zf0yro320l6ir2tu" onerror="this.onerror=null;this.src='https://placehold.co/600x400/2a0000/e0e0e0?text=Touch';" alt="Cover for Touch of the Night" class="w-full h-48 object-cover">
                <div class="p-6 flex-grow flex flex-col">
                    <h2 class="text-2xl font-semibold text-white mb-2">Touch of the Night</h2>
                    <p class="text-gray-400 mb-4 flex-grow">Learn techniques that ignite the senses and deepen intimate connection.</p>
                    <div class="mt-auto pt-4">
                        <a href="https://slawek2094.gumroad.com/l/rjdcr" target="_blank" class="btn-primary block w-full text-center bg-red-700 text-white font-semibold py-3 rounded-lg hover:bg-red-600">Feel the Touch</a>
                    </div>
                </div>
            </div>

            <!-- Product Card 3 -->
            <div class="card bg-gray-900/80 backdrop-blur-sm rounded-2xl shadow-lg overflow-hidden flex flex-col">
                <img src="https://public-files.gumroad.com/wwlvxsqv6cbbyff4h12ji4bjyz6i" onerror="this.onerror=null;this.src='https://placehold.co/600x400/3a0000/e0e0e0?text=Desire';" alt="Cover for Key to Desire" class="w-full h-48 object-cover">
                <div class="p-6 flex-grow flex flex-col">
                    <h2 class="text-2xl font-semibold text-white mb-2">Key to Desire</h2>
                    <p class="text-gray-400 mb-4 flex-grow">Unlock the world of dominance and submission. Find your role.</p>
                    <div class="mt-auto pt-4">
                        <a href="https://slawek2094.gumroad.com/l/papbiw" target="_blank" class="btn-primary block w-full text-center bg-red-700 text-white font-semibold py-3 rounded-lg hover:bg-red-600">Turn the Key</a>
                    </div>
                </div>
            </div>

            <!-- Product Card 4 -->
            <div class="card bg-gray-900/80 backdrop-blur-sm rounded-2xl shadow-lg overflow-hidden flex flex-col">
                <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%2Fid%2FOIP.V-iiE3si2N1HnjWte3OgYQHaFV%3Fpid%3DApi&f=1&ipt=f17a4262ca594c73da6bf073371e6a126c468d187ee298a267c3f9be029534c5&ipo=images" onerror="this.onerror=null;this.src='https://placehold.co/600x400/4a0000/e0e0e0?text=Passion';" alt="Cover for Spark of Passion" class="w-full h-48 object-cover">
                <div class="p-6 flex-grow flex flex-col">
                    <h2 class="text-2xl font-semibold text-white mb-2">Spark of Passion</h2>
                    <p class="text-gray-400 mb-4 flex-grow">A collection of inspirations and scenarios to reignite the flame.</p>
                    <div class="mt-auto pt-4">
                        <a href="https://slawek2094.gumroad.com/l/zvtqln" target="_blank" class="btn-primary block w-full text-center bg-red-700 text-white font-semibold py-3 rounded-lg hover:bg-red-600">Ignite the Spark</a>
                    </div>
                </div>
            </div>

            <!-- Product Card 5 -->
            <div class="card bg-gray-900/80 backdrop-blur-sm rounded-2xl shadow-lg overflow-hidden flex flex-col">
                <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%2Fid%2FOIP.IO0C9RNH8i5k_yJl7ifDHgHaE8%3Fpid%3DApi&f=1&ipt=e2c59d62cf8f1aee96cea607fff19fdc4f7d0fc7c00f092440b1f23fb0ccaccb&ipo=images" onerror="this..onerror=null;this.src='https://placehold.co/600x400/5a0000/e0e0e0?text=Trust';" alt="Cover for Seal of Trust" class="w-full h-48 object-cover">
                <div class="p-6 flex-grow flex flex-col">
                    <h2 class="text-2xl font-semibold text-white mb-2">Seal of Trust</h2>
                    <p class="text-gray-400 mb-4 flex-grow">Build a deep bond and safety while exploring new boundaries together.</p>
                    <div class="mt-auto pt-4">
                        <a href="https://slawek2094.gumroad.com/l/ysrivs" target="_blank" class="btn-primary block w-full text-center bg-red-700 text-white font-semibold py-3 rounded-lg hover:bg-red-600">Earn the Trust</a>
                    </div>
                </div>
            </div>

            <!-- Product Card 6 -->
            <div class="card bg-gray-900/80 backdrop-blur-sm rounded-2xl shadow-lg overflow-hidden flex flex-col">
                <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%2Fid%2FOIP.dS4BGI-cPYlWsoWOB5DV5AHaEK%3Fpid%3DApi&f=1&ipt=aef9866f1c8794fcd8f2a9aaf32d5bfa12d46740836353540a523306b21eaf5b&ipo=images" onerror="this.onerror=null;this.src='https://placehold.co/600x400/6a0000/e0e0e0?text=Stardust';" alt="Cover for Stardust" class="w-full h-48 object-cover">
                <div class="p-6 flex-grow flex flex-col">
                    <h2 class="text-2xl font-semibold text-white mb-2">Stardust</h2>
                    <p class="text-gray-400 mb-4 flex-grow">Discover the cosmic energy of orgasm and techniques to heighten pleasure.</p>
                    <div class="mt-auto pt-4">
                        <a href="https://slawek2094.gumroad.com/l/mragz" target="_blank" class="btn-primary block w-full text-center bg-red-700 text-white font-semibold py-3 rounded-lg hover:bg-red-600">Reach for the Stars</a>
                    </div>
                </div>
            </div>

        </main>
        
        <!-- Footer -->
        <footer class="text-center mt-16 md:mt-20 text-gray-500">
            <p>&copy; 2024 EvaWhisper. All rights reserved.</p>
            <p class="text-xs mt-2">The content on this website is intended for adults only.</p>
        </footer>

    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const ageGate = document.getElementById('age-gate');
            const mainContent = document.getElementById('main-content');
            const enterBtn = document.getElementById('enter-btn');
            const exitBtn = document.getElementById('exit-btn');

            // Age Gate Logic
            if (sessionStorage.getItem('ageVerified') === 'true') {
                ageGate.style.display = 'none';
                mainContent.classList.remove('blurred');
            }

            enterBtn.addEventListener('click', () => {
                sessionStorage.setItem('ageVerified', 'true');
                ageGate.style.opacity = '0';
                mainContent.classList.remove('blurred');
                
                setTimeout(() => {
                    ageGate.style.display = 'none';
                }, 500);
            });

            exitBtn.addEventListener('click', () => {
                window.location.href = 'https://www.google.com';
            });

            // Scroll Animation Logic
            const cards = document.querySelectorAll('.card');
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('is-visible');
                    }
                });
            }, {
                threshold: 0.1
            });

            cards.forEach(card => {
                observer.observe(card);
            });
        });
    </script>

</body>
</html>
