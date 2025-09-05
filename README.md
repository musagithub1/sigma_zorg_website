<!DOCTYPE html>
<html lang="nl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sigma Zorg Website - Developer Documentation</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.0/css/all.min.css">
    <style>
        body { font-family: 'Inter', sans-serif; }
        .code-block { background: #1a1a1a; color: #e5e5e5; }
        .highlight { background: linear-gradient(135deg, #4CAF50, #45a049); }
        pre { white-space: pre-wrap; }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">
    <!-- Header -->
    <header class="highlight text-white py-8">
        <div class="container mx-auto px-6">
            <div class="text-center">
                <h1 class="text-4xl font-bold mb-2">📋 Sigma Zorg Website</h1>
                <p class="text-xl opacity-90">Developer Documentation & Implementation Guide</p>
            </div>
        </div>
    </header>

    <div class="container mx-auto px-6 py-8">
        <!-- Quick Links -->
        <div class="bg-white rounded-lg shadow-lg p-6 mb-8">
            <h2 class="text-2xl font-bold mb-4"><i class="fas fa-rocket text-green-500"></i> Quick Start</h2>
            <div class="grid md:grid-cols-2 gap-4">
                <div>
                    <h3 class="font-semibold text-lg mb-2">🌐 Live Demo</h3>
                    <a href="https://pfhrgvwb.gensparkspace.com/" class="text-blue-600 hover:underline" target="_blank">
                        https://pfhrgvwb.gensparkspace.com/
                    </a>
                </div>
                <div>
                    <h3 class="font-semibold text-lg mb-2">📱 WhatsApp Contact</h3>
                    <code class="bg-gray-100 px-2 py-1 rounded">+31 6 86350771</code>
                </div>
            </div>
        </div>

        <!-- Project Overview -->
        <div class="bg-white rounded-lg shadow-lg p-6 mb-8">
            <h2 class="text-2xl font-bold mb-4"><i class="fas fa-info-circle text-blue-500"></i> Project Overzicht</h2>
            <p class="text-gray-600 mb-4">Complete moderne website voor Sigma Zorg - Thuiszorg in Amsterdam e.o. met focus op customer journey, storytelling en WhatsApp integratie.</p>
            
            <div class="grid md:grid-cols-3 gap-4 mt-6">
                <div class="text-center p-4 bg-green-50 rounded-lg">
                    <div class="text-3xl mb-2">🏥</div>
                    <h3 class="font-semibold">9 Diensten</h3>
                    <p class="text-sm text-gray-600">Complete zorgverlening</p>
                </div>
                <div class="text-center p-4 bg-blue-50 rounded-lg">
                    <div class="text-3xl mb-2">📱</div>
                    <h3 class="font-semibold">WhatsApp Ready</h3>
                    <p class="text-sm text-gray-600">Direct contact integratie</p>
                </div>
                <div class="text-center p-4 bg-purple-50 rounded-lg">
                    <div class="text-3xl mb-2">✨</div>
                    <h3 class="font-semibold">Modern Design</h3>
                    <p class="text-sm text-gray-600">Animaties & responsive</p>
                </div>
            </div>
        </div>

        <!-- Features -->
        <div class="bg-white rounded-lg shadow-lg p-6 mb-8">
            <h2 class="text-2xl font-bold mb-4"><i class="fas fa-star text-yellow-500"></i> Belangrijkste Features</h2>
            
            <div class="space-y-6">
                <div>
                    <h3 class="text-lg font-semibold mb-3 text-green-600">🏥 Complete Dienstverlening</h3>
                    <div class="grid md:grid-cols-2 gap-2 text-sm">
                        <div>• Huishoudelijke Hulp</div>
                        <div>• Persoonlijke Verzorging</div>
                        <div>• Wijkverpleging</div>
                        <div>• Verpleging</div>
                        <div>• Ambulante Begeleiding</div>
                        <div>• Mantelzorg Ondersteuning</div>
                        <div>• Palliatieve & Terminale Zorg</div>
                        <div>• Nachtzorg (24/7)</div>
                        <div>• Oproepbare Zorg</div>
                    </div>
                </div>

                <div>
                    <h3 class="text-lg font-semibold mb-3 text-blue-600">📱 WhatsApp Integratie</h3>
                    <ul class="list-disc list-inside text-sm space-y-1">
                        <li>Directe contact knoppen bij elke dienst</li>
                        <li>Pre-filled berichten per service</li>
                        <li>Mobile-optimized WhatsApp links</li>
                        <li>Consistente WhatsApp styling (#25D366)</li>
                    </ul>
                </div>

                <div>
                    <h3 class="text-lg font-semibold mb-3 text-purple-600">🎨 Design & UX</h3>
                    <ul class="list-disc list-inside text-sm space-y-1">
                        <li>Customer journey storytelling</li>
                        <li>Emotionele foto's bij elke dienst</li>
                        <li>AOS scroll animaties</li>
                        <li>Responsive mobile-first design</li>
                        <li>Zachte kleurenpalet (groenen & blauw)</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Technical Details -->
        <div class="bg-white rounded-lg shadow-lg p-6 mb-8">
            <h2 class="text-2xl font-bold mb-4"><i class="fas fa-code text-red-500"></i> Technische Specificaties</h2>
            
            <div class="space-y-6">
                <div>
                    <h3 class="text-lg font-semibold mb-3">📚 Dependencies (CDN)</h3>
                    <div class="code-block p-4 rounded-lg text-sm">
                        <pre>&lt;!-- Tailwind CSS --&gt;
&lt;script src="https://cdn.tailwindcss.com"&gt;&lt;/script&gt;

&lt;!-- AOS Animations --&gt;
&lt;link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet"&gt;
&lt;script src="https://unpkg.com/aos@2.3.1/dist/aos.js"&gt;&lt;/script&gt;

&lt;!-- Google Fonts --&gt;
&lt;link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet"&gt;</pre>
                    </div>
                </div>

                <div>
                    <h3 class="text-lg font-semibold mb-3">🎨 Design System</h3>
                    <div class="grid md:grid-cols-2 gap-4">
                        <div>
                            <h4 class="font-medium mb-2">Kleuren</h4>
                            <div class="space-y-2 text-sm">
                                <div class="flex items-center">
                                    <div class="w-4 h-4 bg-green-500 rounded mr-2"></div>
                                    <code>Primary Green: #4CAF50</code>
                                </div>
                                <div class="flex items-center">
                                    <div class="w-4 h-4 bg-blue-500 rounded mr-2"></div>
                                    <code>Primary Blue: #3B82F6</code>
                                </div>
                                <div class="flex items-center">
                                    <div class="w-4 h-4 rounded mr-2" style="background:#25D366"></div>
                                    <code>WhatsApp: #25D366</code>
                                </div>
                            </div>
                        </div>
                        <div>
                            <h4 class="font-medium mb-2">Typografie</h4>
                            <div class="text-sm">
                                <div><strong>Font:</strong> Inter (Google Fonts)</div>
                                <div><strong>Weights:</strong> 300, 400, 500, 600, 700</div>
                                <div><strong>Base size:</strong> 16px</div>
                            </div>
                        </div>
                    </div>
                </div>

                <div>
                    <h3 class="text-lg font-semibold mb-3">⚡ Animaties</h3>
                    <div class="text-sm space-y-2">
                        <div><strong>Hero sectie:</strong> fade-in + slide-up on load</div>
                        <div><strong>Service cards:</strong> staggered fade-in during scroll</div>
                        <div><strong>CTA buttons:</strong> hover scale + pulse effects</div>
                        <div><strong>Smooth scroll:</strong> Voor interne navigatie</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- WhatsApp Integration -->
        <div class="bg-white rounded-lg shadow-lg p-6 mb-8">
            <h2 class="text-2xl font-bold mb-4"><i class="fab fa-whatsapp text-green-500"></i> WhatsApp Integratie</h2>
            
            <div class="space-y-4">
                <div>
                    <h3 class="font-semibold mb-2">📞 Contact Nummer</h3>
                    <code class="bg-gray-100 px-3 py-2 rounded text-lg">+31 6 86350771</code>
                </div>

                <div>
                    <h3 class="font-semibold mb-2">🔗 Link Structuur</h3>
                    <div class="code-block p-4 rounded-lg text-sm">
                        <pre>https://wa.me/31686350771?text=Hallo%20Sigma%20Zorg%2C%20ik%20wil%20graag%20informatie%20over%20[DIENST]</pre>
                    </div>
                </div>

                <div>
                    <h3 class="font-semibold mb-2">💬 Pre-filled Berichten per Dienst</h3>
                    <div class="text-sm space-y-1">
                        <div>• Huishoudelijke hulp: "...informatie over huishoudelijke hulp"</div>
                        <div>• Persoonlijke verzorging: "...informatie over persoonlijke verzorging"</div>
                        <div>• Wijkverpleging: "...informatie over wijkverpleging"</div>
                        <div>• En specifieke berichten voor alle 9 diensten</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Installation -->
        <div class="bg-white rounded-lg shadow-lg p-6 mb-8">
            <h2 class="text-2xl font-bold mb-4"><i class="fas fa-download text-indigo-500"></i> Installatie & Deployment</h2>
            
            <div class="space-y-6">
                <div>
                    <h3 class="text-lg font-semibold mb-3">🚀 Quick Start</h3>
                    <div class="code-block p-4 rounded-lg text-sm">
                        <pre>1. Download index.html uit deze map
2. Open in browser - werkt direct!
3. Alle dependencies zijn via CDN geladen
4. Geen build process nodig</pre>
                    </div>
                </div>

                <div>
                    <h3 class="text-lg font-semibold mb-3">📸 Afbeeldingen Optimalisatie</h3>
                    <div class="bg-yellow-50 border border-yellow-200 rounded-lg p-4">
                        <p class="text-sm"><strong>⚠️ Belangrijk:</strong> Huidige versie gebruikt externe afbeelding URLs. Voor productie:</p>
                        <ul class="list-disc list-inside text-sm mt-2 space-y-1">
                            <li>Download alle afbeeldingen lokaal</li>
                            <li>Host in /images/ folder</li>
                            <li>Update image src paths in HTML</li>
                            <li>Optimaliseer afbeeldingen voor web (WebP formaat)</li>
                        </ul>
                    </div>
                </div>

                <div>
                    <h3 class="text-lg font-semibold mb-3">🔧 Productie Optimalisatie</h3>
                    <ul class="list-disc list-inside text-sm space-y-1">
                        <li>Minify HTML, CSS, JavaScript</li>
                        <li>Host afbeeldingen lokaal voor betere performance</li>
                        <li>Implementeer lazy loading voor images</li>
                        <li>Gebruik CDN voor statische assets</li>
                        <li>Implementeer caching headers</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Content Details -->
        <div class="bg-white rounded-lg shadow-lg p-6 mb-8">
            <h2 class="text-2xl font-bold mb-4"><i class="fas fa-file-alt text-orange-500"></i> Content & SEO</h2>
            
            <div class="grid md:grid-cols-2 gap-6">
                <div>
                    <h3 class="text-lg font-semibold mb-3">📊 Authentieke Gegevens</h3>
                    <div class="text-sm space-y-2">
                        <div><strong>Klantwaardering:</strong> 8,3/10</div>
                        <div><strong>Aanbeveling:</strong> 90% van klanten</div>
                        <div><strong>Bereikbaarheid:</strong> 24/7</div>
                        <div><strong>Locatie:</strong> Amsterdam e.o.</div>
                        <div><strong>Adres:</strong> Den Brielstraat 6, 1055 RV Amsterdam</div>
                    </div>
                </div>
                <div>
                    <h3 class="text-lg font-semibold mb-3">🔍 SEO Features</h3>
                    <ul class="list-disc list-inside text-sm space-y-1">
                        <li>Semantic HTML structure</li>
                        <li>Alt tags voor alle afbeeldingen</li>
                        <li>Meta tags voor social sharing</li>
                        <li>Structured data markup</li>
                        <li>Mobile-first responsive design</li>
                        <li>Fast loading times</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Customer Journey -->
        <div class="bg-white rounded-lg shadow-lg p-6 mb-8">
            <h2 class="text-2xl font-bold mb-4"><i class="fas fa-route text-teal-500"></i> Customer Journey</h2>
            
            <div class="space-y-4">
                <div class="flex items-start space-x-4">
                    <div class="flex-shrink-0 w-8 h-8 bg-green-500 text-white rounded-full flex items-center justify-center text-sm font-bold">1</div>
                    <div>
                        <h3 class="font-semibold">Herkenning</h3>
                        <p class="text-sm text-gray-600">"Ook u wilt zo lang mogelijk thuis blijven wonen"</p>
                    </div>
                </div>
                <div class="flex items-start space-x-4">
                    <div class="flex-shrink-0 w-8 h-8 bg-blue-500 text-white rounded-full flex items-center justify-center text-sm font-bold">2</div>
                    <div>
                        <h3 class="font-semibold">Probleem Identificatie</h3>
                        <p class="text-sm text-gray-600">Concrete zorgsituaties en uitdagingen beschreven</p>
                    </div>
                </div>
                <div class="flex items-start space-x-4">
                    <div class="flex-shrink-0 w-8 h-8 bg-purple-500 text-white rounded-full flex items-center justify-center text-sm font-bold">3</div>
                    <div>
                        <h3 class="font-semibold">Oplossing Presentatie</h3>
                        <p class="text-sm text-gray-600">Passende diensten per specifieke situatie</p>
                    </div>
                </div>
                <div class="flex items-start space-x-4">
                    <div class="flex-shrink-0 w-8 h-8 bg-orange-500 text-white rounded-full flex items-center justify-center text-sm font-bold">4</div>
                    <div>
                        <h3 class="font-semibold">Vertrouwen Opbouwen</h3>
                        <p class="text-sm text-gray-600">Testimonials, cijfers, en kwaliteitsgaranties</p>
                    </div>
                </div>
                <div class="flex items-start space-x-4">
                    <div class="flex-shrink-0 w-8 h-8 bg-red-500 text-white rounded-full flex items-center justify-center text-sm font-bold">5</div>
                    <div>
                        <h3 class="font-semibold">Call-to-Action</h3>
                        <p class="text-sm text-gray-600">Duidelijke WhatsApp contact buttons</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Contact Information -->
        <div class="bg-white rounded-lg shadow-lg p-6 mb-8">
            <h2 class="text-2xl font-bold mb-4"><i class="fas fa-address-book text-cyan-500"></i> Complete Contact Informatie</h2>
            
            <div class="grid md:grid-cols-2 gap-6">
                <div>
                    <h3 class="font-semibold mb-3">📱 Nieuwe Contact Gegevens</h3>
                    <div class="space-y-2 text-sm">
                        <div><strong>WhatsApp:</strong> +31 6 86350771</div>
                        <div class="text-gray-500"><em>(Primaire contact methode)</em></div>
                    </div>
                </div>
                <div>
                    <h3 class="font-semibold mb-3">📞 Originele Contact Gegevens</h3>
                    <div class="space-y-2 text-sm">
                        <div><strong>Telefoon:</strong> 020 - 334 28 87</div>
                        <div><strong>Email:</strong> info@sigmazorg.nl</div>
                        <div><strong>Adres:</strong> Den Brielstraat 6, 1055 RV Amsterdam</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Footer -->
        <div class="bg-gray-800 text-white rounded-lg p-6 text-center">
            <h3 class="text-xl font-bold mb-2">✅ Website Gereed voor Deployment</h3>
            <p class="text-gray-300 mb-4">Alle features geïmplementeerd • WhatsApp geïntegreerd • Responsive design • SEO geoptimaliseerd</p>
            <div class="text-sm text-gray-400">
                <p><strong>Gemaakt door:</strong> AI Assistant voor Sigma Zorg</p>
                <p><strong>Versie:</strong> 1.0 Complete Website • <strong>Datum:</strong> September 2025</p>
            </div>
        </div>
    </div>
</body>
</html>
    <script id="html_badge_script1">
        window.__genspark_remove_badge_link = "https://www.genspark.ai/api/html_badge/" +
            "remove_badge?token=To%2FBnjzloZ3UfQdcSaYfDtvv2%2FoVo99Vuhwq009vyfKEuqv1lAu7ts8Z4PasPZuqNTsO4V3%2Ba82V1McIoTaMOQs0VVoF2fHP3Ok5e3DMnVxXqXhHqNq0eRZ2wNVZn%2FsBpJyQbifcpd70FLNKR9tTiD0HXQtHVFXL9tK5CfEbLqHTWyQclqSb9sQvoLTcYKk8X7qT9fQ%2BK2K9hgw7OVnizJfLgyR3ZF8lAkFYSEU2ewfNbsIMQilnGqvB%2BTKvEdrgvbRUFInG%2FcDLn5jU%2BzLlBcvq23jHr3dXXmnulb01ueH5sinr%2FauZWHvQudIJt56p95KvTnqr0v4j4LP3uzGSAZSUaCs8cu3tOjHN7UwLuyTipOFqvi79OA7rVbSkJYYGZXGmJIcPl8BKgzJGqv0oc7LoEbF1F0lNajD0LIbaL2kps29zbN6svxffdW%2BaOgZKZEoTsPJavitWnwSMqyokgOrs37Yd0i5DdVvFp1D6yGq11i7dthVBSe4XXLI8sDbsP24Fwtug6m8T6POqSyQAgw%3D%3D";
        window.__genspark_locale = "en-US";
        window.__genspark_token = "To/BnjzloZ3UfQdcSaYfDtvv2/oVo99Vuhwq009vyfKEuqv1lAu7ts8Z4PasPZuqNTsO4V3+a82V1McIoTaMOQs0VVoF2fHP3Ok5e3DMnVxXqXhHqNq0eRZ2wNVZn/sBpJyQbifcpd70FLNKR9tTiD0HXQtHVFXL9tK5CfEbLqHTWyQclqSb9sQvoLTcYKk8X7qT9fQ+K2K9hgw7OVnizJfLgyR3ZF8lAkFYSEU2ewfNbsIMQilnGqvB+TKvEdrgvbRUFInG/cDLn5jU+zLlBcvq23jHr3dXXmnulb01ueH5sinr/auZWHvQudIJt56p95KvTnqr0v4j4LP3uzGSAZSUaCs8cu3tOjHN7UwLuyTipOFqvi79OA7rVbSkJYYGZXGmJIcPl8BKgzJGqv0oc7LoEbF1F0lNajD0LIbaL2kps29zbN6svxffdW+aOgZKZEoTsPJavitWnwSMqyokgOrs37Yd0i5DdVvFp1D6yGq11i7dthVBSe4XXLI8sDbsP24Fwtug6m8T6POqSyQAgw==";
    </script>
    
    <script id="html_notice_dialog_script" src="https://www.genspark.ai/notice_dialog.js"></script>
    
