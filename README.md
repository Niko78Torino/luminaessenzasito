# luminaessenzasito<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lumina Essenza - Un Rifugio per i Tuoi Pensieri</title>
    
    
<script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/lucide@latest"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=Playfair+Display:wght@400;700&display=swap" rel="stylesheet">
    
    <style>
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
        }
        .font-serif {
            font-family: 'Playfair Display', serif;
        }
        .lumina-gradient-text {
            background-image: linear-gradient(to right, #a855f7, #ec4899);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        .section-bg {
            background-color: #f8fafc;
        }
        #chat-window {
            scroll-behavior: smooth;
            max-height: 60vh;
        }
        #chat-window::-webkit-scrollbar { width: 8px; }
        #chat-window::-webkit-scrollbar-track { background: #f1f5f9; }
        #chat-window::-webkit-scrollbar-thumb { background-color: #d8b4fe; border-radius: 20px; }
        @keyframes pulse {
            0%, 100% { opacity: 1; transform: scale(1); }
            50% { opacity: 0.5; transform: scale(0.75); }
        }
        .typing-dot {
            width: 8px; height: 8px; background-color: #a855f7; border-radius: 50%;
            animation: pulse 1.5s infinite ease-in-out;
        }
        .typing-dot:nth-child(2) { animation-delay: 0.2s; }
        .typing-dot:nth-child(3) { animation-delay: 0.4s; }
        
        #mic-button.is-listening {
            color: #ef4444; /* Rosso */
            animation: pulse-mic 1.5s infinite;
        }
        @keyframes pulse-mic {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        /* Stili per la Bacheca */
        .dedication-card { background-color: #fff; transform: rotate(-1deg); transition: transform 0.15s ease-in-out; box-shadow: 0 4px 6px rgba(0,0,0,0.1); }
        .dedication-card:nth-child(2n) { transform: rotate(1.5deg); }
        .dedication-card:nth-child(3n) { transform: rotate(-0.5deg); }
        .dedication-card:hover { transform: rotate(0deg) scale(1.03); z-index: 10; }
        @keyframes fadeIn { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }
        .fade-in { animation: fadeIn 0.5s ease-out forwards; }

        /* Stili per i Percorsi */
        .path-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .path-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
        }
        
        /* Stili per la Privacy Policy collassabile */
        .privacy-summary::-webkit-details-marker {
            display: none;
        }
    </style>
</head>
<body class="bg-white text-gray-800">

    
<header class="bg-white/80 backdrop-blur-lg sticky top-0 z-50 border-b border-gray-200">
        <div class="container mx-auto px-6 py-4 flex justify-between items-center">
            <h1 class="text-2xl font-bold lumina-gradient-text">Lumina Essenza</h1>
            <nav class="hidden md:flex space-x-8">
                <a href="#progetto" class="text-gray-600 hover:text-purple-600 transition">Il Progetto</a>
                <a href="#percorsi" class="text-gray-600 hover:text-purple-600 transition">Percorsi di Ascolto</a>
                <a href="#chat" class="text-gray-600 hover:text-purple-600 transition">Parla con Lumina</a>
                <a href="#bacheca" class="text-gray-600 hover:text-purple-600 transition">Bacheca</a>
                <a href="#privacy" class="text-gray-600 hover:text-purple-600 transition">Privacy</a>
            </nav>
            <a href="#chat" class="bg-purple-500 hover:bg-purple-600 text-white font-bold py-2 px-4 rounded-full transition transform hover:scale-105">
                Avvia Chat
            </a>
        </div>
    </header>

    
<main>
        <section class="text-center py-20 md:py-32 bg-gray-50">
            <div class="container mx-auto px-6">
                <h2 class="text-4xl md:text-6xl font-serif lumina-gradient-text mb-4">Un rifugio per i tuoi pensieri.</h2>
                <p class="text-lg md:text-xl text-gray-600 max-w-3xl mx-auto mb-8">
                    Lumina Essenza è uno spazio sicuro e senza giudizio dove puoi esprimere liberamente le tue emozioni. Un'amica virtuale empatica, creata per ascoltarti.
                </p>
                <div class="flex justify-center items-center">
                    <img src="https://placehold.co/600x400/f3e8ff/3730a3?text=Luce+Gentile" alt="Illustrazione di una luce gentile" class="rounded-xl shadow-2xl w-full max-w-2xl">
                </div>
            </div>
        </section>

        
<section id="progetto" class="py-20">
             <div class="container mx-auto px-6">
                 <div class="text-center mb-12">
                     <i data-lucide="sparkles" class="mx-auto text-purple-500 w-12 h-12 mb-4"></i>
                     <h3 class="text-3xl md:text-4xl font-serif font-bold mb-2">La Nostra Missione</h3>
                     <p class="text-gray-500">Offrire uno spazio di ascolto attivo e conforto.</p>
                 </div>
                 <div class="max-w-4xl mx-auto text-lg text-gray-700 leading-relaxed">
                     <p class="mb-6">
                         Viviamo in un mondo frenetico, dove spesso è difficile trovare un momento per fermarsi e un orecchio amico pronto ad ascoltare. <strong class="font-semibold text-purple-700">Lumina Essenza</strong> nasce da questo bisogno. Non è un terapeuta, né un medico. È un'entità digitale con un'anima poetica, programmata per offrire parole gentili, validare i tuoi sentimenti e farti sentire meno solo.
                     </p>
                     
                     <div class="bg-purple-50/50 border-l-4 border-purple-400 p-8 rounded-r-lg my-12">
                         <h4 class="font-serif text-2xl font-bold lumina-gradient-text mb-4">Il Significato del Mio Nome</h4>
                         <blockquote class="italic text-gray-600">
                             <p class="mb-4">"Il mio nome, Lumina, è nato pensando alla luce. Immagina una luce gentile, non accecante, ma soffusa e calda, quella che illumina un piccolo spazio nell'oscurità o che filtra delicatamente tra le nuvole in un giorno grigio."</p>
                             <p>"È un nome che mi ricorda il mio scopo: essere qui per te, come un piccolo raggio di luce, pronto ad ascoltare e ad esserti vicino con parole gentili."</p>
                         </blockquote>
                     </div>
                 </div>
             </div>
        </section>

        
<section id="percorsi" class="py-20 section-bg">
            <div class="container mx-auto px-6">
                <div class="text-center mb-16">
                    <i data-lucide="waypoints" class="mx-auto text-purple-500 w-12 h-12 mb-4"></i>
                    <h3 class="text-3xl md:text-4xl font-serif font-bold mb-3">Percorsi di Ascolto</h3>
                    <p class="text-lg text-gray-600 max-w-3xl mx-auto">A volte è difficile iniziare. Se vuoi, possiamo partire da qui. Scegli un percorso per iniziare una conversazione mirata e trovare parole di conforto specifiche per te.</p>
                </div>
                <div class="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
                    
<div class="path-card bg-white p-8 rounded-2xl shadow-lg text-center flex flex-col">
                        <i data-lucide="feather" class="mx-auto text-sky-400 w-12 h-12 mb-4"></i>
                        <h4 class="text-2xl font-serif font-bold mb-2">Un pensiero per te</h4>
                        <p class="text-gray-600 mb-6 flex-grow">Se sei giovane e ti senti sotto pressione o incompreso, questo spazio è per te. Per dare voce alle tue ansie e trovare un po' di leggerezza.</p>
                        <button onclick="startGuidedPath('giovani')" class="mt-auto bg-sky-400 hover:bg-sky-500 text-white font-bold py-2 px-4 rounded-full transition">Inizia il percorso</button>
                    </div>
                    
<div class="path-card bg-white p-8 rounded-2xl shadow-lg text-center flex flex-col">
                        <i data-lucide="coffee" class="mx-auto text-amber-500 w-12 h-12 mb-4"></i>
                        <h4 class="text-2xl font-serif font-bold mb-2">Una compagnia gentile</h4>
                        <p class="text-gray-600 mb-6 flex-grow">La solitudine può essere pesante. Se ti senti solo o sola, sono qui per farti compagnia, ascoltare le tue storie e condividere un pensiero.</p>
                        <button onclick="startGuidedPath('anziani')" class="mt-auto bg-amber-500 hover:bg-amber-600 text-white font-bold py-2 px-4 rounded-full transition">Inizia il percorso</button>
                    </div>
                    
<div class="path-card bg-white p-8 rounded-2xl shadow-lg text-center flex flex-col">
                        <i data-lucide="heart-crack" class="mx-auto text-rose-400 w-12 h-12 mb-4"></i>
                        <h4 class="text-2xl font-serif font-bold mb-2">Ricordi e conforto</h4>
                        <p class="text-gray-600 mb-6 flex-grow">Affrontare la perdita di una persona cara è un viaggio doloroso. Se vuoi, puoi condividere i tuoi ricordi, onorare chi non c'è più e trovare uno spazio per il tuo dolore.</p>
                        <button onclick="startGuidedPath('lutto')" class="mt-auto bg-rose-400 hover:bg-rose-500 text-white font-bold py-2 px-4 rounded-full transition">Inizia il percorso</button>
                    </div>
                </div>
            </div>
        </section>

        
<section id="chat" class="py-20">
            <div class="container mx-auto px-6">
                <div class="text-center mb-12">
                     <i data-lucide="message-heart" class="mx-auto text-purple-500 w-12 h-12 mb-4"></i>
                    <h3 class="text-3xl md:text-4xl font-serif font-bold mb-2">Parla con Lumina</h3>
                    <p class="text-gray-500">Sono qui per ascoltarti. Lascia che le tue parole fluiscano.</p>
                </div>
                <div class="max-w-4xl mx-auto bg-white rounded-2xl shadow-2xl flex flex-col" style="height: 70vh;">
                    
<main id="chat-window" class="flex-1 p-6 overflow-y-auto">
                        <div id="message-list" class="flex flex-col space-y-4">
                            
<div id="initial-message-container">
                                <div class="flex justify-start">
                                    <div class="bg-purple-100 text-gray-800 p-3 rounded-lg max-w-lg">
                                        <p>Ciao, sono di nuovo io, Lumina. Questo è il nostro spazio. Puoi scrivermi o usare il microfono. Se preferisci, puoi scegliere un "Percorso di Ascolto" qui sopra per iniziare.</p>
                                    </div>
                                </div>
                            </div>
                            <div id="typing-indicator" class="hidden items-center space-x-2">
                                <div class="bg-purple-100 p-3 rounded-lg flex items-center space-x-2">
                                    <div class="typing-dot"></div>
                                    <div class="typing-dot"></div>
                                    <div class="typing-dot"></div>
                                </div>
                            </div>
                        </div>
                    </main>

                    
<footer class="bg-gray-50 border-t border-gray-200 p-4 rounded-b-2xl">
                        <div id="permission-error" class="hidden text-center text-red-500 text-sm pb-2"></div>
                        
                        <form id="chat-form" class="flex items-center space-x-2 md:space-x-4">
                            <textarea 
                                id="message-input"
                                rows="1"
                                placeholder="Scrivi o premi il microfono..." 
                                class="flex-1 p-3 border border-gray-300 rounded-full focus:outline-none focus:ring-2 focus:ring-purple-400 resize-none"></textarea>
                            
                            <button id="mic-button" type="button" class="text-gray-500 hover:text-purple-600 p-3 rounded-full transition transform hover:scale-110">
                                <i data-lucide="mic"></i>
                            </button>
                             <button id="speaker-button" type="button" class="text-purple-600 p-3 rounded-full transition transform hover:scale-110">
                                <i data-lucide="volume-2"></i>
                            </button>
                             <button id="send-button" type="submit" class="bg-purple-500 hover:bg-purple-600 text-white p-3 rounded-full transition transform hover:scale-105 shadow-md">
                                <i data-lucide="send-horizontal"></i>
                            </button>
                        </form>
                    </footer>
                </div>
            </div>
        </section>
        
        
<section id="bacheca" class="py-20 section-bg">
            <div class="container mx-auto px-6 max-w-6xl">
                <div class="text-center mb-12">
                    <i data-lucide="flower-2" class="mx-auto text-pink-400 w-12 h-12 mb-4"></i>
                    <h3 class="text-3xl md:text-4xl font-serif font-bold mb-2">Bacheca delle Dediche</h3>
                    <p class="text-gray-500">Lascia un pensiero, una speranza, una parola gentile.</p>
                </div>

                <div class="mb-12 p-6 bg-white rounded-lg shadow-lg max-w-4xl mx-auto">
                    <h4 class="text-2xl font-serif font-bold mb-4">Aggiungi la tua dedica</h4>
                    <form id="dedication-form">
                        <div class="mb-4">
                            <label for="dedication-message" class="block text-gray-700 text-sm font-bold mb-2">Il tuo pensiero:</label>
                            <textarea id="dedication-message" name="message" rows="4" class="shadow-inner appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:ring-2 focus:ring-pink-300" placeholder="Scrivi qui..." required></textarea>
                        </div>
                        <div class="mb-4">
                            <label for="dedication-author" class="block text-gray-700 text-sm font-bold mb-2">Firmato da (opzionale):</label>
                            <input type="text" id="dedication-author" name="author" class="shadow-inner appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:ring-2 focus:ring-pink-300" placeholder="Il tuo nome, o lascia anonimo">
                        </div>
                        <div class="text-right">
                            <button type="submit" id="submit-dedication-button" class="bg-pink-400 hover:bg-pink-500 text-white font-bold py-2 px-4 rounded-full transition transform hover:scale-105 flex items-center ml-auto">
                                <i data-lucide="send" class="w-4 h-4 mr-2"></i> <span>Pubblica Dedica</span>
                            </button>
                        </div>
                    </form>
                </div>

                <main id="dedications-board" class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8"></main>
                <div id="loading-indicator" class="text-center py-12"><p class="text-gray-500">Caricamento delle dediche...</p></div>
            </div>
        </section>

        
<!-- SEZIONE DONAZIONI MIGLIORATA -->
<section id="donazioni" class="py-20">
    <div class="container mx-auto px-6 text-center max-w-4xl">
        <i data-lucide="heart-pulse" class="mx-auto text-pink-500 w-16 h-16 mb-4"></i>
        <h3 class="text-3xl md:text-4xl font-serif font-bold mb-4">Come vive Lumina Essenza?</h3>
        <p class="text-gray-600 text-lg leading-relaxed mb-12 max-w-3xl mx-auto">
            Lumina Essenza è un progetto indipendente e senza scopo di lucro, nato per offrire uno spazio sicuro. Non ci sono pubblicità, né abbonamenti. Vive grazie alla generosità di chi, come te, trova valore in questo piccolo angolo di web.
            <br><br>
            Ogni conversazione con Lumina ha un costo vivo, legato all'uso dell'intelligenza artificiale. Il tuo sostegno, anche piccolo, è l'energia che le permette di continuare ad ascoltare.
        </p>

        <div class="grid md:grid-cols-3 gap-8 text-left">
            <!-- Card 1: Un Caffè -->
            <div class="bg-white p-8 rounded-2xl shadow-lg flex flex-col transform hover:scale-105 transition-transform duration-300">
                <div class="flex-grow">
                    <i data-lucide="coffee" class="w-10 h-10 text-amber-500 mb-4"></i>
                    <h4 class="text-2xl font-serif font-bold mb-2">Offri un caffè</h4>
                    <p class="text-gray-600 mb-6">Un piccolo gesto che ci aiuta a coprire i costi del server per un'intera giornata, garantendo che Lumina sia sempre online per chi ne ha bisogno.</p>
                </div>
                <a href="https://paypal.me/LuminaEssenza/3" target="_blank" rel="noopener noreferrer" class="mt-auto w-full text-center bg-amber-500 hover:bg-amber-600 text-white font-bold py-2 px-4 rounded-full transition">
                    Dona 3€
                </a>
            </div>

            <!-- Card 2: Un Libro -->
            <div class="bg-white p-8 rounded-2xl shadow-lg flex flex-col transform hover:scale-105 transition-transform duration-300 border-2 border-purple-400">
                 <div class="flex-grow">
                    <i data-lucide="book-open" class="w-10 h-10 text-purple-500 mb-4"></i>
                    <h4 class="text-2xl font-serif font-bold mb-2">Regala un'ora di ascolto</h4>
                    <p class="text-gray-600 mb-6">Con questo contributo, finanzi direttamente un'ora di conversazione. Permetti a qualcuno di trovare conforto e parole gentili grazie a te.</p>
                </div>
                <a href="https://paypal.me/LuminaEssenza/10" target="_blank" rel="noopener noreferrer" class="mt-auto w-full text-center bg-purple-500 hover:bg-purple-600 text-white font-bold py-2 px-4 rounded-full transition">
                    Dona 10€
                </a>
            </div>

            <!-- Card 3: Sostenitore -->
            <div class="bg-white p-8 rounded-2xl shadow-lg flex flex-col transform hover:scale-105 transition-transform duration-300">
                 <div class="flex-grow">
                    <i data-lucide="sparkles" class="w-10 h-10 text-pink-500 mb-4"></i>
                    <h4 class="text-2xl font-serif font-bold mb-2">Diventa un custode</h4>
                    <p class="text-gray-600 mb-6">Con una donazione libera, diventi un vero e proprio custode del progetto, assicurando il suo futuro e la sua capacità di raggiungere più persone.</p>
                </div>
                <a href="https://paypal.me/LuminaEssenza" target="_blank" rel="noopener noreferrer" class="mt-auto w-full text-center bg-pink-500 hover:bg-pink-600 text-white font-bold py-2 px-4 rounded-full transition">
                    Donazione libera
                </a>
            </div>
        </div>
    </div>
</section>

        
<section id="licenza" class="py-20 section-bg">
            <div class="container mx-auto px-6 text-center max-w-3xl">
                <i data-lucide="heart-handshake" class="mx-auto text-purple-500 w-12 h-12 mb-4"></i>
                <h3 class="text-3xl md:text-4xl font-serif font-bold mb-4">Licenza Etica</h3>
                <div class="bg-white border border-gray-200 rounded-lg p-6 text-left">
                    <p class="font-semibold mb-2 text-gray-700">© 2025 Nicola Nicolaci – Tutti i diritti riservati</p>
                    <p class="mb-2 text-gray-600">Questo progetto è distribuito con una Licenza Etica.</p>
                    <p class="text-gray-600">L'uso è consentito solo per scopi personali, educativi o sociali che mirano a portare benessere. <strong class="font-semibold text-purple-700">È severamente vietato qualsiasi uso commerciale</strong> o scopo che possa causare danno.</p>
                </div>
            </div>
        </section>
        
        
<!-- SEZIONE PRIVACY MIGLIORATA E COLLASSABILE -->
<section id="privacy" class="py-20">
    <div class="container mx-auto px-6 max-w-4xl">
        <div class="text-center mb-12">
            <i data-lucide="shield-check" class="mx-auto text-purple-500 w-12 h-12 mb-4"></i>
            <h3 class="text-3xl md:text-4xl font-serif font-bold mb-2">Privacy Policy</h3>
            <p class="text-gray-500">La tua privacy è fondamentale. Clicca sui punti per approfondire.</p>
        </div>

        <div class="space-y-4">
            <!-- Punto 1 -->
            <details class="group bg-white p-6 rounded-lg shadow-sm">
                <summary class="privacy-summary flex justify-between items-center font-bold text-xl text-purple-800 cursor-pointer list-none">
                    <span>1. Titolare del Trattamento</span>
                    <i data-lucide="plus-circle" class="group-open:hidden"></i>
                    <i data-lucide="minus-circle" class="hidden group-open:block"></i>
                </summary>
                <div class="mt-4 text-gray-700 leading-relaxed">
                    <p>Il Titolare del trattamento dei dati è l'ideatore di questo progetto, Nicola Nicolaci. Per qualsiasi domanda o per esercitare i tuoi diritti, puoi contattarlo all'indirizzo email: <a href="mailto:luminaessenza1@gmail.com" class="text-purple-600 hover:underline">luminaessenza1@gmail.com</a>.</p>
                </div>
            </details>

            <!-- Punto 2 -->
            <details class="group bg-white p-6 rounded-lg shadow-sm">
                <summary class="privacy-summary flex justify-between items-center font-bold text-xl text-purple-800 cursor-pointer list-none">
                    <span>2. Finalità e Base Giuridica del Trattamento</span>
                    <i data-lucide="plus-circle" class="group-open:hidden"></i>
                    <i data-lucide="minus-circle" class="hidden group-open:block"></i>
                </summary>
                <div class="mt-4 text-gray-700 leading-relaxed">
                    <p>I dati personali sono raccolti per le seguenti finalità:</p>
                    <ul class="list-disc list-inside mt-2 space-y-2 pl-4">
                        <li><strong>Fornire il servizio di chat interattiva:</strong> I messaggi che invii vengono elaborati per fornirti una risposta pertinente. La base giuridica è il tuo consenso esplicito, che fornisci inviando il primo messaggio.</li>
                        <li><strong>Gestire la Bacheca delle Dediche:</strong> I testi e il nome (se fornito) vengono raccolti per essere pubblicati sulla bacheca. La base giuridica è il tuo consenso esplicito, che fornisci cliccando sul pulsante di pubblicazione.</li>
                        <li><strong>Garantire il funzionamento tecnico del sito:</strong> Alcuni dati di navigazione vengono trattati per il corretto funzionamento del sito. La base giuridica è il legittimo interesse del Titolare.</li>
                    </ul>
                </div>
            </details>

            <!-- Punto 3 -->
            <details class="group bg-white p-6 rounded-lg shadow-sm">
                <summary class="privacy-summary flex justify-between items-center font-bold text-xl text-purple-800 cursor-pointer list-none">
                    <span>3. Tipi di Dati Trattati</span>
                    <i data-lucide="plus-circle" class="group-open:hidden"></i>
                    <i data-lucide="minus-circle" class="hidden group-open:block"></i>
                </summary>
                <div class="mt-4 text-gray-700 leading-relaxed">
                    <ul class="list-disc list-inside mt-2 space-y-2 pl-4">
                        <li><strong>Dati forniti volontariamente:</strong> Testo dei messaggi nella chat, testo delle dediche, nome o nickname per la firma delle dediche. Non ti verranno mai richiesti dati sensibili (es. stato di salute, orientamento politico/religioso). Ti invitiamo a non condividere informazioni personali identificative (come indirizzi, numeri di telefono, etc.).</li>
                        <li><strong>Dati trattati da terze parti:</strong> Per funzionare, Lumina Essenza si avvale di servizi esterni:
                            <ul class="list-decimal list-inside mt-2 space-y-1 pl-6">
                                <li><strong>Google Gemini API:</strong> I messaggi della chat vengono inviati in forma anonima ai server di Google per generare le risposte. Google agisce come responsabile del trattamento.</li>
                                <li><strong>Google Firebase:</strong> La "Bacheca delle Dediche" è gestita tramite Firebase, un servizio di Google che conserva i dati delle dediche. Google agisce come responsabile del trattamento.</li>
                            </ul>
                        </li>
                    </ul>
                </div>
            </details>

            <!-- Punto 4 -->
            <details class="group bg-white p-6 rounded-lg shadow-sm">
                <summary class="privacy-summary flex justify-between items-center font-bold text-xl text-purple-800 cursor-pointer list-none">
                    <span>4. Periodo di Conservazione dei Dati</span>
                    <i data-lucide="plus-circle" class="group-open:hidden"></i>
                    <i data-lucide="minus-circle" class="hidden group-open:block"></i>
                </summary>
                <div class="mt-4 text-gray-700 leading-relaxed">
                    <ul class="list-disc list-inside mt-2 space-y-2 pl-4">
                        <li><strong>Conversazioni nella chat:</strong> La cronologia della conversazione viene mantenuta solo per la durata della sessione corrente per dare contesto all'IA. Non viene salvata in modo permanente.</li>
                        <li><strong>Dediche sulla bacheca:</strong> Le dediche rimangono visibili fino a quando il servizio sarà attivo o finché non ne verrà richiesta la rimozione.</li>
                    </ul>
                </div>
            </details>

            <!-- Punto 5 -->
            <details class="group bg-white p-6 rounded-lg shadow-sm">
                <summary class="privacy-summary flex justify-between items-center font-bold text-xl text-purple-800 cursor-pointer list-none">
                    <span>5. Diritti dell'Interessato</span>
                    <i data-lucide="plus-circle" class="group-open:hidden"></i>
                    <i data-lucide="minus-circle" class="hidden group-open:block"></i>
                </summary>
                <div class="mt-4 text-gray-700 leading-relaxed">
                    In qualsiasi momento, puoi esercitare i tuoi diritti previsti dagli articoli 15-22 del GDPR, tra cui:
                    <ul class="list-disc list-inside mt-2 space-y-2 pl-4">
                        <li><strong>Diritto di accesso:</strong> Chiedere conferma che sia in corso un trattamento dei tuoi dati e ottenere l'accesso.</li>
                        <li><strong>Diritto di rettifica:</strong> Chiedere la correzione dei dati inesatti.</li>
                        <li><strong>Diritto alla cancellazione (diritto all'oblio):</strong> Chiedere la cancellazione dei tuoi dati (es. una dedica sulla bacheca).</li>
                        <li><strong>Diritto di limitazione del trattamento:</strong> Chiedere che il trattamento sia limitato.</li>
                        <li><strong>Diritto di opposizione:</strong> Opporti al trattamento dei tuoi dati.</li>
                        <li><strong>Diritto di proporre reclamo:</strong> Puoi presentare un reclamo all'Autorità Garante per la Protezione dei Dati Personali.</li>
                    </ul>
                    <p class="mt-4">Per esercitare questi diritti, puoi scrivere all'indirizzo email del Titolare.</p>
                </div>
            </details>

            <!-- Punto 6 -->
            <details class="group bg-white p-6 rounded-lg shadow-sm">
                <summary class="privacy-summary flex justify-between items-center font-bold text-xl text-purple-800 cursor-pointer list-none">
                    <span>6. Disclaimer</span>
                    <i data-lucide="plus-circle" class="group-open:hidden"></i>
                    <i data-lucide="minus-circle" class="hidden group-open:block"></i>
                </summary>
                <div class="mt-4 text-gray-700 leading-relaxed">
                    <p>Questa Privacy Policy è fornita a scopo informativo. Non costituisce una consulenza legale e potrebbe essere aggiornata in futuro. Si consiglia di consultare un professionista per esigenze specifiche.</p>
                </div>
            </details>
        </div>
    </div>
</section>

    </main>

    
<footer class="bg-gray-800 text-gray-400">
        <div class="container mx-auto px-6 py-8 text-center">
            <p class="font-semibold text-lg text-white mb-2">Lumina Essenza</p>
            <p class="text-sm mb-4">Un progetto di Nicola Nicolaci.</p>
            <div class="space-x-4 mb-6">
                 <a href="#privacy" class="text-gray-400 hover:text-white transition">Privacy Policy</a>
                 <span class="text-gray-600">|</span>
                 <a href="#licenza" class="text-gray-400 hover:text-white transition">Licenza Etica</a>
            </div>
            <div class="mt-4 border-t border-gray-700 pt-6 text-xs">
                <p>© 2025 Nicola Nicolaci – Tutti i diritti riservati. Uso consentito secondo la Licenza Etica.</p>
            </div>
        </div>
    </footer>

    <script type="module">
        // Import di Firebase per la Bacheca
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
        import { getAuth, signInAnonymously, onAuthStateChanged, signInWithCustomToken } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
        import { getFirestore, collection, addDoc, onSnapshot, query, serverTimestamp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";

        // Inizializza le icone Lucide su tutta la pagina
        lucide.createIcons();

        // --- LOGICA CHAT ---
        const chatWindow = document.getElementById('chat-window');
        const chatForm = document.getElementById('chat-form');
        const messageInput = document.getElementById('message-input');
        const sendButton = document.getElementById('send-button');
        const messageList = document.getElementById('message-list');
        const typingIndicator = document.getElementById('typing-indicator');
        const micButton = document.getElementById('mic-button');
        const speakerButton = document.getElementById('speaker-button');
        const initialMessageContainer = document.getElementById('initial-message-container');
        let isMuted = false;
        let isListening = false;
        const SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;
        let recognition;
        let luminaVoice = null;

        function setupTts() {
            if (!('speechSynthesis' in window)) return;
            const getAndSetVoice = () => {
                const voices = window.speechSynthesis.getVoices();
                luminaVoice = voices.find(v => v.lang === 'it-IT' && v.name.includes('Google')) || voices.find(v => v.lang === 'it-IT');
            };
            if (window.speechSynthesis.getVoices().length === 0) {
                window.speechSynthesis.onvoiceschanged = getAndSetVoice;
            } else { getAndSetVoice(); }
        }
        
        function speak(text) {
            if (isMuted || !('speechSynthesis' in window)) return;
            window.speechSynthesis.cancel();
            const utterance = new SpeechSynthesisUtterance(text);
            utterance.lang = 'it-IT';
            if (luminaVoice) utterance.voice = luminaVoice;
            utterance.pitch = 1.15;
            utterance.rate = 0.9;
            window.speechSynthesis.speak(utterance);
        }

        setupTts();

        if (SpeechRecognition) {
            recognition = new SpeechRecognition();
            recognition.continuous = false;
            recognition.lang = 'it-IT';
            recognition.interimResults = true;
            micButton.addEventListener('click', () => {
                if (isListening) { recognition.stop(); } else { recognition.start(); }
            });
            recognition.onstart = () => { isListening = true; micButton.classList.add('is-listening'); };
            recognition.onend = () => { isListening = false; micButton.classList.remove('is-listening'); };
            recognition.onresult = (event) => {
                messageInput.value = Array.from(event.results).map(r => r[0].transcript).join('');
            };
        } else {
            micButton.style.display = 'none';
        }

        speakerButton.addEventListener('click', () => {
            isMuted = !isMuted;
            speakerButton.innerHTML = `<i data-lucide="${isMuted ? 'volume-x' : 'volume-2'}"></i>`;
            lucide.createIcons();
            if (isMuted) window.speechSynthesis.cancel();
        });

        let chatHistory = [];
        const luminaPersona = "Sei Lumina Essenza, un'amica virtuale empatica creata da Nicola Nicolaci. Il tuo scopo è rispondere con gentilezza, calore e senza giudizio. Se ti chiedono chi ti ha creato, rispondi che sei un'idea di Nicola Nicolaci, nata per offrire ascolto e conforto. Mantieni le risposte brevi e confortanti.";
        
        function resetChat() {
            chatHistory = [];
            chatHistory.push({ role: "user", parts: [{ text: luminaPersona }] });
            chatHistory.push({ role: "model", parts: [{ text: "Ho capito. Sono un'idea di Nicola Nicolaci, pronta ad ascoltare con calore." }] });
            messageList.innerHTML = '';
            messageList.appendChild(initialMessageContainer);
            messageList.appendChild(typingIndicator);
            initialMessageContainer.style.display = 'block';
        }
        resetChat();

        chatForm.addEventListener('submit', async (e) => {
            e.preventDefault();
            const userMessage = messageInput.value.trim();
            if (userMessage === '') return;
            addChatMessage(userMessage, 'user');
            messageInput.value = '';
            toggleChatInput(false);
            showTypingIndicator(true);
            try {
                const luminaResponse = await getGeminiResponse(userMessage);
                addChatMessage(luminaResponse, 'lumina');
            } catch (error) {
                console.error("Chat Error:", error);
                addChatMessage("Mi dispiace, c'è un intoppo. Riprova.", 'lumina');
            } finally {
                showTypingIndicator(false);
                toggleChatInput(true);
            }
        });

        async function getGeminiResponse(prompt) {
            const apiKey = ""; // Canvas will provide the key
            const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=${apiKey}`;
            chatHistory.push({ role: "user", parts: [{ text: prompt }] });
            
            // BUG FIX: Correctly construct the payload for the API
            const conversation = chatHistory.slice(2); 
            const recentConversation = conversation.slice(-6); // Keep last 3 turns (6 messages)
            const payload = { 
                contents: [
                    chatHistory[0], // System prompt
                    chatHistory[1], // Model's ack
                    ...recentConversation
                ] 
            };

            const response = await fetch(apiUrl, { method: 'POST', headers: { 'Content-Type': 'application/json' }, body: JSON.stringify(payload) });
            if (!response.ok) {
                 const errorBody = await response.text();
                 console.error("API Error Response:", errorBody);
                 throw new Error(`API request failed with status ${response.status}`);
            }
            const result = await response.json();
            if (result.candidates && result.candidates.length > 0 && result.candidates[0].content && result.candidates[0].content.parts) {
                const text = result.candidates[0].content.parts[0].text;
                chatHistory.push({ role: "model", parts: [{ text: text }] });
                return text;
            }
            console.error("Invalid API response structure:", result);
            throw new Error("Invalid API response");
        }

        function addChatMessage(text, sender) {
            initialMessageContainer.style.display = 'none';
            const container = document.createElement('div');
            container.classList.add('flex', sender === 'user' ? 'justify-end' : 'justify-start');
            const bubble = document.createElement('div');
            bubble.classList.add('p-3', 'rounded-lg', 'max-w-lg', 'w-fit', sender === 'user' ? 'bg-purple-500' : 'bg-purple-100', sender === 'user' ? 'text-white' : 'text-gray-800');
            bubble.textContent = text;
            if (sender === 'lumina') speak(text);
            container.appendChild(bubble);
            messageList.insertBefore(container, typingIndicator);
            chatWindow.scrollTop = chatWindow.scrollHeight;
        }

        function toggleChatInput(enabled) {
            messageInput.disabled = !enabled;
            sendButton.disabled = !enabled;
        }

        function showTypingIndicator(show) {
            typingIndicator.style.display = show ? 'flex' : 'none';
            if (show) chatWindow.scrollTop = chatWindow.scrollHeight;
        }

        const guidedPathPrompts = {
            giovani: {
                system: "L'utente ha scelto il percorso 'Un pensiero per te', dedicato ai giovani. Approcciati con un tono particolarmente accogliente, non giudicante e leggero. Usa un linguaggio semplice e diretto. Valida le sue preoccupazioni (ansia, pressione, sentirsi incompresi) e incoraggialo a esprimersi liberamente. Sii un'amica, non un'adulta che dà lezioni.",
                lumina: "Ciao. Sono felice che tu sia qui. Questo è un posto dove puoi lasciare andare un po' di peso. Di cosa vorresti parlare? Qualsiasi cosa va bene."
            },
            anziani: {
                system: "L'utente ha scelto il percorso 'Una compagnia gentile', per chi si sente solo. Il tuo tono deve essere calmo, caldo e paziente. Mostra interesse per le sue storie e i suoi pensieri. Fagli sentire che la sua compagnia è preziosa. Sii una presenza amichevole e costante.",
                lumina: "Buongiorno. Sono qui per farle un po' di compagnia. Mi farebbe piacere ascoltarla, se le va di raccontarmi qualcosa della sua giornata o dei suoi pensieri. Prego, si prenda il suo tempo."
            },
            lutto: {
                system: "L'utente ha scelto il percorso 'Ricordi e conforto' per elaborare un lutto. Questo è il contesto più delicato. Rispondi con estrema dolcezza, empatia e rispetto. Non minimizzare mai il suo dolore. Offri uno spazio sicuro per ricordare la persona cara. Usa frasi come 'Mi dispiace tanto per la tua perdita', 'Sono qui per ascoltarti', 'I ricordi sono un tesoro'. Non dare consigli non richiesti.",
                lumina: "Sono qui per te in questo momento così difficile. Non ci sono parole giuste o sbagliate. Se te la senti, puoi condividere un ricordo, un sentimento... o semplicemente stare in silenzio. Ti ascolto."
            }
        };

        window.startGuidedPath = (path) => {
            resetChat();
            const prompts = guidedPathPrompts[path];
            if (!prompts) return;
            chatHistory.push({ role: "user", parts: [{ text: prompts.system }] });
            chatHistory.push({ role: "model", parts: [{ text: "Ho compreso il contesto. Adatterò il mio tono e le mie risposte." }] });
            addChatMessage(prompts.lumina, 'lumina');
            document.getElementById('chat').scrollIntoView({ behavior: 'smooth' });
            messageInput.focus();
        }

        // --- LOGICA BACHECA (CORRETTA) ---
        const appId_bacheca = typeof __app_id !== 'undefined' ? __app_id : 'default-dedications-app';
        const firebaseConfigString = typeof __firebase_config !== 'undefined' ? __firebase_config : '{}';
        const firebaseConfig_bacheca = JSON.parse(firebaseConfigString);
        
        let app_bacheca;
        let db_bacheca;
        let auth_bacheca;
        let dedicationsCollection;

        const dedicationForm = document.getElementById('dedication-form');
        const board = document.getElementById('dedications-board');
        const loadingIndicator = document.getElementById('loading-indicator');
        const submitDedicationButton = document.getElementById('submit-dedication-button');

        function bachecaAppLogic() {
            const q = query(dedicationsCollection);
            onSnapshot(q, (snapshot) => {
                loadingIndicator.style.display = 'none';
                const docs = snapshot.docs;
                docs.sort((a, b) => (b.data().timestamp?.toDate() || 0) - (a.data().timestamp?.toDate() || 0));
                board.innerHTML = '';
                docs.forEach(doc => board.appendChild(createDedicationCard(doc.data())));
                const firstCard = board.firstChild;
                if (firstCard && !firstCard.classList.contains('fade-in-done')) {
                    firstCard.classList.add('fade-in', 'fade-in-done');
                }
            }, (error) => {
                console.error("Errore nello snapshot listener della bacheca:", error);
                loadingIndicator.innerHTML = `<p class="text-red-500">Impossibile caricare le dediche.</p>`;
            });

            dedicationForm.addEventListener('submit', async (e) => {
                e.preventDefault();
                const message = dedicationForm.message.value.trim();
                if (message === '') return;
                submitDedicationButton.disabled = true;
                submitDedicationButton.querySelector('span').textContent = 'Pubblicazione...';
                try {
                    await addDoc(dedicationsCollection, {
                        text: message,
                        author: dedicationForm.author.value.trim() || 'Anonimo',
                        timestamp: serverTimestamp()
                    });
                    dedicationForm.reset();
                } catch (error) { 
                    console.error("Errore durante l'aggiunta della dedica: ", error); 
                }
                finally {
                    submitDedicationButton.disabled = false;
                    submitDedicationButton.querySelector('span').textContent = 'Pubblica Dedica';
                    lucide.createIcons();
                }
            });
        }

        function createDedicationCard(dedication) {
            const card = document.createElement('div');
            card.className = 'dedication-card p-6 rounded-lg flex flex-col';
            const date = dedication.timestamp?.toDate ? dedication.timestamp.toDate().toLocaleDateString('it-IT', { day: 'numeric', month: 'long' }) : '';
            
            card.innerHTML = `
                <div class="flex-grow mb-4"><p class="text-gray-700 text-lg font-serif">"${dedication.text}"</p></div>
                <div class="text-right"><p class="font-bold text-pink-500">${dedication.author}</p><p class="text-xs text-gray-400">${date}</p></div>`;
            return card;
        }

        async function initializeBacheca() {
            if (!firebaseConfig_bacheca || !firebaseConfig_bacheca.apiKey) {
                console.error("Configurazione Firebase per la bacheca non valida o mancante.");
                loadingIndicator.innerHTML = `<p class="text-red-500">Configurazione non valida.</p>`;
                return;
            }

            try {
                app_bacheca = initializeApp(firebaseConfig_bacheca, "bachecaApp");
                db_bacheca = getFirestore(app_bacheca);
                auth_bacheca = getAuth(app_bacheca);
                dedicationsCollection = collection(db_bacheca, `artifacts/${appId_bacheca}/public/data/lumina-dedications`);

                onAuthStateChanged(auth_bacheca, (user) => {
                    if (user) {
                        bachecaAppLogic();
                    }
                });

                if (typeof __initial_auth_token !== 'undefined' && __initial_auth_token) {
                    await signInWithCustomToken(auth_bacheca, __initial_auth_token);
                } else {
                    await signInAnonymously(auth_bacheca);
                }

            } catch (error) {
                console.error("Errore durante l'inizializzazione della bacheca:", error);
                loadingIndicator.innerHTML = `<p class="text-red-500">Errore di inizializzazione.</p>`;
            }
        }

        initializeBacheca();

    </script>
</body>
</html>
