<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Suntechworld Global Services | Innovation & Empowerment</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script defer src="https://unpkg.com/alpinejs@3.x.x/dist/cdn.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2">

</script>

    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;800&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Plus Jakarta Sans', sans-serif; scroll-behavior: smooth; }
        .gradient-bg { background: linear-gradient(135deg, #1a1a1a 0%, #2d3436 100%); }
    </style>
</head>
<body class="bg-slate-50 text-slate-900" x-data="{ mobileMenu: false, authModal: false, isLogin: true }">

    <nav class="sticky top-0 z-50 bg-white/80 backdrop-blur-md border-b">
        <div class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">
            <div class="text-2xl font-800 tracking-tighter text-yellow-600">SUNTECH<span class="text-slate-900">WORLD</span></div>
            
            <div class="hidden md:flex space-x-8 font-semibold text-sm uppercase tracking-wide">
                <a href="#home" class="hover:text-yellow-600">Home</a>
                <a href="#shop" class="hover:text-yellow-600">Shop</a>
                <a href="#gallery" class="hover:text-yellow-600">Impact</a>
                <a href="#testimonials" class="hover:text-yellow-600">Testimonials</a>
                <a href="#contact" class="hover:text-yellow-600">Contact</a>
            </div>

            <button @click="authModal = true" class="bg-slate-900 text-white px-6 py-2 rounded-full text-sm font-bold hover:bg-yellow-600 transition">
                Sign In
            </button>
        </div>
    </nav>

    <section id="home" class="gradient-bg text-white py-24 px-6 text-center">
        <div class="max-w-4xl mx-auto">
            <span class="text-yellow-500 font-bold tracking-widest uppercase text-sm">Innovating for Africa</span>
            <h1 class="text-5xl md:text-7xl font-extrabold mt-4 mb-6">Empowering Youth, Women & Agriculture.</h1>
            <p class="text-lg text-slate-300 mb-10 max-w-2xl mx-auto">Suntechworld Global Services delivers high-tech solutions in education and farming while transforming lives through humanitarian support.</p>
            <div class="flex flex-col md:flex-row justify-center gap-4">
                <a href="#shop" class="bg-yellow-500 text-slate-900 px-10 py-4 rounded-xl font-bold text-lg hover:bg-yellow-400">Explore Shop</a>
                <a href="#gallery" class="bg-white/10 border border-white/20 px-10 py-4 rounded-xl font-bold text-lg hover:bg-white/20">View Our Impact</a>
            </div>
        </div>
    </section>

    <section id="shop" class="py-20 max-w-7xl mx-auto px-6">
        <div class="flex justify-between items-end mb-12">
            <div>
                <h2 class="text-4xl font-extrabold">The Suntech Store</h2>
                <p class="text-slate-500">Premium tech and education products.</p>
            </div>
        </div>
        <div class="grid md:grid-cols-3 gap-8">
            <div class="bg-white rounded-2xl overflow-hidden shadow-lg border border-slate-100 group">
                <div class="h-64 bg-slate-200 overflow-hidden">
                    <img src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&q=80&w=800" alt="Tech Course" class="w-full h-full object-cover group-hover:scale-110 transition duration-500">
                </div>
                <div class="p-6">
                    <span class="text-xs font-bold text-yellow-600 uppercase">Education</span>
                    <h3 class="text-xl font-bold mt-2">Full-Stack Career Path</h3>
                    <p class="text-slate-600 text-sm mt-2">6-month intensive training with job placement.</p>
                    <div class="mt-6 flex justify-between items-center">
                        <span class="text-2xl font-bold">$150</span>
                        <button class="bg-slate-900 text-white px-4 py-2 rounded-lg text-sm">Enroll Now</button>
                    </div>
                </div>
            </div>
            <div class="bg-white rounded-2xl overflow-hidden shadow-lg border border-slate-100 group">
                <div class="h-64 bg-slate-200 overflow-hidden">
                    <img src="https://images.unsplash.com/photo-1581091226825-a6a2a5aee158?auto=format&fit=crop&q=80&w=800" alt="Soil Sensor" class="w-full h-full object-cover group-hover:scale-110 transition duration-500">
                </div>
                <div class="p-6">
                    <span class="text-xs font-bold text-green-600 uppercase">Agriculture</span>
                    <h3 class="text-xl font-bold mt-2">Green-Eye Soil Sensor</h3>
                    <p class="text-slate-600 text-sm mt-2">Solar-powered real-time soil analytics.</p>
                    <div class="mt-6 flex justify-between items-center">
                        <span class="text-2xl font-bold">$45</span>
                        <button class="bg-slate-900 text-white px-4 py-2 rounded-lg text-sm">Add to Cart</button>
                    </div>
                </div>
            </div>
            <div class="bg-white rounded-2xl overflow-hidden shadow-lg border border-slate-100 group">
                <div class="h-64 bg-slate-200 overflow-hidden">
                    <img src="https://images.unsplash.com/photo-1509091350041-6c7d40c5b7de?auto=format&fit=crop&q=80&w=800" alt="Solar Lamp" class="w-full h-full object-cover group-hover:scale-110 transition duration-500">
                </div>
                <div class="p-6">
                    <span class="text-xs font-bold text-blue-600 uppercase">Humanitarian</span>
                    <h3 class="text-xl font-bold mt-2">Sponsor a Solar Lamp</h3>
                    <p class="text-slate-600 text-sm mt-2">Provide light for off-grid students.</p>
                    <div class="mt-6 flex justify-between items-center">
                        <span class="text-2xl font-bold">$15</span>
                        <button class="bg-yellow-500 text-slate-900 px-4 py-2 rounded-lg text-sm font-bold">Donate One</button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="gallery" class="py-20 bg-slate-100">
        <div class="max-w-7xl mx-auto px-6 text-center">
            <h2 class="text-4xl font-extrabold mb-12">Our Impact Gallery</h2>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                <div class="h-48 bg-slate-300 rounded-xl overflow-hidden"><img src="https://images.unsplash.com/photo-1524178232363-1fb28f74b671?auto=format&fit=crop&w=400" class="w-full h-full object-cover"></div>
                <div class="h-48 bg-slate-300 rounded-xl overflow-hidden"><img src="https://images.unsplash.com/photo-1593113598332-cd288d649433?auto=format&fit=crop&w=400" class="w-full h-full object-cover"></div>
                <div class="h-48 bg-slate-300 rounded-xl overflow-hidden"><img src="https://images.unsplash.com/photo-1531206715517-5c0ba140b2b8?auto=format&fit=crop&w=400" class="w-full h-full object-cover"></div>
                <div class="h-48 bg-slate-300 rounded-xl overflow-hidden"><img src="https://images.unsplash.com/photo-1495539406979-bf61750d38ad?auto=format&fit=crop&w=400" class="w-full h-full object-cover"></div>
            </div>
        </div>
    </section>

    <section id="testimonials" class="py-20">
        <div class="max-w-5xl mx-auto px-6 text-center">
            <h2 class="text-3xl font-bold mb-12">Voices of Success</h2>
            <div class="grid md:grid-cols-2 gap-8">
                <div class="bg-white p-8 rounded-2xl shadow-sm italic text-slate-600 border">
                    "The soil sensors transformed our yields in just one season. Suntechworld is changing farming in Africa."
                    <p class="mt-4 font-bold text-slate-900">— Amina J., Agri-Partner</p>
                </div>
                <div class="bg-white p-8 rounded-2xl shadow-sm italic text-slate-600 border">
                    "I learned to build apps and now I support my family with a remote tech job. Empowering indeed!"
                    <p class="mt-4 font-bold text-slate-900">— Kofi A., Academy Alumni</p>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-2 gap-16">
            <div>
                <h2 class="text-4xl font-extrabold mb-6">Let's Build Africa Together</h2>
                <p class="text-lg text-slate-600 mb-8">Ready to innovate or want to partner with us for humanitarian missions? Reach out to Suntechworld Global Services.</p>
                <div class="space-y-4">
                    <div class="flex items-center space-x-4">
                        <span class="p-3 bg-yellow-100 text-yellow-600 rounded-full">📍</span>
                        <p>Lagos, Nigeria | Accra, Ghana</p>
                    </div>
                    <div class="flex items-center space-x-4">
                        <span class="p-3 bg-blue-100 text-blue-600 rounded-full">📧</span>
                        <p>hello@suntechworld.global</p>
                    </div>
                </div>
            </div>
            <form class="space-y-4 bg-slate-50 p-8 rounded-2xl border">
                <input type="text" placeholder="Your Name" class="w-full p-4 rounded-xl border-slate-200 focus:ring-2 focus:ring-yellow-500 outline-none">
                <input type="email" placeholder="Your Email" class="w-full p-4 rounded-xl border-slate-200 focus:ring-2 focus:ring-yellow-500 outline-none">
                <textarea rows="4" placeholder="Message" class="w-full p-4 rounded-xl border-slate-200 focus:ring-2 focus:ring-yellow-500 outline-none"></textarea>
                <button class="w-full bg-slate-900 text-white py-4 rounded-xl font-bold hover:bg-yellow-600 transition">Send Message</button>
            </form>
        </div>
    </section>

    <footer class="bg-slate-900 text-slate-400 py-12 px-6">
        <div class="max-w-7xl mx-auto flex flex-col md:row justify-between items-center border-b border-slate-800 pb-8">
            <div class="text-2xl font-bold text-white mb-4 md:mb-0">SUNTECHWORLD</div>
            <div class="flex space-x-6 text-sm">
                <a href="#" class="hover:text-white">Privacy Policy</a>
                <a href="#" class="hover:text-white">Terms of Service</a>
            </div>
        </div>
        <p class="text-center mt-8 text-xs">&copy; 2026 Suntechworld Global Services. All Rights Reserved.</p>
    </footer>

    <div x-show="authModal" class="fixed inset-0 z-[100] flex items-center justify-center bg-black/60 backdrop-blur-sm p-4" x-cloak>
        <div @click.away="authModal = false" class="bg-white max-w-md w-full rounded-3xl p-8 shadow-2xl relative">
            <button @click="authModal = false" class="absolute top-4 right-4 text-slate-400 hover:text-slate-900">✕</button>
            <h2 class="text-3xl font-bold text-center mb-2" x-text="isLogin ? 'Sign In' : 'Sign Up'"></h2>
            <p class="text-center text-slate-500 mb-8">Access the Suntechworld Platform</p>
            
            <form class="space-y-4">
                <template x-if="!isLogin">
                    <input type="text" placeholder="Full Name" class="w-full p-3 border rounded-xl">
                </template>
                <input type="email" placeholder="Email Address" class="w-full p-3 border rounded-xl">
                <input type="password" placeholder="Password" class="w-full p-3 border rounded-xl">
                <button type="button" class="w-full bg-yellow-600 text-white py-3 rounded-xl font-bold">Continue</button>
            </form>

            <div class="mt-6 text-center">
                <button @click="isLogin = !isLogin" class="text-yellow-600 font-bold" x-text="isLogin ? 'Need an account? Sign Up' : 'Have an account? Sign In'"></button>
            </div>
        </div>
    </div>

</body>
</html>

