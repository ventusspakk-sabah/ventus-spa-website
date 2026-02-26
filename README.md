# ventus-spa-website
Ventus Spa - 7 Page Full Service Luxury Hub
<!DOCTYPE html>
<html lang="zh-Hant">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ventus Spa | 7-Page Full Service Luxury Hub</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        html { scroll-behavior: smooth; }
        body { font-family: 'Inter', sans-serif; background-color: #F8F7F2; }
        .font-serif { font-family: 'Playfair Display', serif; }
        .nav-link { position: relative; padding: 0.5rem 0; transition: color 0.3s; }
        .nav-link::after { 
            content: ''; position: absolute; width: 0; height: 1.5px; 
            bottom: 0; left: 0; background-color: #57635c; transition: width 0.3s; 
        }
        .nav-link:hover::after { width: 100%; }
        #mobile-menu { transition: transform 0.5s cubic-bezier(0.77, 0, 0.175, 1); }
        .hidden-menu { transform: translateY(-100%); }
        .section-title { position: relative; display: inline-block; padding-bottom: 15px; }
        .section-title::after { 
            content: ''; position: absolute; width: 40px; height: 1px; 
            background: #57635c; bottom: 0; left: 50%; transform: translateX(-50%); 
        }
        .service-card:hover { transform: translateY(-5px); transition: all 0.3s ease; border-color: #57635c; }
    </style>
</head>
<body class="text-stone-800">

    <nav class="bg-white/90 backdrop-blur-md sticky top-0 z-50 shadow-sm">
        <div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between">
            <div class="text-2xl font-serif tracking-[0.2em] text-[#4A554F] font-bold uppercase">Ventus Spa</div>
            <div class="hidden md:flex space-x-6 text-[10px] uppercase tracking-[0.15em] font-semibold text-stone-500">
                <a href="#home" class="nav-link text-stone-900">Home 首頁</a>
                <a href="#story" class="nav-link">Story 故事</a>
                <a href="#mode" class="nav-link">Mode 模式</a>
                <a href="#inspa" class="nav-link">In-Spa 店內</a>
                <a href="#outcall" class="nav-link">Outcall 外派</a>
                <a href="#faq" class="nav-link">FAQ 問答</a>
                <a href="#contact" class="nav-link">Contact 聯繫</a>
            </div>
            <a href="https://wa.me/60128172166" class="hidden sm:block bg-[#57635c] text-white px-6 py-2 text-[10px] font-bold tracking-[0.2em] hover:bg-stone-700 transition uppercase shadow-lg">Book Now</a>
            <button id="menu-btn" class="md:hidden text-stone-600 p-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-7 w-7" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M4 6h16M4 12h16M4 18h16" /></svg>
            </button>
        </div>
    </nav>

    <div id="mobile-menu" class="fixed inset-0 z-[100] bg-[#2D3632] text-[#E5E1D8] flex flex-col items-center justify-center space-y-6 text-xl font-serif italic hidden-menu text-center">
        <button id="close-menu" class="absolute top-8 right-8"><svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" /></svg></button>
        <a href="#home" class="mobile-nav-item">Home 首頁</a>
        <a href="#story" class="mobile-nav-item">Story 故事</a>
        <a href="#mode" class="mobile-nav-item">Mode 模式</a>
        <a href="#inspa" class="mobile-nav-item">In-Spa 店內</a>
        <a href="#outcall" class="mobile-nav-item">Outcall 外派</a>
        <a href="#faq" class="mobile-nav-item">FAQ 問答</a>
        <a href="#contact" class="mobile-nav-item">Contact 聯繫</a>
    </div>

    <section id="home" class="relative h-[85vh] flex items-center overflow-hidden">
        <div class="absolute inset-0 bg-[url('https://images.unsplash.com/photo-1544161515-4ab6ce6db874?q=80&w=2070')] bg-cover bg-center">
            <div class="absolute inset-0 bg-black/40"></div>
        </div>
        <div class="relative z-10 max-w-7xl mx-auto px-10 text-white">
            <div class="inline-block bg-white/20 backdrop-blur-md px-4 py-1 text-[10px] tracking-[0.3em] uppercase mb-4">KL & Selangor Premium Therapy</div>
            <h1 class="text-6xl md:text-8xl font-serif mb-6 italic leading-tight">Ventus Spa</h1>
            <p class="text-xl font-light tracking-[0.4em] mb-10 opacity-90 uppercase">釋放疲憊 · 喚醒感官</p>
            <a href="https://wa.me/601172691788" class="bg-white text-stone-800 px-10 py-4 font-bold tracking-widest text-xs uppercase shadow-2xl hover:bg-stone-100 transition">立即預約 Booking Now</a>
        </div>
    </section>

    <section id="story" class="py-24 bg-white">
        <div class="max-w-4xl mx-auto px-6 text-center">
            <h2 class="text-3xl font-serif italic section-title mb-10">手藝是磨出來的 <br><span class="text-sm not-italic text-stone-400 tracking-[0.2em]">The Heritage of Craftsmanship Since 1970s</span></h2>
            <div class="space-y-6 text-stone-600 leading-relaxed text-sm md:text-base italic">
                <p>源於 1970 年代的傳承。我們結合了中醫師父親的「精準穴位點壓」與馬來母親傳承的「天然香茅驅風推拿」。</p>
                <p class="font-serif text-stone-900 text-lg not-italic font-bold">"按得準、推得爽、風散得快。"</p>
            </div>
        </div>
    </section>

    <section id="mode" class="py-12 bg-stone-50">
        <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-2 gap-4">
            <div class="group relative h-80 overflow-hidden">
                <img src="https://images.unsplash.com/photo-1519415387722-a1c3bbef716c?q=80&w=800" class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition duration-700">
                <div class="absolute inset-0 bg-black/50 flex flex-col justify-center items-center text-white p-6">
                    <h3 class="text-2xl font-serif italic">店內奢華 In-Spa</h3>
                    <p class="text-[10px] tracking-widest uppercase mt-2 opacity-80 text-center">私密靜謐環境 · 五星級理療設備</p>
                    <a href="#inspa" class="mt-4 px-6 py-2 border border-white text-[10px] tracking-widest hover:bg-white hover:text-black transition uppercase">View Catalog</a>
                </div>
            </div>
            <div class="group relative h-80 overflow-hidden">
                <img src="https://images.unsplash.com/photo-1540555700478-4be289fbecef?q=80&w=800" class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition duration-700">
                <div class="absolute inset-0 bg-[#57635c]/60 flex flex-col justify-center items-center text-white p-6">
                    <h3 class="text-2xl font-serif italic">專業外派 Outcall</h3>
                    <p class="text-[10px] tracking-widest uppercase mt-2 opacity-80 text-center">飯店住宅專人上門 · 免除塞車煩惱</p>
                    <a href="#outcall" class="mt-4 px-6 py-2 bg-white text-[#57635c] text-[10px] tracking-widest hover:bg-stone-100 transition uppercase">View Offers</a>
                </div>
            </div>
        </div>
    </section>

    <section id="inspa" class="py-24">
        <div class="max-w-5xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-2xl font-serif italic section-title">店內服務目錄 In-Spa Catalog</h2>
                <p class="text-[10px] text-stone-400 mt-2 uppercase">點擊下方按鈕直接進入預約網站</p>
            </div>
            <div class="grid md:grid-cols-2 gap-8">
                <div class="bg-white p-8 border border-stone-100 shadow-sm service-card flex flex-col justify-between">
                    <div>
                        <div class="flex justify-between items-start mb-4">
                            <h4 class="font-bold text-lg text-stone-800">馬來傳統香茅按摩<br><span class="text-xs text-stone-400 font-normal italic">Signature Malay Lemongrass Massage</span></h4>
                            <span class="text-[#d35400] font-bold">RM 78</span>
                        </div>
                        <p class="text-[10px] text-stone-500 mb-6">時長: 60分鐘 | 內容: 全身推拿、特製香茅油、驅風舒壓。</p>
                    </div>
                    <a href="https://ventus-spa.com/booking" target="_blank" class="text-center border border-[#57635c] text-[#57635c] py-2 text-[10px] font-bold tracking-widest hover:bg-[#57635c] hover:text-white transition uppercase">進入預約網站 Visit Website</a>
                </div>
                <div class="bg-white p-8 border border-stone-100 shadow-sm service-card flex flex-col justify-between">
                    <div>
                        <div class="flex justify-between items-start mb-4">
                            <h4 class="font-bold text-lg text-stone-800">深度穴位理療 (無油)<br><span class="text-xs text-stone-400 font-normal italic">Deep Tissue Acupressure (No Oil)</span></h4>
                            <span class="text-[#d35400] font-bold">RM 78</span>
                        </div>
                        <p class="text-[10px] text-stone-500 mb-6">時長: 60分鐘 | 內容: 中式指壓、精準穴位放鬆、緩解長期肌肉僵硬。</p>
                    </div>
                    <a href="https://ventus-spa.com/booking" target="_blank" class="text-center border border-[#57635c] text-[#57635c] py-2 text-[10px] font-bold tracking-widest hover:bg-[#57635c] hover:text-white transition uppercase">進入預約網站 Visit Website</a>
                </div>
                <div class="bg-white p-8 border border-stone-100 shadow-sm service-card col-span-1 md:col-span-2 border-t-4 border-[#57635c] flex flex-col md:flex-row justify-between items-center">
                    <div class="mb-6 md:mb-0">
                        <div class="flex items-center gap-4 mb-2">
                            <h4 class="font-bold text-xl text-stone-800">招牌深度修復全效套餐</h4>
                            <span class="text-[#d35400] font-bold text-xl">RM 138</span>
                        </div>
                        <p class="text-xs text-stone-400 italic mb-2">Signature Full Body Recovery Combo (120 min)</p>
                        <p class="text-[10px] text-stone-500 uppercase tracking-tighter">90min Massage + 30min Foot + Free Ear Waxing</p>
                    </div>
                    <a href="https://ventus-spa.com/booking" target="_blank" class="w-full md:w-auto px-12 py-3 bg-[#57635c] text-white text-[10px] font-bold tracking-widest hover:bg-stone-800 transition uppercase shadow-md">立即在線預約 Online Booking</a>
                </div>
            </div>
        </div>
    </section>

    <section id="outcall" class="py-24 bg-[#F2F0E9]">
        <div class="max-w-5xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-2xl font-serif italic section-title">外派服務項目 Outcall Services</h2>
            </div>
            <div class="grid md:grid-cols-2 gap-8">
                <div class="bg-white p-8 border-t-4 border-[#A9B388] shadow-md">
                    <div class="flex justify-between items-center mb-6">
                        <h4 class="font-bold text-stone-800">單人上門首試價<br><span class="text-[10px] text-stone-400 italic">Single Outcall Trial</span></h4>
                        <span class="text-xl font-bold text-[#d35400]">RM 89</span>
                    </div>
                    <a href="https://wa.me/601172691788" class="block text-center bg-[#A9B388] text-white py-2 text-[10px] font-bold tracking-widest uppercase">WhatsApp 預約</a>
                </div>
                <div class="bg-white p-8 border-t-4 border-[#A9B388] shadow-md">
                    <div class="flex justify-between items-center mb-6">
                        <h4 class="font-bold text-stone-800">雙人/情侶同行組合<br><span class="text-[10px] text-stone-400 italic">Duo/Couple Home Spa</span></h4>
                        <span class="text-xl font-bold text-[#d35400]">RM 188</span>
                    </div>
                    <a href="https://wa.me/601172691788" class="block text-center bg-[#A9B388] text-white py-2 text-[10px] font-bold tracking-widest uppercase">WhatsApp 預約</a>
                </div>
            </div>
        </div>
    </section>

    <section id="faq" class="py-24 max-w-3xl mx-auto px-6">
        <h2 class="text-2xl font-serif italic text-center mb-12 section-title w-full">常見問題 FAQ</h2>
        <div class="space-y-4">
            <details class="group bg-white p-6 cursor-pointer border-l-4 border-[#57635c]"><summary class="font-bold text-sm uppercase">如何進行外派預約？<span class="float-right group-open:rotate-180">↓</span></summary><p class="mt-4 text-xs text-stone-500 italic">請透過 WhatsApp 提供地點時間，我們將在 15 分鐘內確認師傅安排。</p></details>
        </div>
    </section>

    <footer id="contact" class="bg-[#2D3632] text-[#E5E1D8] pt-24 pb-12">
        <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-4 gap-12 border-b border-white/5 pb-20">
            <div class="col-span-1">
                <h4 class="text-3xl font-serif italic mb-6">Ventus Spa</h4>
                <p class="opacity-40 text-[10px] uppercase tracking-widest leading-loose">Hotline: 01172691788<br>WhatsApp: +60128172166<br>WeChat: ventusspa</p>
            </div>
            <div>
                <h5 class="text-[10px] font-bold text-white/40 mb-8 uppercase tracking-[0.2em]">Social Media</h5>
                <ul class="text-[11px] space-y-4 opacity-70">
                    <li>Line: ventusspa123</li>
                    <li>Kakaotalk: ventusspa</li>
                </ul>
            </div>
            <div class="md:col-span-2 text-right">
                <a href="https://wa.me/601172691788" class="inline-block bg-white text-stone-800 px-12 py-4 text-[10px] font-bold tracking-[0.2em] hover:bg-stone-200 transition uppercase shadow-xl">Booking Now</a>
            </div>
        </div>
        <div class="text-center mt-12 text-[8px] opacity-20 uppercase tracking-[0.4em]">© 2026 VENTUS SPA MALAYSIA.</div>
    </footer>

    <script>
        const menuBtn = document.getElementById('menu-btn');
        const closeBtn = document.getElementById('close-menu');
        const mobileMenu = document.getElementById('mobile-menu');
        const items = document.querySelectorAll('.mobile-nav-item');
        menuBtn.onclick = () => { mobileMenu.classList.remove('hidden-menu'); document.body.style.overflow = 'hidden'; }
        closeBtn.onclick = () => { mobileMenu.classList.add('hidden-menu'); document.body.style.overflow = 'auto'; }
        items.forEach(i => i.onclick = () => { mobileMenu.classList.add('hidden-menu'); document.body.style.overflow = 'auto'; });
    </script>
</body>
</html>
