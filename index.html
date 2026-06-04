<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Évaluation d'Habilitation HT/THT - STOS Sonelgaz</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Tajawal:wght@500;700;800&display=swap'); 
        
        body { font-family: 'Inter', sans-serif; background-color: #f1f5f9; }
        .font-arabic { font-family: 'Tajawal', sans-serif; }
        .fade-in { animation: fadeIn 0.3s ease-out forwards; }
        @keyframes fadeIn { from { opacity: 0; transform: translateY(15px); } to { opacity: 1; transform: translateY(0); } }
        
        .radio-custom:checked + label { background-color: #eff6ff; border-color: #0072ce; box-shadow: 0 4px 6px -1px rgba(0, 114, 206, 0.1); }
        .radio-custom:checked + label .radio-circle { border-color: #0072ce; background-color: #0072ce; }
        
        .custom-scrollbar::-webkit-scrollbar { width: 6px; height: 6px;}
        .custom-scrollbar::-webkit-scrollbar-track { background: #f1f1f1; border-radius: 4px; }
        .custom-scrollbar::-webkit-scrollbar-thumb { background: #cbd5e1; border-radius: 4px; }
        
        .bg-sonelgaz-blue { background-color: #0072ce; }
        .text-sonelgaz-blue { color: #0072ce; }
        .border-sonelgaz-blue { border-color: #0072ce; }
        .bg-sonelgaz-orange { background-color: #f39200; }
        
        .tab-active { border-bottom: 3px solid #0072ce; color: #0072ce; font-weight: 700; }
        .tab-inactive { border-bottom: 3px solid transparent; color: #64748b; font-weight: 500; }

        /* Style Webcam & Visio */
        #webcam-container {
            position: fixed; bottom: 20px; right: 20px; width: 240px; height: 180px;
            background: #1e293b; border-radius: 12px; box-shadow: 0 10px 25px rgba(0,0,0,0.5);
            border: 3px solid #f39200; overflow: hidden; z-index: 50; display: none; transition: all 0.3s ease;
        }
        #webcam-container:hover { transform: scale(1.05); }
        #webcam-video { width: 100%; height: 100%; object-fit: cover; transform: scaleX(-1); }
        .recording-indicator {
            position: absolute; top: 10px; left: 10px; background: rgba(0,0,0,0.6);
            padding: 4px 8px; border-radius: 20px; display: flex; align-items: center; gap: 6px; color: white; font-size: 10px; font-weight: bold;
        }
        .recording-dot { width: 8px; height: 8px; background-color: #ef4444; border-radius: 50%; animation: pulse 1.5s infinite; }
        #audio-level { position: absolute; bottom: 10px; right: 10px; width: 10px; height: 40px; background: rgba(255,255,255,0.2); border-radius: 5px; overflow: hidden; }
        #audio-bar { width: 100%; height: 0%; background: #22c55e; transition: height 0.1s ease; position: absolute; bottom: 0; }
        
        @media print {
            body { background: white; }
            .no-print { display: none !important; }
            #app-container { max-width: 100% !important; margin: 0; padding: 0; box-shadow: none; border: none; }
        }
    </style>
</head>
<body class="text-gray-800 antialiased min-h-screen flex flex-col selection:bg-sonelgaz-orange selection:text-white relative">

    <!-- CHRONOMÈTRE GLOBAL -->
    <div id="global-timer" class="hidden fixed top-2 right-2 sm:top-5 sm:right-5 z-40 bg-red-600 text-white font-mono font-bold text-lg sm:text-2xl px-4 sm:px-6 py-2 sm:py-3 rounded-xl shadow-2xl border-4 border-white flex items-center gap-3 no-print">
        <i class="fas fa-stopwatch animate-pulse"></i>
        <span id="timer-display">01:00:00</span>
    </div>

    <!-- WEBCAM CONTAINER (VISIO) -->
    <div id="webcam-container" class="no-print">
        <video id="webcam-video" autoplay muted playsinline></video>
        <div class="recording-indicator"><div class="recording-dot"></div> EXAMEN SURVEILLÉ (REC)</div>
        <div id="audio-level" title="Niveau du microphone"><div id="audio-bar"></div></div>
    </div>

    <!-- CUSTOM MODAL -->
    <div id="custom-modal" class="hidden fixed inset-0 bg-slate-900/80 z-50 flex items-center justify-center fade-in no-print">
        <div class="bg-white rounded-2xl p-8 max-w-sm w-full mx-4 shadow-2xl text-center border-t-4 border-sonelgaz-orange">
            <div id="modal-icon" class="w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4 text-2xl"></div>
            <h3 id="modal-title" class="text-xl font-bold text-slate-800 mb-2">Titre</h3>
            <p id="modal-message" class="text-sm text-slate-500 mb-6">Message</p>
            <div id="modal-buttons" class="flex gap-3 justify-center"></div>
        </div>
    </div>

    <header class="bg-white border-b-4 border-sonelgaz-blue shadow-sm py-3 px-4 sm:px-6 flex justify-between items-center sticky top-0 z-30 no-print">
        <div class="flex items-center gap-3 sm:gap-5">
            <div id="logo-container" class="relative shrink-0 flex items-center justify-center bg-white rounded-lg shadow-sm border border-slate-100 h-12 w-12 sm:h-16 sm:w-16 overflow-hidden">
                <img src="logo.png" alt="Sonelgaz Logo" class="w-full h-full object-contain z-10" id="main-logo" onerror="document.getElementById('main-logo').style.display='none'; document.getElementById('svg-logo').style.display='block';">
                <svg id="svg-logo" style="display:none;" viewBox="0 0 100 100" class="w-full h-full rounded">
                    <rect width="100" height="100" fill="#f39200"/><path d="M 20 60 L 45 20 L 60 20 L 40 50 L 75 50 L 50 85 L 65 85 L 85 45 L 80 40 L 50 40 Z" fill="#0072ce"/><circle cx="60" cy="25" r="7" fill="#0072ce"/><circle cx="80" cy="25" r="7" fill="#0072ce"/>
                </svg>
            </div>
            <div class="flex flex-col justify-center">
                <span class="text-sonelgaz-blue font-bold text-sm sm:text-lg md:text-xl font-arabic leading-tight tracking-wide">الشركة الجزائرية للكهرباء و الغاز - نقل الكهرباء و مسير المنظومة</span>
                <span class="text-sonelgaz-blue font-semibold text-[10px] sm:text-xs md:text-sm mt-0.5 leading-tight">Société algérienne de l'électricité et du gaz - Transport électricité et opérateur système</span>
            </div>
        </div>
        <button onclick="window.showAdminLogin()" class="ml-4 text-slate-400 hover:text-sonelgaz-blue transition flex flex-col items-center shrink-0 p-2 rounded-xl hover:bg-slate-50 border border-transparent hover:border-slate-200">
            <i class="fas fa-lock text-lg"></i><span class="text-[10px] font-bold mt-1 tracking-widest">ADMIN</span>
        </button>
    </header>

    <main id="app-container" class="flex-grow flex items-center justify-center p-4 sm:p-6 w-full max-w-6xl mx-auto"></main>

    <footer class="bg-white border-t border-gray-200 py-4 text-center text-xs sm:text-sm text-gray-500 font-medium no-print">
        &copy; 2026 - Plateforme d'Évaluation Pédagogique - STOS Sonelgaz
    </footer>

    <script>
        const districts = ["ORAN", "MOSTAGANEM", "SIDI BELABES", "TIARET", "MASCARA", "TLEMCEN", "AIN TEMOUCHENT"];
        const services = ["Exploitation", "Contrôle électrique", "Maintenance Poste", "Maintenance Ligne (ML)", "CE ESSAIS/ANALYSES", "Télécom & Téléconduite"];
        
        /* ================= BANQUES DE DONNÉES COMPLÈTES (SÉPARÉES) ================= */

        // 1. EXPLOITATION (Réseau, Consignation, Manœuvres, CGE)
        const poolExploitation = [
            { theme: "Procédure & OT", type: "Épreuve Écrite", question: "Une équipe se présente pour une intervention urgente. Le Chef de Travaux (CDT) n'a pas d'Ordre de Travail (OT). Que doit faire le CC ?", options: ["L'accepter avec accord verbal.", "Rédiger l'OT.", "Refuser toute consignation jusqu'à présentation de l'OT.", "Délivrer l'AT sous condition."], correctIndex: 2, justification: "L'OT est le document juridique de base sans lequel l'intervention n'existe pas." },
            { theme: "Faute d'Exploitation", type: "Épreuve Écrite", question: "Suite à une surcharge, le Chef de Consignation effectue un transfert de charge sans informer le Dispatching. Qualification ?", options: ["Initiative proactive.", "Routine.", "Faute grave d'exploitation.", "Toléré de jour."], correctIndex: 2, justification: "Seul le Dispatching a l'autorité sur la topologie du réseau." },
            { theme: "Communication", type: "Épreuve Écrite", question: "Le Dispatching ordonne l'ouverture. Le Chef de Poste répond : « D'accord j'ouvre ». Quelle règle de sécurité manque ?", options: ["Dire Terminé.", "Le message collationné (répétition intégrale).", "L'envoi d'un fax.", "Aucune."], correctIndex: 1, justification: "Le collationnement est obligatoire pour éviter les fausses manœuvres." },
            { theme: "Habilitation", type: "Épreuve Écrite", question: "Un agent habilité 'HC' peut-il réparer physiquement un disjoncteur ?", options: ["Oui.", "Oui s'il est seul.", "Non, il faut une habilitation H2 (Travaux).", "Oui avec des gants isolants."], correctIndex: 2, justification: "HC = Consignation uniquement. H2 = Réalisation de travaux." },
            { theme: "Manœuvres", type: "Épreuve Écrite", question: "Un Chef de Poste exécute l'ouverture d'un sectionneur de mémoire, sans cocher sa Fiche de Manœuvre. Conclusion ?", options: ["Oubli administratif.", "Sectionneur défectueux.", "Faute grave de manque de suivi pas-à-pas.", "Toléré."], correctIndex: 2, justification: "Le travail de mémoire est la cause numéro 1 des fausses manœuvres en HT." },
            { theme: "Règles d'Or", type: "Simulation", question: "Le CDT a reçu l'AT et dit à son équipe de monter sur le pylône. Quelle étape vitale a-t-il oublié ?", options: ["Météo non vérifiée.", "Oubli de la Vérification d'Absence de Tension (VAT) et de la pose des MALT locales (Chantier).", "Pas de casque.", "Aucune."], correctIndex: 1, justification: "La VAT et les terres de chantier sont la responsabilité absolue du CDT pour protéger ses hommes." },
            { theme: "Alarme SF6", type: "Simulation", question: "Sur un disjoncteur 400kV, l'alarme 'SF6 2ème Stade (Lockout)' retentit. Un défaut réseau survient. Que faire ?", options: ["Ouvrir manuellement le disjoncteur.", "Forcer la commande électrique.", "Isoler la travée via les disjoncteurs adjacents (Protection 50BF).", "Fermer les sectionneurs de terre."], correctIndex: 2, justification: "Le disjoncteur est verrouillé (Lockout) pour éviter une explosion mortelle car le gaz ne peut plus éteindre l'arc." },
            { theme: "Transformateur", type: "Simulation", question: "Alarme Température huile Transfo Très Haute. Les ventilateurs sont à l'arrêt. Action prioritaire ?", options: ["Arroser d'eau.", "Demander un délestage immédiat au Dispatching pour réduire la charge.", "Mettre le régleur au minimum.", "Couper le neutre."], correctIndex: 1, justification: "Sans ventilation forcée, le transformateur perd 30% de sa capacité. Le délestage sauve l'appareil." },
            { theme: "RSE (Régime Spécial)", type: "Épreuve Écrite", question: "Quel est l'objectif du Régime Spécial d'Exploitation (RSE) ?", options: ["Augmenter le transit.", "Empêcher tout réenclenchement (bloquer le 79) pour protéger les agents en Travaux Sous Tension (TST).", "Refroidir les câbles.", "Délestage automatique."], correctIndex: 1, justification: "Le RSE protège les équipes TST des réenclenchements automatiques ou volontaires en cas de défaut." },
            { theme: "Incendie", type: "Simulation", question: "Feu déclaré sur un transformateur HT. Les gicleurs sont inopérants. Première action ?", options: ["Utiliser un extincteur à eau.", "S'assurer par VAT qu'il est HORS TENSION avant la lutte.", "Attendre les pompiers.", "Mettre du sable."], correctIndex: 1, justification: "Ne jamais projeter d'eau sur une installation électrique non séparée des sources." },
            { theme: "VCC (Courant Continu)", type: "Simulation", question: "Perte totale du courant continu (127 VCC) au poste. Quel est le risque majeur ?", options: ["Perte d'éclairage.", "Perte totale du contrôle-commande et protections. Risque d'explosion du poste si un défaut réseau survient.", "Perte du téléphone.", "Perte de la climatisation."], correctIndex: 1, justification: "Le VCC alimente les relais et les bobines d'ouverture. Sans lui, le poste est paralysé." },
            { theme: "Blackout", type: "Simulation", question: "En cas de Blackout total (Zéro tension), quelle est la première action de l'exploitant dans le poste ?", options: ["Attendre le Dispatching.", "Ouvrir impérativement tous les disjoncteurs (mise à plat) pour éviter un choc lors du retour de tension.", "Démarrer le groupe diesel.", "Fermer les sectionneurs de terre."], correctIndex: 1, justification: "La mise à plat empêche un 'Inrush' massif qui ferait redéclencher le réseau lors de sa reconstitution." },
            { theme: "Couplage de Réseaux", type: "Épreuve Écrite", question: "Quelle est la condition de fréquence pour réaliser un couplage (reprise de parallèle) normal ?", options: ["Écart > 0.5 Hz.", "Écart inférieur ou égal à 0.2 Hz.", "Écart = 1 Hz.", "Pas d'importance."], correctIndex: 1, justification: "Un écart de glissement supérieur à 0.2 Hz créerait un choc violent sur les alternateurs." },
            { theme: "Protection MALT", type: "Épreuve Écrite", question: "Lors de la dépose d'une Mise à la Terre (MALT/CC), dans quel ordre doit-on procéder ?", options: ["Terre d'abord, puis phases.", "Phases d'abord, puis la terre en tout dernier.", "Tirer le câble.", "Couper à la pince."], correctIndex: 1, justification: "On retire toujours les phases en premier. Si on retirait la terre d'abord, on s'exposerait à une tension induite mortelle." },
            { theme: "Restitution d'ouvrage", type: "Épreuve Écrite", question: "Avis de Fin de Travail signé. Le CC trouve une caisse à outils oubliée sur les barres. Qui est fautif ?", options: ["Le CC.", "L'ouvrier.", "Le Chef de Travaux (CDT).", "Le Dispatching."], correctIndex: 2, justification: "En signant la fin d'AT, le CDT certifie avoir inspecté la zone et retiré tout le matériel et le personnel." }
        ];

        // 2. CONTRÔLE ÉLECTRIQUE (Protections, Automatismes, Moteurs, CCNA/Relais)
        const poolControle = [
            { theme: "Relais Buchholz", type: "Épreuve Écrite", question: "Quel est le rôle principal du relais Buchholz (63) sur un transformateur ?", options: ["Protéger des surcharges électriques externes.", "Détecter les défauts internes via le dégagement de gaz ou l'afflux d'huile.", "Régler la tension.", "Mesurer la puissance active."], correctIndex: 1, justification: "Il détecte la décomposition de l'huile causée par un arc interne ou un point chaud." },
            { theme: "Relais Lockout (86)", type: "Épreuve Écrite", question: "Dans le schéma de protection, quelle est la fonction du relais ANSI 86 ?", options: ["Réenclencheur.", "Bloquer la fermeture du disjoncteur jusqu'à son réarmement manuel après un défaut majeur.", "Régulateur de tension.", "Relais de communication."], correctIndex: 1, justification: "Le Lockout empêche la remise sous tension accidentelle d'un transformateur en défaut." },
            { theme: "Inrush Current", type: "Épreuve Écrite", question: "Qu'est-ce qui provoque souvent le déclenchement intempestif du relais différentiel (87T) lors de la mise sous tension d'un transfo ?", options: ["Le courant d'enclenchement magnétisant (Inrush) asymétrique.", "Le régleur en charge.", "La surtension de foudre.", "Un court-circuit externe."], correctIndex: 0, justification: "Le courant Inrush n'apparaît qu'au primaire, le relais 87T le voit donc comme un faux défaut interne. Il est bloqué par l'harmonique 2." },
            { theme: "Automatisme (ELCB/RCD)", type: "Épreuve Écrite", question: "Quel est le but d'un disjoncteur différentiel résiduel (ELCB / RCD 30mA) dans un coffret BT ?", options: ["Protéger contre les surcharges.", "Protéger l'humain contre l'électrocution due aux courants de fuite à la terre.", "Inverser les phases.", "Protéger le moteur."], correctIndex: 1, justification: "Il mesure la différence entre la Phase et le Neutre. Si > 30mA (danger mortel), il coupe le circuit." },
            { theme: "Protection Distance (21)", type: "Épreuve Écrite", question: "En protection de distance de ligne, qu'est-ce que le phénomène de 'Over-reach' (Dépassement de zone) ?", options: ["Refus de déclencher sur défaut.", "Déclenchement à tort pour un défaut situé hors de sa zone (ex: ligne adjacente) suite à une erreur de mesure d'impédance.", "Augmentation de la tension de ligne.", "Perte du signal CPL."], correctIndex: 1, justification: "Cela brise la sélectivité du réseau en déclenchant des lignes saines." },
            { theme: "Défaillance Disjoncteur (50BF)", type: "Simulation", question: "Quel est le rôle de la protection 'Breaker Failure' (50BF) ?", options: ["Refermer la ligne.", "Mesurer l'usure mécanique.", "Si un disjoncteur refuse de s'ouvrir sur défaut, elle déclenche tous les disjoncteurs du jeu de barres pour isoler le nœud.", "Détecter le SF6."], correctIndex: 2, justification: "C'est la protection de secours ultime du poste (Local Backup)." },
            { theme: "Protection Directionnelle (67)", type: "Épreuve Écrite", question: "Pourquoi utilise-t-on une protection de surintensité directionnelle (ANSI 67) ?", options: ["Pour mesurer l'énergie.", "Pour déclencher uniquement si le courant de défaut circule vers la zone protégée, assurant la sélectivité dans un réseau bouclé.", "Pour réduire le coût.", "Pour inverser les moteurs."], correctIndex: 1, justification: "Le relais 67 compare l'angle entre U et I pour déterminer le sens du défaut." },
            { theme: "Moteurs Asynchrones", type: "Épreuve Écrite", question: "Dans un moteur triphasé à cage d'écureuil tournant à vide, que se passe-t-il électriquement ?", options: ["Le courant est nul.", "Il tire un fort courant réactif (jusqu'à 40% de In) pour sa magnétisation, d'où un facteur de puissance (Cos Phi) très faible.", "Le moteur tourne à l'envers.", "Le rotor chauffe énormément."], correctIndex: 1, justification: "Le courant de magnétisation fait chuter le Cos Phi proche de 0.2 à vide." },
            { theme: "Relais Statiques (SSR)", type: "Épreuve Écrite", question: "Quel est l'avantage d'un Solid State Relay (SSR) en automatisation par rapport à un contacteur classique ?", options: ["Il est bruyant.", "Il n'a aucune pièce mécanique mobile, offrant une durée de vie quasi infinie et une commutation ultra-rapide sans étincelle.", "Il n'a pas besoin de refroidissement.", "Il produit des arcs."], correctIndex: 1, justification: "Utilisant des Thyristors ou Triacs, il ne s'use pas mécaniquement." },
            { theme: "Compensation (Facteur Puissance)", type: "Épreuve Écrite", question: "Comment compense-t-on un mauvais facteur de puissance dans un réseau industriel ?", options: ["Avec des résistances en série.", "En connectant des condensateurs EN PARALLÈLE avec la charge pour fournir l'énergie réactive localement.", "En augmentant la fréquence.", "Avec de plus gros câbles."], correctIndex: 1, justification: "Les condensateurs produisent des kVAR, évitant de les soutirer du réseau THT." },
            { theme: "Discordance de Pôles (52D)", type: "Simulation", question: "Un pôle fermé, deux ouverts sur un disjoncteur HT. Risque et action ?", options: ["Rien, la tension s'équilibre.", "Le relais 52D détecte l'asymétrie et force l'ouverture tripolaire pour éviter les courants homopolaires destructeurs pour les machines tournantes.", "Le disjoncteur explose.", "Le SCADA plante."], correctIndex: 1, justification: "Une discordance prolongée chauffe les rotors des générateurs du réseau." },
            { theme: "Contrôle (Timers)", type: "Épreuve Écrite", question: "En logique de relais, comment fonctionne un temporisateur 'On-Delay' ?", options: ["Il ferme immédiatement et ouvre plus tard.", "Ses contacts changent d'état seulement APRÈS l'écoulement d'un délai programmé suite à sa mise sous tension.", "Il compte les impulsions.", "Il ignore le temps."], correctIndex: 1, justification: "Utilisé pour décaler les démarrages ou coordonner des protections." },
            { theme: "Synchronisme (25)", type: "Épreuve Écrite", question: "Le relais de synchronisme (25) contrôle trois paramètres avant de fermer un disjoncteur de ligne :", options: ["Pression, température et SF6.", "La différence de Tension (ΔU), de Fréquence (Δf) et l'Angle de phase (Δθ) entre les deux côtés.", "La puissance active.", "La résistance de contact."], correctIndex: 1, justification: "Le couplage de deux réseaux asynchrones provoquerait un choc destructeur." },
            { theme: "Puissance Inverse (32)", type: "Simulation", question: "Sur un alternateur, que protège le relais ANSI 32 (Reverse Power) ?", options: ["Contre les surtensions.", "Il empêche l'alternateur de se comporter comme un moteur électrique géant (pompant le réseau) s'il perd sa turbine d'entraînement.", "Il accélère la turbine.", "Il augmente l'excitation."], correctIndex: 1, justification: "La marche en moteur endommagerait la turbine (ex: pales de turbine à vapeur)." },
            { theme: "Logique Câblée (Arrêt d'Urgence)", type: "Épreuve Écrite", question: "Pourquoi utilise-t-on TOUJOURS un contact Normalement Fermé (NC/NF) pour un bouton d'Arrêt d'Urgence ?", options: ["Le NF est moins cher.", "Pour la 'Sécurité Positive' : si le fil de commande se coupe accidentellement, le système s'arrêtera de lui-même.", "Pour économiser du courant.", "Pour la couleur rouge."], correctIndex: 1, justification: "Principe du Fail-Safe. Un fil coupé sur un contact NO rendrait l'arrêt inopérant." }
        ];

        // 3. MAINTENANCE POSTE (Huile, Terre, Batteries, GIS)
        const poolMaintenance = [
            { theme: "Rigidité Diélectrique (Huile)", type: "Simulation", question: "Quelle est la distance standard entre les électrodes lors du test de claquage de l'huile (IEC 156) ?", options: ["10 mm.", "2.5 mm.", "5 cm.", "1 mm."], correctIndex: 1, justification: "La norme IEC spécifie un écartement de 2.5 mm avec des électrodes sphériques pour garantir la reproductibilité du test (> 50kV)." },
            { theme: "Analyse DGA (C2H2)", type: "Épreuve Écrite", question: "La présence d'Acétylène (C2H2) lors de l'analyse des gaz dissous indique :", options: ["Une chauffe normale du papier.", "Des décharges partielles mineures.", "L'existence d'un arc électrique de haute énergie (étincelle/court-circuit) à l'intérieur de la cuve.", "L'oxydation lente de l'huile."], correctIndex: 2, justification: "La formation d'Acétylène nécessite une température extrême (milliers de degrés), signature unique de l'arc électrique." },
            { theme: "Silicagel", type: "Simulation", question: "Les granulés de Silicagel du reniflard sont devenus roses (ou transparents/blancs). Que faire ?", options: ["Ajouter de l'eau.", "Ne rien faire, c'est l'été.", "Programmer leur remplacement ou régénération car ils sont saturés en humidité.", "Dégazer le Buchholz."], correctIndex: 2, justification: "Le silicagel sec est bleu ou orange. Saturé, il ne protège plus le papier isolant de l'humidité atmosphérique." },
            { theme: "Résistance de Contact (Micro-ohmmètre)", type: "Simulation", question: "Le test sur les pôles d'un disjoncteur fermé indique 450 µΩ (limite constructeur : 50 µΩ). Quel est le risque ?", options: ["Une fuite de SF6.", "Un échauffement thermique extrême (Point chaud) au passage du courant nominal, risquant l'incendie ou la fusion des contacts.", "La panne du moteur de réarmement.", "Aucun risque."], correctIndex: 1, justification: "Loi de Joule (P = R.I²). Une résistance élevée avec 2000A dissipera une chaleur destructive." },
            { theme: "Tension de Pas (Step Voltage)", type: "Épreuve Écrite", question: "Lors d'un court-circuit à la terre, qu'est-ce que la Tension de Pas ?", options: ["La tension du câble.", "La différence de potentiel dangereuse créée entre les deux pieds d'une personne marchant sur le sol près du défaut.", "La tension nominale du réseau.", "La tension de la batterie."], correctIndex: 1, justification: "Le courant s'écoulant dans la terre crée un gradient de tension de surface mortel." },
            { theme: "Gravier en Poste Extérieur", type: "Simulation", question: "Pourquoi la cour des postes THT est-elle recouverte d'une épaisse couche de gravier ?", options: ["Pour l'esthétique.", "Pour augmenter fortement la résistivité électrique du sol en surface, réduisant ainsi les courants mortels de tension de pas et de contact.", "Pour absorber les fuites d'huile.", "Pour éviter le gel."], correctIndex: 1, justification: "Le gravier sec agit comme une couche isolante vitale pour les opérateurs au sol." },
            { theme: "Batteries VCC", type: "Épreuve Écrite", question: "Pourquoi les systèmes de contrôle-commande sont-ils alimentés par des batteries DC (110V/220V) ?", options: ["Le courant continu coûte moins cher.", "Pour garantir l'alimentation des relais et l'ouverture des disjoncteurs même lors d'un effondrement total du réseau alternatif (Sécurité absolue).", "Pour alimenter les PC portables.", "Pour éviter les harmoniques."], correctIndex: 1, justification: "C'est l'Ultimate Backup. Sans batteries, un poste en black-out ne pourrait ouvrir aucun disjoncteur sur défaut." },
            { theme: "Extinction Incendie Salle Relais", type: "Épreuve Écrite", question: "Quel gaz d'extinction est privilégié dans les salles abritant l'électronique de contrôle (SCADA/Relais) ?", options: ["L'eau pulvérisée.", "Le CO2 ou le FM-200, car ils étouffent le feu sans laisser de résidus destructeurs pour les cartes électroniques.", "La poudre ABC.", "La mousse chimique."], correctIndex: 1, justification: "L'eau ou la poudre détruiraient irrémédiablement les composants électroniques." },
            { theme: "Climatisation (HVAC)", type: "Épreuve Écrite", question: "Pourquoi la redondance de la climatisation est-elle critique dans la salle des relais d'un poste HT ?", options: ["Pour le confort du personnel.", "Pour empêcher la poussière.", "Les relais numériques et calculateurs plantent ou grillent rapidement au-dessus de 40°C, entraînant la perte de contrôle du poste.", "Pour évaporer l'humidité."], correctIndex: 2, justification: "La durée de vie de l'électronique IED chute drastiquement avec la chaleur." },
            { theme: "Test SFRA", type: "Épreuve Écrite", question: "Que permet de détecter l'essai SFRA (Sweep Frequency Response Analysis) sur un transformateur ?", options: ["L'acidité de l'huile (TAN).", "Les déformations mécaniques ou déplacements physiques des bobines et du noyau suite à un court-circuit violent ou un choc de transport.", "Les micro-fuites de SF6.", "La température du cuivre."], correctIndex: 1, justification: "Le SFRA trace l'empreinte RLC du transformateur. Toute déformation physique modifie la fréquence de résonance." },
            { theme: "Maintenance OLTC", type: "Épreuve Écrite", question: "Sur un Changeur de Prises en Charge (OLTC), quel compartiment nécessite le filtrage d'huile le plus fréquent ?", options: ["La cuve principale.", "Le compartiment de l'Interrupteur de Puissance (Diverter Switch) car il coupe le courant sous charge, créant des arcs qui carbonisent l'huile.", "Le radiateur.", "Le sélecteur de prises."], correctIndex: 1, justification: "Les arcs électriques normaux de commutation dégradent très vite l'huile de ce compartiment spécifique." },
            { theme: "Groupes Électrogènes (Wet Stacking)", type: "Simulation", question: "Lors de l'essai mensuel du groupe diesel de secours, pourquoi est-il déconseillé de le faire tourner à vide ?", options: ["Pour économiser du carburant.", "Cela provoque le 'Glaçage des cylindres' (Wet Stacking), l'huile imbrûlée se déposant dans l'échappement par manque de chaleur.", "Cela démagnétise l'alternateur.", "Le démarreur brûle."], correctIndex: 1, justification: "Un moteur diesel a besoin d'être chargé (min 30%) pour atteindre sa température de combustion optimale." },
            { theme: "GIS (SF6)", type: "Épreuve Écrite", question: "Lors de l'ouverture d'un compartiment de Poste Blindé GIS, l'agent doit porter un équipement étanche car :", options: ["Le SF6 pur est hautement toxique.", "L'air corrode l'aluminium.", "Les poudres blanches résiduelles (sous-produits de l'arc SF6) sont extrêmement toxiques et corrosives pour les voies respiratoires.", "Il fait très froid."], correctIndex: 2, justification: "Le SF6 pur est inerte, mais les fluorures métalliques créés par l'arc sont dangereux." },
            { theme: "Décharges Partielles (DP)", type: "Épreuve Écrite", question: "Que sont les Décharges Partielles dans l'isolation d'un équipement HT ?", options: ["Des coups de foudre atténués.", "Des micro-arcs se produisant dans des vides d'air internes à l'isolant, qui rongent lentement le matériau jusqu'au claquage final.", "Des fuites d'huile.", "L'ouverture lente d'un contact."], correctIndex: 1, justification: "Les DP sont le \"cancer\" de l'isolation (câbles, transfos), dégradant l'équipement sur le long terme." },
            { theme: "Résistance d'Enroulement (Transfo)", type: "Simulation", question: "Pourquoi mesure-t-on la résistance ohmique des enroulements (DC Winding) d'un transformateur ?", options: ["Pour calculer les pertes fer.", "Pour vérifier l'intégrité des connexions internes, et détecter un mauvais contact au niveau des prises (Taps) qui générerait un point chaud.", "Pour vérifier l'huile.", "Pour changer l'indice horaire."], correctIndex: 1, justification: "Une légère augmentation de résistance ohmique (milliohms) créera une chaleur énorme à pleine charge." }
        ];

        // 4. MAINTENANCE LIGNE (ML) (Pylônes, Sécurité en hauteur, Câbles)
        const poolMaintenanceLigne = [
            { theme: "Sécurité Téléphone", type: "Simulation", question: "Pourquoi l'utilisation du smartphone est-elle strictement interdite pendant la consignation (VAT, MALT) sur un pylône ?", options: ["Interférence radio avec le SCADA.", "La distraction (SMS, Appel) fait perdre la concentration lors d'étapes vitales, menant directement au non-respect des distances et à l'arc mortel.", "C'est un ordre administratif.", "Pour économiser la batterie."], correctIndex: 1, justification: "En THT, la distraction cognitive de quelques secondes cause les accidents les plus graves." },
            { theme: "Sécurité (Point Mort)", type: "Simulation", question: "Qu'est-ce que l'erreur éliminatoire du 'Point Mort' en ascension de pylône ?", options: ["Faire une pause trop longue.", "Se déconnecter totalement (aucune longe attachée) pendant quelques secondes pour franchir un obstacle, se retrouvant sans protection antichute.", "Lâcher ses outils.", "Ne pas porter de lunettes."], correctIndex: 1, justification: "La règle de l'ancrage 100% continu nécessite l'usage d'une longe double (en Y). Le point mort est mortel." },
            { theme: "Step Bolts (Boulons d'escalade)", type: "Simulation", question: "Peut-on ancrer le mousqueton de sa longe antichute sur les boulons d'escalade (Step bolts) du pylône ?", options: ["Oui, ils sont faits pour ça.", "Non, ils se cisailleraient sous la force dynamique gigantesque d'une chute (12 kN). L'ancrage se fait toujours sur les membrures principales de la structure.", "Oui, s'ils sont neufs.", "C'est au choix du lignard."], correctIndex: 1, justification: "Les step bolts ne supportent que le poids statique (les pieds)." },
            { theme: "Lavage Isolateurs (Sous Tension)", type: "Simulation", question: "Dans quel sens doit-on impérativement arroser les isolateurs lors d'un lavage sous tension ?", options: ["Par le milieu.", "Du sommet (terre) vers le bas.", "Obligatoirement par le BAS (côté conducteur sous tension) en remontant progressivement vers la terre.", "Peu importe."], correctIndex: 2, justification: "Si on lave par le haut, l'eau sale ruisselle sur les jupes inférieures, créant un flashover (court-circuit) immédiat." },
            { theme: "Qualité d'Eau (Lavage)", type: "Épreuve Écrite", question: "Quel paramètre de l'eau est vital pour autoriser le lavage sous tension ?", options: ["Son goût.", "Son pH.", "Sa conductivité électrique, qui doit être d'une pureté extrême (eau déminéralisée, ex: < 50 µS/cm).", "Sa densité."], correctIndex: 2, justification: "Utiliser de l'eau du réseau (conductrice) guiderait l'arc électrique HT jusqu'au camion du lignard." },
            { theme: "Effet Couronne", type: "Épreuve Écrite", question: "Qu'est-ce que l'Effet Couronne (Corona Effect) visible sur les lignes THT ?", options: ["Le reflet du soleil sur le câble.", "L'ionisation (claquage) de l'air entourant le conducteur due au champ électrique très intense (crépitement, ozone, lueur bleutée).", "Un dépôt de givre.", "Un défaut d'ancrage."], correctIndex: 1, justification: "Il cause des pertes de puissance active et des interférences radio." },
            { theme: "Faisceaux de Câbles (Bundle)", type: "Épreuve Écrite", question: "Pourquoi regrouper 2, 3 ou 4 câbles par phase en 400kV au lieu d'un seul gros câble ?", options: ["Pour résister aux tempêtes.", "Pour augmenter le diamètre virtuel de la phase, ce qui réduit considérablement le gradient de champ électrique en surface et limite l'effet Couronne.", "Pour faire fuir les oiseaux.", "Pour baisser la résistance mécanique."], correctIndex: 1, justification: "Adoucit le champ de surface, rendant la ligne plus efficace et silencieuse." },
            { theme: "Flèche (Sag) et Température", type: "Épreuve Écrite", question: "Que subit physiquement le conducteur en plein été sous un fort transit de courant ?", options: ["Il rétrécit.", "Il gèle.", "Il subit une dilatation thermique, sa longueur augmente, ce qui FAIT AUGMENTER la flèche (Sag) et diminue dangereusement la garde au sol.", "Sa tension mécanique s'accroît."], correctIndex: 2, justification: "La dilatation excessive cause des blackout par amorçage sur la végétation en contrebas." },
            { theme: "Effet Ferranti", type: "Simulation", question: "Lors de la mise sous tension d'une ligne longue 400kV à VIDE (sans charge), l'Effet Ferranti se manifeste par :", options: ["Une chute de tension massive.", "La tension à l'arrivée (récepteur) devient SUPÉRIEURE à la tension de départ (source).", "La ligne tremble.", "Coupure de phase."], correctIndex: 1, justification: "L'effet capacitif de la ligne à vide élève la tension, nécessitant des bobines de réactance (Shunt Reactors) pour compenser." },
            { theme: "Parafoudres Polymères", type: "Épreuve Écrite", question: "Quel est l'avantage principal du parafoudre ZnO à enveloppe silicone/polymère par rapport à la porcelaine ?", options: ["Il est beaucoup plus lourd.", "Il est hydrophobe (repousse l'eau et la pollution) et n'éclate pas en morceaux tranchants mortels en cas d'explosion interne.", "Il est moins cher.", "Il est inflammable."], correctIndex: 1, justification: "Le silicone maintient l'isolation même sous forte pollution marine ou désertique." },
            { theme: "Amortisseurs (Stockbridge)", type: "Épreuve Écrite", question: "Quel est le rôle des amortisseurs en forme d'haltères fixés sur les câbles près des pylônes ?", options: ["Faire un contrepoids pour la flèche.", "Dissiper l'énergie des vibrations éoliennes (vent léger) pour empêcher la rupture par fatigue des brins d'aluminium du câble au point d'ancrage.", "Attirer la foudre.", "Améliorer le passage du courant."], correctIndex: 1, justification: "Ils protègent le câble des vibrations de haute fréquence (Tourbillons de Karman)." },
            { theme: "Pylônes 400kV (Extensions)", type: "Simulation", question: "Si le sol est en pente, comment ajuste-t-on la base du pylône 400kV ?", options: ["On coule plus de ciment.", "On utilise des haubans.", "On installe des extensions de pieds (Leg extensions) de différentes longueurs (ex: +1.5m, +3m).", "On tord l'acier."], correctIndex: 2, justification: "Cela permet de garder le corps du pylône parfaitement vertical sans travaux de terrassement massifs." },
            { theme: "Pylône d'Arrêt (Tension Tower)", type: "Épreuve Écrite", question: "Quelle est la principale différence de contrainte entre un pylône de Suspension et un pylône d'Arrêt (Angle) ?", options: ["Le pylône d'arrêt est en bois.", "Le pylône d'Arrêt résiste à la forte tension mécanique longitudinale (traction) des câbles, nécessitant des fondations massives contre l'arrachement (Uplift).", "Il n'y a aucune différence.", "Le pylône d'arrêt n'a pas de terre."], correctIndex: 1, justification: "Les pylônes d'arrêt 'tirent' le câble, alors que ceux de suspension ne font que supporter le poids vertical." },
            { theme: "Isolateurs (Corona Ring)", type: "Épreuve Écrite", question: "À quoi servent les anneaux métalliques (Corona rings) aux extrémités des chaînes d'isolateurs THT ?", options: ["À accrocher les poulies.", "À répartir uniformément le gradient de tension électrique sur les premières jupes, protégeant l'isolateur de l'étincelage.", "À faire du poids.", "À repousser la pluie."], correctIndex: 1, justification: "Adoucit le champ électrique énorme au niveau de la fixation du câble THT." },
            { theme: "Harnais de Sécurité", type: "Simulation", question: "Quel est le risque si les sangles de cuisses du harnais antichute sont trop lâches ?", options: ["Le lignard aura froid.", "Le pantalon se déchire.", "En cas de chute, les sangles remontent violemment dans l'aine, causant des traumatismes artériels graves et accélérant le syndrome du harnais.", "Le mousqueton se bloque."], correctIndex: 2, justification: "Un harnais doit être ajusté près du corps pour répartir la force de choc sur le squelette solide." }
        ];

        // 5. CE ESSAIS / ANALYSES (Commissioning, Injection, Câbles, TDR)
        const poolEssaisAnalyses = [
            { theme: "Polarité TC", type: "Simulation", question: "Test Flick (Pile 9V) sur un TC. Si la polarité (P1-P2/S1-S2) est correcte, que fait le galvanomètre à la fermeture ?", options: ["L'aiguille ne bouge pas.", "Elle dévie brusquement dans le sens positif (droite) puis revient à zéro.", "Elle dévie en négatif (gauche).", "Elle oscille continuellement."], correctIndex: 1, justification: "L'induction (Loi de Lenz) crée un pulse positif si le câblage respecte les bornes homologues." },
            { theme: "Danger TC Ouvert", type: "Simulation", question: "Le circuit secondaire d'un TC en service est accidentellement laissé OUVERT. Conséquence ?", options: ["Le relais déclenche le poste.", "Le noyau magnétique sature instantanément, induisant des pics de tension de plusieurs kV aux bornes ouvertes, détruisant l'isolant et menaçant l'opérateur de mort.", "Le courant réseau s'effondre.", "L'huile du TC gèle."], correctIndex: 1, justification: "Sans courant secondaire pour démagnétiser le noyau, la tension induite (e = N.dΦ/dt) explose." },
            { theme: "Danger TT Court-Circuité", type: "Simulation", question: "Que se passe-t-il si un technicien crée un court-circuit franc aux bornes secondaires d'un Transformateur de Tension (TT) sous tension ?", options: ["Rien, le TT encaisse.", "Un courant énorme va y circuler, brûlant le bobinage et pouvant faire exploser le TT si les fusibles (MCB) ne fondent pas.", "La tension primaire augmente.", "Le relais de distance plante."], correctIndex: 1, justification: "Le TT est une source de tension. Un court-circuit secondaire équivaut à un I=U/Z massif." },
            { theme: "Injection Primaire", type: "Épreuve Écrite", question: "Quel est l'objectif ultime de l'essai d'injection primaire lors du Commissioning d'un poste ?", options: ["C'est plus rapide que la secondaire.", "Tester l'IHM du relais.", "Valider l'intégrité de TOUTE la chaîne (Rapport physique du TC, filerie, polarité réelle, et déclenchement effectif du disjoncteur HT).", "Tester la température."], correctIndex: 2, justification: "C'est l'essai global 'End-to-End' qui garantit qu'il n'y a aucune erreur de câblage sur le terrain." },
            { theme: "Test Câbles (VLF vs DC)", type: "Épreuve Écrite", question: "Pourquoi les normes exigent-elles de tester les câbles XLPE synthétiques en VLF (0.1 Hz) et non en Hipot DC ?", options: ["Le VLF est plus rapide.", "Le test DC piège des charges d'espace dans le plastique XLPE, provoquant son claquage irréversible à la remise sous tension AC (phénomène de Water treeing).", "Le VLF a plus de tension.", "Le DC est illégal en Algérie."], correctIndex: 1, justification: "L'application de DC sur du polymère détériore la durée de vie du câble sain." },
            { theme: "Localisation (TDR / Échomètre)", type: "Épreuve Écrite", question: "Rôle de l'échomètre (TDR) en recherche de défauts de câbles ?", options: ["Brûler l'isolant du câble.", "Envoyer une impulsion basse tension pour mesurer le temps de retour de l'écho, permettant de calculer la DISTANCE du défaut (Pré-localisation).", "Écouter l'arc sous terre.", "Mesurer l'humidité."], correctIndex: 1, justification: "Le TDR analyse la réflexion de l'onde pour donner une distance en mètres (ex: Défaut à 450m)." },
            { theme: "Localisation (Thumper)", type: "Simulation", question: "À quoi sert le Générateur d'ondes de choc (Thumper / Éclateur) couplé à un géophone ?", options: ["Nettoyer le câble.", "Localiser le défaut avec précision (Pinpointing) en créant un arc bruyant sous terre, écouté en surface par l'opérateur.", "Mesurer la terre du poste.", "Refroidir l'isolant fondu."], correctIndex: 1, justification: "Permet de marquer le sol exactement au-dessus du défaut avant de creuser." },
            { theme: "Charge TC (Burden Test)", type: "Épreuve Écrite", question: "Lors du 'Burden Test', si la charge réelle de la filerie+relais dépasse la valeur en VA plaquée sur le TC :", options: ["Le TC deviendra plus précis.", "Le TC saturera prématurément lors d'un court-circuit, empêchant la protection de voir la vraie valeur du courant de défaut.", "La tension du poste chutera.", "Aucun impact."], correctIndex: 1, justification: "Le TC n'aura pas la puissance magnétique nécessaire pour pousser le courant dans une impédance trop forte." },
            { theme: "Mesure de Terre (3 Piquets)", type: "Épreuve Écrite", question: "Lors de la méthode 'Fall of Potential', où doit-on planter le piquet de courant (C2) par rapport au maillage du poste ?", options: ["À 2 mètres du grillage.", "Dans le bâtiment de commande.", "Le plus loin possible (ex: >100m) pour que les zones d'influence de la grille du poste et du piquet C2 ne se chevauchent pas.", "Sur le transformateur."], correctIndex: 2, justification: "Une distance insuffisante fausse la courbe qui ne présentera aucun palier de vraie résistance." },
            { theme: "Test DRM Disjoncteur", type: "Épreuve Écrite", question: "Que permet de visualiser la mesure de Résistance Dynamique (DRM) sur un disjoncteur SF6 ?", options: ["La résistance statique à l'arrêt.", "La résistance EN COURS de mouvement (ouverture), permettant de diagnostiquer l'usure cachée de la pointe d'arc en tungstène (Arcing Contact).", "La résistance de la bobine.", "La pression du gaz."], correctIndex: 1, justification: "Diagnostic vital pour évaluer l'usure interne des contacts sans avoir à récupérer le gaz SF6." },
            { theme: "Test GOOSE (IEC 61850)", type: "Simulation", question: "Comment tester un interverrouillage GOOSE entre deux baies numériques ?", options: ["Avec un multimètre sur les câbles.", "Avec une pince ampèremétrique.", "À l'aide d'un analyseur de réseau (ex: Wireshark/IEDScout) branché sur le switch Ethernet pour lire le changement d'état de la variable booléenne.", "En augmentant la tension HT."], correctIndex: 2, justification: "L'information transite sous forme de trames logicielles sur le réseau local (LAN)." },
            { theme: "Phasage (Concordance)", type: "Simulation", question: "Avant la première mise en parallèle d'un transfo neuf avec le réseau, le test le plus critique est :", options: ["Le test de bruit.", "Le test de concordance de phases (Phasing), prouvant que la Phase A du transfo correspond exactement à la Phase A du réseau.", "L'analyse DGA de l'huile.", "Le test du relais Buchholz."], correctIndex: 1, justification: "Si les phases sont inversées, la fermeture du disjoncteur causera une explosion cataclysmique (Court-circuit franc)." },
            { theme: "Saturation 87B", type: "Simulation", question: "Dans le test de stabilité d'une protection différentielle de barre (87B), on injecte un courant traversant (Through-fault). Pourquoi ?", options: ["Pour chauffer la barre.", "Pour s'assurer que si un TC sature sur un défaut EXTERNE, le relais lit bien Zéro (Idiff) et ne purge pas tout le poste à tort.", "Pour tester l'affichage IHM.", "Pour vérifier le SF6."], correctIndex: 1, justification: "Un défaut externe crée un fort courant. La saturation d'un TC crée une erreur lue comme un défaut interne. Le relais doit être stabilisé." },
            { theme: "Synchronisme (25)", type: "Épreuve Écrite", question: "Pendant le test du relais de synchronisme (ANSI 25), quels Deltas (Δ) fait-on varier pour trouver les seuils de blocage ?", options: ["La pression, le volume, la température.", "Le Delta-Voltage (ΔV), Delta-Fréquence (Δf) et Delta-Angle (Δθ) entre la ligne et la barre.", "Les harmoniques 3, 5, 7.", "Les courants I1, I2, I0."], correctIndex: 1, justification: "Le relais bloque la fermeture si l'un de ces trois écarts entre les deux réseaux est trop grand." },
            { theme: "Megger & PI", type: "Épreuve Écrite", question: "Lors d'un test Megger (5000V DC) sur un transfo, le calcul du PI (Index de Polarisation) donne 1.05. Conclusion ?", options: ["L'isolant est parfait.", "L'isolant (papier/huile) est fortement humide ou pollué. Ne pas mettre sous tension.", "Le testeur n'a plus de batterie.", "C'est normal en hiver."], correctIndex: 1, justification: "Un PI sain (bonne absorption diélectrique) est > 1.5. Un PI proche de 1 indique un courant de fuite fort et continu (Humidité/Danger)." }
        ];

        // 6. TÉLÉCOM & TÉLÉCONDUITE (Bilingue + SCADA, OPGW, CCNA, Réseaux)
        const poolTelecom = [
            { 
                theme: "Réseaux / الشبكات (CCNA)", 
                type: "Épreuve Écrite", 
                question: "Quelle est la principale différence entre un Switch (commutateur) et un Hub (concentrateur) ?<br><br><span class='text-sonelgaz-orange font-arabic text-lg'>ما هو الفرق الرئيسي بين المحول (Switch) والموزع (Hub)؟</span>", 
                options: [
                    "Le Hub filtre les paquets par adresse MAC, le Switch non. / الموزع يفلتر الحزم عبر عنوان MAC، المحول لا.", 
                    "Le Switch envoie les données uniquement au port de destination (via table MAC), évitant les collisions, alors que le Hub diffuse à tous les ports. / المحول يرسل البيانات فقط إلى منفذ الوجهة (عبر جدول MAC) لتجنب التصادم، بينما يوزع الـ Hub للجميع.", 
                    "Le Switch ne fonctionne qu'en Wi-Fi. / المحول يعمل فقط عبر الواي فاي.", 
                    "Le Hub est plus rapide. / الموزع أسرع."
                ], 
                correctIndex: 1, 
                justification: "Le Switch opère au niveau 2 (Liaison de données) et réduit les domaines de collision. / يعمل المحول في الطبقة الثانية ويقلل من نطاقات التصادم.",
                image: "[Image de : Un schéma illustrant la diffusion globale d'un Hub vs la transmission ciblée d'un Switch via Table MAC]"
            },
            { 
                theme: "Téléconduite / التحكم الإشرافي (SCADA)", 
                type: "Épreuve Écrite", 
                question: "Dans une architecture SCADA, quel est le rôle du RTU (Remote Terminal Unit) ?<br><br><span class='text-sonelgaz-orange font-arabic text-lg'>في معمارية سكادا، ما هو دور الوحدة الطرفية عن بعد (RTU)؟</span>", 
                options: [
                    "Produire de l'énergie réactive. / توليد الطاقة التفاعلية.", 
                    "Collecter les signaux physiques (capteurs, relais) du poste et les numériser pour les transmettre au centre de contrôle (Dispatching). / جمع البيانات الفيزيائية في المحطة وإرسالها إلى مركز التحكم.", 
                    "Remplacer le disjoncteur HT. / استبدال قاطع الدورة.", 
                    "Chiffrer les données Wi-Fi. / تشفير بيانات الواي فاي."
                ], 
                correctIndex: 1, 
                justification: "Le RTU est l'interface vitale entre l'équipement physique de la sous-station et le réseau de télécommunication. / الـ RTU هو الواجهة الحيوية بين المعدات الفيزيائية وشبكة الاتصالات.",
                image: "[Image de : Schéma montrant des relais connectés à un RTU, lui-même relié à un centre SCADA]"
            },
            { 
                theme: "Télécommunication (CPL / PLC)", 
                type: "Épreuve Écrite", 
                question: "À quoi sert un 'Bouchon de Ligne' (Line Trap / Wave Trap) suspendu aux portiques THT ?<br><br><span class='text-sonelgaz-orange font-arabic text-lg'>ما هي فائدة 'مانع الذبذبات' (Line Trap) المثبت على هياكل الضغط العالي؟</span>", 
                options: [
                    "Filtrer les impuretés de l'huile. / تصفية شوائب الزيت.", 
                    "Empêcher le courant 50 Hz de passer. / منع مرور تيار 50 هرتز.", 
                    "Bloquer les signaux de télécommunication haute fréquence (CPL) pour qu'ils ne se perdent pas dans le poste, tout en laissant passer la puissance (50 Hz). / حجب إشارات الاتصالات عالية التردد (CPL) لكي لا تضيع في المحطة، مع السماح بمرور الطاقة.", 
                    "Attirer la foudre. / جذب الصواعق."
                ], 
                correctIndex: 2, 
                justification: "Le Bouchon de ligne agit comme une haute impédance pour les hautes fréquences (Data) et une faible impédance pour la puissance. / يعمل كممانعة عالية للبيانات وممانعة منخفضة للطاقة.",
                image: "[Image de : Photo d'un Bouchon de Ligne (cylindre) avec son schéma équivalent RLC]"
            },
            { 
                theme: "Fibre Optique / الألياف البصرية (OPGW)", 
                type: "Simulation", 
                question: "Sur une ligne aérienne HT, quel est le double rôle du câble OPGW (Optical Ground Wire) situé au sommet ?<br><br><span class='text-sonelgaz-orange font-arabic text-lg'>على خط النقل الهوائي، ما هو الدور المزدوج لكابل OPGW؟</span>", 
                options: [
                    "Transporter les phases A et B. / نقل الأطوار A و B.", 
                    "Protéger la ligne contre la foudre (fil de garde) ET transmettre des données à très haut débit (fibres optiques internes). / حماية الخط من الصواعق ونقل البيانات بسرعة عالية.", 
                    "Éviter les vibrations éoliennes. / منع الاهتزازات الهوائية.", 
                    "Mesurer la température. / قياس درجة الحرارة."
                ], 
                correctIndex: 1, 
                justification: "L'OPGW mutualise l'infrastructure : le tube en acier/aluminium protège de la foudre, et le cœur en fibre achemine la téléprotection et le SCADA. / يجمع بين حماية الصواعق ونقل البيانات.",
                image: "[Image de : Coupe transversale d'un câble OPGW montrant les brins d'acier externes et les fibres optiques au centre]"
            },
            { 
                theme: "Protocoles / البروتوكولات (IEC 60870-5)", 
                type: "Épreuve Écrite", 
                question: "Quelle est la principale différence de transport entre l'IEC 60870-5-101 et l'IEC 60870-5-104 ?<br><br><span class='text-sonelgaz-orange font-arabic text-lg'>ما هو الفرق الرئيسي بين بروتوكول 101 و 104 في معيار IEC 60870؟</span>", 
                options: [
                    "Le 101 est pour le gaz, le 104 pour l'électricité. / 101 للغاز و 104 للكهرباء.", 
                    "Le 101 utilise des liaisons séries asynchrones (RS-232/485), tandis que le 104 transporte ces données encapsulées sur des réseaux TCP/IP (Ethernet/LAN/WAN). / 101 يستخدم روابط تسلسلية، بينما 104 ينقل البيانات عبر شبكات TCP/IP.", 
                    "Le 104 est analogique, le 101 est numérique. / 104 تناظري، 101 رقمي.", 
                    "Aucune différence. / لا يوجد فرق."
                ], 
                correctIndex: 1, 
                justification: "L'IEC-104 a révolutionné la téléconduite en permettant d'utiliser l'infrastructure réseau IP standard des entreprises pour le transport SCADA. / بروتوكول 104 استخدم شبكات IP القياسية للتحكم."
            },
            { 
                theme: "Protocoles / البروتوكولات (DNP3)", 
                type: "Épreuve Écrite", 
                question: "Dans le protocole DNP3, à quoi sert le mécanisme 'Report By Exception' (Unsolicited Response) ?<br><br><span class='text-sonelgaz-orange font-arabic text-lg'>في بروتوكول DNP3، ما هي فائدة آلية 'الرد غير المطلوب' (Report By Exception)؟</span>", 
                options: [
                    "Imprimer des rapports PDF. / طباعة تقارير PDF.", 
                    "Le RTU n'attend pas d'être interrogé (Polled) par le SCADA; il envoie spontanément les données uniquement lorsqu'il y a un changement d'état (événement), économisant la bande passante. / الوحدة لا تنتظر طلب المركز، بل ترسل البيانات تلقائياً فقط عند حدوث تغيير، لتوفير عرض النطاق الترددي.", 
                    "Forcer le redémarrage du RTU. / فرض إعادة تشغيل الوحدة.", 
                    "Changer l'adresse IP. / تغيير عنوان IP."
                ], 
                correctIndex: 1, 
                justification: "C'est l'un des grands avantages du DNP3 par rapport au vieux Modbus. / ميزة كبرى مقارنة بـ Modbus القديم."
            },
            { 
                theme: "Réseaux / الشبكات (VLAN)", 
                type: "Simulation", 
                question: "En configuration de Switch (CCNA), pourquoi crée-t-on des VLANs (Virtual LAN) dans une sous-station numérique ?<br><br><span class='text-sonelgaz-orange font-arabic text-lg'>لماذا نقوم بإنشاء شبكات VLAN على محولات المحطة الرقمية؟</span>", 
                options: [
                    "Pour augmenter la consommation d'énergie. / لزيادة استهلاك الطاقة.", 
                    "Pour séparer logiquement les trafics (ex: Ségréguer le trafic SCADA critique de la Vidéo-surveillance) afin d'améliorer la cybersécurité et de réduire les tempêtes de diffusion (Broadcast). / لفصل حركات المرور منطقياً (مثل فصل بيانات سكادا عن كاميرات المراقبة) لتحسين الأمان.", 
                    "Pour changer l'adresse MAC. / لتغيير عنوان MAC.", 
                    "Pour transformer le switch en routeur. / لتحويل المحول إلى موجه."
                ], 
                correctIndex: 1, 
                justification: "Les VLANs assurent que les données vitales (GOOSE/SCADA) ne soient pas ralenties par une caméra IP bavarde. / شبكات VLAN تضمن عدم تأثر البيانات الحيوية بالكاميرات.",
                image: "[Image de : Un Switch divisé en couleurs (VLAN 10 SCADA, VLAN 20 Vidéo)]"
            },
            { 
                theme: "Cybersécurité / الأمن السيبراني", 
                type: "Épreuve Écrite", 
                question: "Quelle est la vulnérabilité majeure des anciens protocoles (Modbus RTU, DNP3 classique) utilisés en milieu industriel ?<br><br><span class='text-sonelgaz-orange font-arabic text-lg'>ما هي الثغرة الأمنية الكبرى في بروتوكولات سكادا القديمة؟</span>", 
                options: [
                    "Ils sont trop lents. / بطيئة جداً.", 
                    "Ils transmettent les données et commandes en texte clair (Clear Text), sans chiffrement ni authentification, rendant le réseau vulnérable à l'interception et l'injection de fausses commandes. / تنقل الأوامر كنص عادي (بدون تشفير)، مما يجعلها عرضة للقرصنة وتزييف الأوامر.", 
                    "Ils utilisent trop de RAM. / تستهلك الكثير من الذاكرة.", 
                    "Ils bloquent les pare-feux. / تعطل جدران الحماية."
                ], 
                correctIndex: 1, 
                justification: "C'est pourquoi la mise en place de VPNs (IPSec) et de Firewalls industriels autour des réseaux OT (Operation Technology) est devenue vitale. / لذلك أصبح استخدام الشبكات الافتراضية الخاصة (VPN) إلزامياً."
            },
            { 
                theme: "Télécom (Multiplexage SDH)", 
                type: "Épreuve Écrite", 
                question: "Dans les réseaux de transport optique inter-postes (SDH/PDH), que signifie le 'Multiplexage' ?<br><br><span class='text-sonelgaz-orange font-arabic text-lg'>في شبكات النقل البصري، ماذا يعني تعدد الإرسال (Multiplexing)؟</span>", 
                options: [
                    "Multiplier la tension HT. / مضاعفة الجهد.", 
                    "Combiner plusieurs signaux lents (voix, SCADA, téléprotection) dans une seule trame à haut débit (STM-1/STM-4) sur une même fibre optique pour optimiser le média. / دمج عدة إشارات بيانات في وسط فيزيائي واحد لتحسين السعة.", 
                    "Couper la fibre en deux. / قطع الألياف إلى نصفين.", 
                    "Supprimer le chiffrement. / إزالة التشفير."
                ], 
                correctIndex: 1, 
                justification: "Le multiplexeur (MUX) rassemble les différents services de la sous-station pour les envoyer sur le backbone national. / جهاز الـ Mux يجمع الخدمات لإرسالها عبر الشبكة الوطنية."
            },
            { 
                theme: "Fiabilité / الموثوقية (Redondance)", 
                type: "Simulation", 
                question: "Que signifie une architecture 'Hot-Standby' pour des serveurs SCADA ou des Routeurs ?<br><br><span class='text-sonelgaz-orange font-arabic text-lg'>ماذا تعني معمارية 'Hot-Standby' لخوادم سكادا؟</span>", 
                options: [
                    "Les deux serveurs sont éteints pour refroidir. / الخادمان مغلقان للتبريد.", 
                    "Le serveur principal (Master) gère le trafic, tandis que le secondaire (Standby) est allumé, synchronisé, et prend automatiquement le relais (Failover) en quelques millisecondes si le principal tombe en panne. / الخادم الرئيسي نشط، والاحتياطي يعمل ويزامن البيانات ليتولى المهمة تلقائياً في حال الفشل.", 
                    "Partage de charge 50/50. / يتقاسمان الحمل 50/50.", 
                    "Connexion Bluetooth. / اتصال بلوتوث."
                ], 
                correctIndex: 1, 
                justification: "Cette redondance (ex: HSRP/VRRP en Cisco) garantit que le Dispatching ne devienne jamais 'Aveugle' (Blind) suite à une simple panne matérielle. / يضمن هذا النظام عدم فقدان مركز التحكم للرؤية أبداً."
            },
            {
                theme: "Matériel (UPS)", 
                type: "Épreuve Écrite", 
                question: "Pourquoi les équipements Télécom et SCADA d'un poste HT doivent-ils être alimentés par un UPS (Uninterruptible Power Supply) avec batteries 48V ou 110V DC ?<br><br><span class='text-sonelgaz-orange font-arabic text-lg'>لماذا يجب تغذية معدات الاتصالات وسكادا بنظام UPS (طاقة غير منقطعة)؟</span>", 
                options: [
                    "Pour améliorer la vitesse d'Internet. / لتحسين سرعة الإنترنت.", 
                    "Pour garantir la transmission des données et alarmes vers le Dispatching même en cas de Black-out (perte totale du réseau AC local). / لضمان نقل البيانات والإنذارات إلى مركز التحكم حتى في حالة الانقطاع التام للكهرباء.", 
                    "Pour protéger contre les virus. / للحماية من الفيروسات.", 
                    "Pour refroidir l'équipement. / لتبريد المعدات."
                ], 
                correctIndex: 1, 
                justification: "Sans UPS et batteries, le Dispatching perdrait la supervision (télémétrie) de la sous-station au moment le plus critique (Défaut réseau). / بدون البطاريات، سيفقد المركز السيطرة في أهم اللحظات."
            }
        ];

        /* ================= GESTION DE L'ÉTAT ET LOGIQUE ================= */
        let appState = {
            mode: 'declaratif', id: "", nom: "", prenom: "", matricule: "", societe: "", poste: "", service: "", district: "",
            currentQuestion: 0, answers: [], score: 0, testQuestions: [], timeRemaining: 3600, timerInterval: null,
            webcamActive: false, mediaStream: null, audioContext: null, analyser: null
        };

        window.allCandidatesResults = JSON.parse(localStorage.getItem('sonelgaz_results')) || [];
        const appContainer = document.getElementById('app-container');

        function saveToLocalStorage() { localStorage.setItem('sonelgaz_results', JSON.stringify(window.allCandidatesResults)); }
        
        function shuffleArray(array) {
            let currentIndex = array.length, randomIndex;
            while (currentIndex !== 0) {
                randomIndex = Math.floor(Math.random() * currentIndex); currentIndex--;
                [array[currentIndex], array[randomIndex]] = [array[randomIndex], array[currentIndex]];
            }
            return array;
        }

        /* --- FENÊTRES MODALES (Remplacement de Alert/Confirm) --- */
        function showCustomAlert(title, message, type = "info") {
            const modal = document.getElementById('custom-modal');
            const icon = document.getElementById('modal-icon');
            document.getElementById('modal-title').innerText = title;
            document.getElementById('modal-message').innerHTML = message;
            
            icon.className = "w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4 text-2xl ";
            if (type === "error") icon.className += "bg-red-100 text-red-600 fas fa-times-circle";
            else icon.className += "bg-blue-100 text-sonelgaz-blue fas fa-info-circle";

            document.getElementById('modal-buttons').innerHTML = `<button onclick="document.getElementById('custom-modal').classList.add('hidden')" class="bg-slate-800 hover:bg-slate-900 text-white font-bold py-2.5 px-6 rounded-xl transition">OK, j'ai compris</button>`;
            modal.classList.remove('hidden');
        }

        function showCustomConfirm(title, message, onConfirm, confirmText = "Confirmer", cancelText = "Annuler") {
            const modal = document.getElementById('custom-modal');
            document.getElementById('modal-title').innerText = title;
            document.getElementById('modal-message').innerHTML = message;
            document.getElementById('modal-icon').className = "w-16 h-16 bg-orange-100 text-sonelgaz-orange rounded-full flex items-center justify-center mx-auto mb-4 text-2xl fas fa-exclamation-triangle";
            
            document.getElementById('modal-buttons').innerHTML = `
                <button id="btn-cancel" class="w-1/2 bg-slate-100 hover:bg-slate-200 text-slate-700 font-bold py-3 rounded-xl transition">${cancelText}</button>
                <button id="btn-confirm" class="w-1/2 bg-red-600 hover:bg-red-700 text-white font-bold py-3 rounded-xl shadow-md transition">${confirmText}</button>
            `;
            
            document.getElementById('btn-cancel').onclick = () => modal.classList.add('hidden');
            document.getElementById('btn-confirm').onclick = () => { modal.classList.add('hidden'); onConfirm(); };
            modal.classList.remove('hidden');
        }

        /* --- INTERFACE D'ACCUEIL --- */
        window.renderIntro = function() {
            clearInterval(appState.timerInterval);
            document.getElementById('global-timer').classList.add('hidden');
            stopWebcam();
            
            const randomId = "CAND-" + Math.floor(10000 + Math.random() * 90000);
            let distOptions = '<option value="">-- Choisir un district --</option>';
            districts.forEach(d => { distOptions += `<option value="${d}">${d}</option>`; });
            let servOptions = '<option value="">-- Choisir une spécialité --</option>';
            services.forEach(s => { servOptions += `<option value="${s}">${s}</option>`; });

            appContainer.innerHTML = `
                <div class="bg-white rounded-2xl shadow-xl w-full max-w-4xl overflow-hidden fade-in border border-slate-200">
                    <div class="bg-slate-800 p-8 text-white text-center relative border-b-4 border-sonelgaz-blue">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-sonelgaz-blue rounded-bl-full opacity-20"></div>
                        <i class="fas fa-file-signature text-5xl mb-4 text-sonelgaz-orange drop-shadow-md"></i>
                        <h2 class="text-3xl font-bold font-arabic mb-1">منصة التقييم المهني</h2>
                        <h3 class="text-xl font-bold tracking-wide">Test d'Habilitation HT/THT</h3>
                        <p class="text-slate-300 mt-2 text-sm"><i class="fas fa-database mr-1"></i> Banques Intégrales : Exploitation, Contrôle, Maintenance, Lignards (ML), Essais, <span class="text-white font-bold">Télécom & SCADA</span></p>
                    </div>

                    <div class="p-6 sm:p-10">
                        <div class="flex border-b border-slate-200 mb-8">
                            <button onclick="window.switchMode('declaratif')" class="w-1/2 py-3 transition-colors ${appState.mode === 'declaratif' ? 'tab-active' : 'tab-inactive'}"><i class="fas fa-user-check mr-2"></i> Mode Officiel</button>
                            <button onclick="window.switchMode('anonyme')" class="w-1/2 py-3 transition-colors ${appState.mode === 'anonyme' ? 'tab-active' : 'tab-inactive'}"><i class="fas fa-user-secret mr-2"></i> Mode Entraînement</button>
                        </div>

                        <div id="form-declaratif" class="${appState.mode === 'declaratif' ? 'block' : 'hidden'} space-y-4 fade-in">
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 bg-slate-50 p-6 rounded-xl border border-slate-100">
                                <div><label class="block text-xs font-bold text-slate-500 uppercase mb-1">Nom / اللقب</label><input type="text" id="in-nom" class="w-full px-3 py-2 border rounded-lg focus:ring-2 focus:ring-sonelgaz-blue outline-none" placeholder="Nom de famille"></div>
                                <div><label class="block text-xs font-bold text-slate-500 uppercase mb-1">Prénom / الإسم</label><input type="text" id="in-prenom" class="w-full px-3 py-2 border rounded-lg focus:ring-2 focus:ring-sonelgaz-blue outline-none" placeholder="Prénom"></div>
                                <div><label class="block text-xs font-bold text-slate-500 uppercase mb-1">Matricule / الرقم</label><input type="text" id="in-mat" class="w-full px-3 py-2 border rounded-lg focus:ring-2 focus:ring-sonelgaz-blue outline-none" placeholder="Ex: 123456"></div>
                                <div><label class="block text-xs font-bold text-slate-500 uppercase mb-1">Société / الشركة</label><input type="text" id="in-soc" value="STOS - Sonelgaz" class="w-full px-3 py-2 border rounded-lg focus:ring-2 focus:ring-sonelgaz-blue outline-none"></div>
                                <div class="md:col-span-2"><label class="block text-xs font-bold text-slate-500 uppercase mb-1">Poste Occupé / المنصب</label><input type="text" id="in-poste" class="w-full px-3 py-2 border rounded-lg focus:ring-2 focus:ring-sonelgaz-blue outline-none" placeholder="Ex: Ingénieur Télécom / Exploitant"></div>
                                <div><label class="block text-xs font-bold text-slate-500 uppercase mb-1">Spécialité / التخصص (Banque QCM)</label><select id="in-serv" class="w-full px-3 py-2 border rounded-lg bg-white">${servOptions}</select></div>
                                <div><label class="block text-xs font-bold text-slate-500 uppercase mb-1">District / الناحية</label><select id="in-dist" class="w-full px-3 py-2 border rounded-lg bg-white">${distOptions}</select></div>
                            </div>
                        </div>

                        <div id="form-anonyme" class="${appState.mode === 'anonyme' ? 'block' : 'hidden'} space-y-4 fade-in">
                            <div class="bg-orange-50 border-l-4 border-sonelgaz-orange p-4 mb-4 text-sm text-slate-700">Test d'entraînement anonyme. ID: <strong id="in-id" class="font-mono text-lg">${randomId}</strong></div>
                            <div>
                                <label class="block text-xs font-bold text-slate-500 uppercase mb-1">Choisissez la spécialité à réviser</label>
                                <select id="in-serv-anon" class="w-full px-3 py-2 border rounded-lg bg-white focus:ring-2 focus:ring-sonelgaz-blue outline-none">
                                    ${servOptions}
                                </select>
                            </div>
                        </div>

                        <div class="mt-6 border-t border-slate-200 pt-6">
                            <div class="flex flex-col sm:flex-row items-center gap-4 bg-blue-50 p-5 rounded-xl border border-blue-200 mb-6">
                                <div class="flex items-center gap-3">
                                    <input type="checkbox" id="in-webcam" class="w-6 h-6 text-sonelgaz-blue rounded focus:ring-sonelgaz-blue cursor-pointer">
                                </div>
                                <div>
                                    <label for="in-webcam" class="font-bold text-slate-800 cursor-pointer text-sm block">
                                        <i class="fas fa-video text-sonelgaz-blue mr-1"></i> Examen à Chaud (Surveillance Visio/Audio)
                                    </label>
                                    <span class="text-xs text-slate-500">Active la caméra et le micro pour simuler une session d'évaluation en direct avec l'Administrateur STOS.</span>
                                </div>
                            </div>
                        
                            <label class="block text-xs font-bold text-slate-500 uppercase mb-2">Longueur de l'évaluation</label>
                            <select id="in-num-q" class="w-full px-4 py-3 bg-slate-50 border rounded-lg focus:ring-2 focus:ring-sonelgaz-blue font-medium outline-none">
                                <option value="5">Test Rapide (5 Questions aléatoires)</option>
                                <option value="15" selected>Test Standard (15 Questions aléatoires)</option>
                                <option value="all">Test Complet (Toutes les questions disponibles de la section)</option>
                            </select>
                        </div>

                        <button onclick="window.startExam()" class="mt-6 w-full bg-sonelgaz-blue hover:bg-blue-700 text-white font-bold py-4 rounded-xl shadow-lg transition transform hover:-translate-y-1 flex justify-center items-center gap-2">
                            Démarrer le Test (1 Heure) <i class="fas fa-stopwatch"></i>
                        </button>
                    </div>
                </div>
            `;
        }

        window.switchMode = function(mode) { appState.mode = mode; window.renderIntro(); }

        /* --- GESTION DE LA WEBCAM --- */
        async function startWebcam() {
            try {
                const stream = await navigator.mediaDevices.getUserMedia({ video: true, audio: true });
                appState.mediaStream = stream;
                document.getElementById('webcam-video').srcObject = stream;
                document.getElementById('webcam-container').style.display = 'block';
                appState.webcamActive = true;
                
                appState.audioContext = new (window.AudioContext || window.webkitAudioContext)();
                const source = appState.audioContext.createMediaStreamSource(stream);
                appState.analyser = appState.audioContext.createAnalyser();
                appState.analyser.fftSize = 256;
                source.connect(appState.analyser);
                const dataArray = new Uint8Array(appState.analyser.frequencyBinCount);
                const audioBar = document.getElementById('audio-bar');
                
                function drawAudio() {
                    if(!appState.webcamActive) return;
                    requestAnimationFrame(drawAudio);
                    appState.analyser.getByteFrequencyData(dataArray);
                    let sum = 0;
                    for(let i=0; i<dataArray.length; i++) sum += dataArray[i];
                    let average = sum / dataArray.length;
                    audioBar.style.height = Math.min(100, (average / 50) * 100) + '%';
                    if (average > 30) audioBar.style.background = '#f39200'; else audioBar.style.background = '#22c55e';
                }
                drawAudio();

            } catch (err) {
                showCustomAlert("Caméra/Micro inaccessibles", "Impossible d'activer le mode Visio (Refus ou absence de matériel). L'examen va se poursuivre en mode normal sans surveillance.", "error");
                appState.webcamActive = false;
            }
        }

        function stopWebcam() {
            if (appState.mediaStream) { appState.mediaStream.getTracks().forEach(track => track.stop()); appState.mediaStream = null; }
            if (appState.audioContext) { appState.audioContext.close(); appState.audioContext = null; }
            document.getElementById('webcam-container').style.display = 'none';
            appState.webcamActive = false;
        }

        function startTimer() {
            appState.timeRemaining = 3600; // 60 mins
            clearInterval(appState.timerInterval);
            document.getElementById('global-timer').classList.remove('hidden');
            document.getElementById('global-timer').classList.remove('bg-red-700', 'animate-pulse');
            document.getElementById('global-timer').classList.add('bg-red-600');
            updateTimerDisplay();
            appState.timerInterval = setInterval(() => {
                appState.timeRemaining--; updateTimerDisplay();
                if (appState.timeRemaining <= 0) { clearInterval(appState.timerInterval); autoSubmitTest(); }
            }, 1000);
        }

        function updateTimerDisplay() {
            const el = document.getElementById('timer-display');
            if(!el) return;
            const h = Math.floor(appState.timeRemaining / 3600);
            const m = Math.floor((appState.timeRemaining % 3600) / 60);
            const s = appState.timeRemaining % 60;
            el.innerText = `${h.toString().padStart(2,'0')}:${m.toString().padStart(2,'0')}:${s.toString().padStart(2,'0')}`;
            const timerContainer = document.getElementById('global-timer');
            if (appState.timeRemaining < 300) { timerContainer.classList.remove('bg-red-600'); timerContainer.classList.add('bg-red-700', 'animate-pulse'); }
        }

        function autoSubmitTest() {
            while (appState.answers.length < appState.testQuestions.length) { appState.answers.push({ questionIndex: appState.answers.length, selected: -1, isCorrect: false }); }
            window.saveResultAndRender();
        }

        window.startExam = function() {
            if (appState.mode === 'declaratif') {
                const fields = ['nom', 'prenom', 'mat', 'soc', 'poste', 'serv', 'dist'];
                let isValid = true;
                fields.forEach(f => {
                    const val = document.getElementById(`in-${f}`).value.trim();
                    if(!val) isValid = false;
                    appState[f === 'mat' ? 'matricule' : (f==='soc' ? 'societe' : (f==='serv' ? 'service' : (f==='dist' ? 'district' : f)))] = val.toUpperCase();
                });
                if (!isValid) return showCustomAlert("Erreur", "Veuillez remplir tous les champs obligatoires.", "error");
                appState.id = `${appState.matricule}-${Math.floor(100+Math.random()*900)}`;
            } else {
                const serviceVal = document.getElementById('in-serv-anon').value;
                if (!serviceVal) return showCustomAlert("Erreur", "Veuillez choisir une spécialité.", "error");
                appState.id = document.getElementById('in-id').innerText;
                appState.nom = "ANONYME"; appState.prenom = ""; appState.matricule = "N/A";
                appState.societe = "N/A"; appState.poste = "N/A"; appState.district = "N/A";
                appState.service = serviceVal;
            }

            const wantWebcam = document.getElementById('in-webcam').checked;
            if (wantWebcam) startWebcam();

            // SÉLECTION BASE DE DONNÉES (Les tableaux intégraux ci-dessus)
            let basePool = [];
            if (appState.service === 'Contrôle électrique') basePool = JSON.parse(JSON.stringify(poolControle));
            else if (appState.service === 'Maintenance Poste') basePool = JSON.parse(JSON.stringify(poolMaintenance));
            else if (appState.service === 'Maintenance Ligne (ML)') basePool = JSON.parse(JSON.stringify(poolMaintenanceLigne));
            else if (appState.service === 'CE ESSAIS/ANALYSES') basePool = JSON.parse(JSON.stringify(poolEssaisAnalyses));
            else if (appState.service === 'Télécom & Téléconduite') basePool = JSON.parse(JSON.stringify(poolTelecom));
            else basePool = JSON.parse(JSON.stringify(poolExploitation)); 

            const nbReq = document.getElementById('in-num-q').value;
            basePool = shuffleArray(basePool);
            
            if (nbReq !== 'all') appState.testQuestions = basePool.slice(0, Math.min(parseInt(nbReq), basePool.length));
            else appState.testQuestions = basePool;
            
            appState.currentQuestion = 0; 
            appState.answers = appState.testQuestions.map((_, i) => ({ questionIndex: i, selected: -1, isCorrect: false }));
            startTimer();
            window.renderQuestion();
        }

        window.renderQuestion = function() {
            const qIndex = appState.currentQuestion;
            const q = appState.testQuestions[qIndex];
            const progress = ((qIndex) / appState.testQuestions.length) * 100;
            const typeBg = q.type === "Épreuve Écrite" ? "bg-blue-50 text-sonelgaz-blue border-blue-200" : "bg-orange-50 text-sonelgaz-orange border-orange-200";

            let optionsHtml = '';
            const previouslySelected = appState.answers[qIndex].selected;

            q.options.forEach((opt, index) => {
                const isChecked = (previouslySelected === index) ? 'checked' : '';
                optionsHtml += `
                    <div class="relative mb-3 fade-in" style="animation-delay: ${index * 0.05}s">
                        <input type="radio" name="q-option" id="opt-${index}" value="${index}" class="radio-custom sr-only peer" onchange="window.selectAnswer(${index})" ${isChecked}>
                        <label for="opt-${index}" class="flex items-start p-4 bg-white border-2 border-slate-100 rounded-xl cursor-pointer hover:bg-slate-50 transition-all peer-focus:ring-2 peer-focus:ring-sonelgaz-blue shadow-sm">
                            <div class="radio-circle w-5 h-5 border-2 border-slate-300 rounded-full mr-3 mt-0.5 flex-shrink-0 flex items-center justify-center transition-colors"><div class="w-2.5 h-2.5 bg-white rounded-full"></div></div>
                            <span class="text-slate-700 font-medium text-sm md:text-base">${opt}</span>
                        </label>
                    </div>`;
            });

            // Ajout du support Image si présent dans la base
            const imageHtml = q.image ? `<div class="mt-4 mb-4 p-4 bg-blue-50 border border-blue-100 rounded-lg text-center text-sm font-bold text-sonelgaz-blue shadow-inner"><i class="fas fa-image text-2xl block mb-2"></i> ${q.image}</div>` : '';

            const identity = appState.mode === 'declaratif' ? `${appState.nom} ${appState.prenom}` : `Anonyme`;
            const prevBtnState = qIndex === 0 ? 'invisible' : '';
            const nextBtnText = qIndex === appState.testQuestions.length - 1 ? 'Terminer / إنهاء <i class="fas fa-flag-checkered"></i>' : 'Suivant / التالي <i class="fas fa-arrow-right"></i>';
            const nextBtnColor = qIndex === appState.testQuestions.length - 1 ? 'bg-green-600 hover:bg-green-700' : 'bg-sonelgaz-blue hover:bg-blue-700';

            appContainer.innerHTML = `
                <div class="bg-white rounded-2xl shadow-xl w-full max-w-4xl overflow-hidden fade-in border border-slate-200 flex flex-col h-[85vh] max-h-[800px]">
                    <div class="p-4 border-b border-slate-100 shrink-0 bg-slate-50">
                        <div class="flex justify-between items-center mb-3">
                            <div class="flex flex-col">
                                <span class="text-[10px] font-bold text-slate-400 uppercase">Candidat (${appState.service})</span>
                                <span class="text-sm font-bold text-slate-700"><i class="fas fa-user-tag text-sonelgaz-blue mr-1"></i> ${identity}</span>
                            </div>
                            <div class="flex flex-col items-end">
                                <span class="text-sm font-bold bg-white border px-3 py-1 rounded-lg text-slate-600 shadow-sm">Q ${qIndex + 1} / ${appState.testQuestions.length}</span>
                            </div>
                        </div>
                        <div class="w-full bg-slate-200 rounded-full h-1.5"><div class="bg-sonelgaz-orange h-1.5 rounded-full transition-all duration-500" style="width: ${progress}%"></div></div>
                    </div>

                    <div class="p-6 overflow-y-auto flex-grow custom-scrollbar bg-slate-50">
                        <div class="inline-flex items-center gap-2 px-3 py-1 rounded-md text-xs font-bold border ${typeBg} mb-5 shadow-sm"><i class="fas fa-tag"></i> ${q.theme}</div>
                        <h2 class="text-lg md:text-xl font-bold text-slate-800 mb-2 leading-relaxed border-l-4 border-sonelgaz-blue pl-4">${q.question}</h2>
                        ${imageHtml}
                        <div class="options-container space-y-2 mt-4">${optionsHtml}</div>
                    </div>

                    <div class="p-4 border-t border-slate-100 bg-white shrink-0 flex justify-between items-center">
                        <button onclick="window.confirmQuit()" class="text-slate-500 hover:text-red-600 font-bold text-sm px-4 py-2 rounded-lg hover:bg-red-50 transition border border-transparent hover:border-red-200">
                            <i class="fas fa-times mr-1"></i> Quitter / خروج
                        </button>
                        <div class="flex gap-3">
                            <button onclick="window.prevQuestion()" class="${prevBtnState} bg-slate-200 hover:bg-slate-300 text-slate-700 font-bold py-3 px-6 rounded-xl shadow-sm transition flex items-center gap-2">
                                <i class="fas fa-arrow-left"></i> Précédent
                            </button>
                            <button onclick="window.nextQuestion()" class="${nextBtnColor} text-white font-bold py-3 px-8 rounded-xl shadow-md transition flex items-center gap-2">
                                ${nextBtnText}
                            </button>
                        </div>
                    </div>
                </div>
            `;
        }

        window.selectAnswer = function(selectedIndex) {
            const qIndex = appState.currentQuestion;
            const q = appState.testQuestions[qIndex];
            appState.answers[qIndex].selected = selectedIndex;
            appState.answers[qIndex].isCorrect = (selectedIndex === q.correctIndex);
        }

        window.prevQuestion = function() {
            if (appState.currentQuestion > 0) { appState.currentQuestion--; window.renderQuestion(); }
        }

        window.nextQuestion = function() {
            if (appState.answers[appState.currentQuestion].selected === -1) {
                showCustomAlert("Réponse manquante", "Veuillez sélectionner une réponse pour pouvoir avancer / يرجى اختيار إجابة للمتابعة.", "error"); return;
            }
            if (appState.currentQuestion < appState.testQuestions.length - 1) {
                appState.currentQuestion++; window.renderQuestion();
            } else {
                window.saveResultAndRender();
            }
        }

        window.confirmQuit = function() {
            showCustomConfirm(
                "Annuler l'examen ?", 
                "Attention, si vous quittez maintenant, l'examen sera annulé et vos résultats ne seront pas sauvegardés.", 
                () => {
                    clearInterval(appState.timerInterval);
                    document.getElementById('global-timer').classList.add('hidden');
                    stopWebcam();
                    window.renderIntro();
                }, 
                "Oui, quitter", "Continuer l'examen"
            );
        }

        window.saveResultAndRender = function() {
            clearInterval(appState.timerInterval);
            document.getElementById('global-timer').classList.add('hidden');
            stopWebcam();
            
            appState.score = appState.answers.filter(a => a.isCorrect).length;
            const percentage = Math.round((appState.score / appState.testQuestions.length) * 100);
            const timeUsed = 3600 - appState.timeRemaining;
            
            const resultData = {
                id: appState.id, mode: appState.mode,
                nom: appState.nom, prenom: appState.prenom, matricule: appState.matricule, 
                societe: appState.societe, poste: appState.poste, service: appState.service, district: appState.district,
                score: appState.score, total: appState.testQuestions.length, percentage: percentage, 
                date: new Date().toLocaleString('fr-FR'), timeUsed: timeUsed,
                answers: JSON.parse(JSON.stringify(appState.answers)),
                testSnapshot: JSON.parse(JSON.stringify(appState.testQuestions))
            };
            
            window.allCandidatesResults.unshift(resultData);
            saveToLocalStorage(); 
            renderFinalScore(resultData);
        }

        function renderFinalScore(data) {
            let statusClass, statusText, statusIcon;
            if (data.percentage >= 80) { statusClass = "text-green-700 bg-green-50 border-green-500"; statusText = "Avis Favorable / مقبول"; statusIcon = "fa-check-double"; } 
            else if (data.percentage >= 60) { statusClass = "text-sonelgaz-orange bg-orange-50 border-sonelgaz-orange"; statusText = "Avis Réservé / بتحفظ"; statusIcon = "fa-triangle-exclamation"; } 
            else { statusClass = "text-red-700 bg-red-50 border-red-500"; statusText = "Avis Défavorable / مرفوض"; statusIcon = "fa-skull-crossbones"; }

            appContainer.innerHTML = `
                <div class="bg-white rounded-2xl shadow-xl w-full max-w-3xl overflow-hidden fade-in border border-slate-200">
                    <div class="bg-slate-900 p-8 text-white text-center border-b-4 border-sonelgaz-orange relative">
                        <i class="fas fa-clipboard-check text-5xl mb-4 text-sonelgaz-blue drop-shadow-lg"></i>
                        <h2 class="text-2xl font-bold font-arabic mb-1">تقرير التقييم النهائي</h2>
                        <h2 class="text-xl font-bold">Fin de l'évaluation (${data.service})</h2>
                        <p class="text-slate-300 mt-2 text-sm">${data.mode === 'declaratif' ? `${data.nom} ${data.prenom} | Mat: ${data.matricule}` : `Anonyme (${data.id})`}</p>
                    </div>
                    <div class="p-8 text-center bg-slate-50">
                        <div class="bg-white p-6 rounded-2xl shadow-sm border border-slate-200 mb-6 inline-block w-full max-w-sm mx-auto">
                            <h3 class="text-slate-400 font-bold uppercase text-xs mb-2">Score Final / النتيجة</h3>
                            <div class="text-6xl font-black text-slate-800">${data.score} <span class="text-2xl text-slate-400">/ ${data.total}</span></div>
                            <div class="mt-4 text-sm font-semibold border-l-4 pl-4 py-2 ${statusClass} rounded-r-lg text-left"><i class="fas ${statusIcon} mr-2"></i> ${statusText}</div>
                        </div>
                        <div class="flex flex-col gap-3 justify-center items-center">
                            <button onclick="window.renderCandidateCorrection()" class="w-full max-w-xs bg-sonelgaz-blue hover:bg-blue-700 text-white font-bold py-3 px-8 rounded-xl shadow-md transition flex items-center justify-center gap-2">
                                <i class="fas fa-tasks"></i> Voir la Correction / عرض التصحيح
                            </button>
                            <button onclick="window.renderIntro()" class="w-full max-w-xs bg-slate-800 hover:bg-slate-900 text-white font-bold py-3 px-8 rounded-xl shadow-md transition flex items-center justify-center gap-2">
                                <i class="fas fa-home"></i> Accueil / الرئيسية
                            </button>
                        </div>
                    </div>
                </div>
            `;
        }

        // --- NOUVEAU: VUE CORRECTION POUR LE CANDIDAT (Avec Images/Photos Bilingue) ---
        window.renderCandidateCorrection = function() {
            const cand = window.allCandidatesResults[0]; // Dernier test
            let detailsHtml = ''; 
            
            cand.answers.forEach((ans, i) => {
                const q = cand.testSnapshot[ans.questionIndex];
                const selectedText = ans.selected === -1 ? "Non répondu / لم يتم الرد" : q.options[ans.selected];
                const isCorrect = ans.isCorrect;
                
                const bgColor = isCorrect ? "bg-green-50 border-green-200" : "bg-red-50 border-red-200";
                const iconColor = isCorrect ? "text-green-600" : "text-red-600";
                const iconClass = isCorrect ? "fa-check-circle" : "fa-times-circle";
                const badgeBg = isCorrect ? "bg-green-200 text-green-800" : "bg-red-200 text-red-800";
                
                const imageHtml = q.image ? `<div class="mt-4 mb-2 p-3 bg-white border border-slate-200 rounded-lg text-center text-sm font-bold text-slate-500 shadow-sm"><i class="fas fa-image text-sonelgaz-blue text-xl block mb-2"></i> ${q.image}</div>` : '';

                detailsHtml += `
                    <div class="mb-4 p-5 ${bgColor} border rounded-xl shadow-sm">
                        <p class="text-sm font-bold text-slate-800 mb-3 leading-relaxed">
                            <span class="${badgeBg} px-2 py-0.5 rounded text-xs mr-2 shadow-sm">Q${i+1} | ${q.theme}</span>
                            ${q.question}
                        </p>
                        ${imageHtml}
                        <div class="bg-white/60 p-3 rounded-lg border border-white/50">
                            <p class="text-xs md:text-sm ${iconColor} mb-2 font-semibold"><i class="fas ${iconClass} mr-1"></i> <strong>Votre Réponse :</strong> ${selectedText}</p>
                            ${!isCorrect ? `<p class="text-xs md:text-sm text-green-700 font-semibold"><i class="fas fa-check mr-1"></i> <strong>Bonne Réponse :</strong> ${q.options[q.correctIndex]}</p>` : ''}
                        </div>
                        <div class="mt-3 bg-blue-50/50 p-3 border-l-4 border-sonelgaz-blue rounded-r-lg">
                            <p class="text-xs text-blue-900 leading-relaxed"><strong>Justification :</strong> ${q.justification}</p>
                        </div>
                    </div>`;
            });

            appContainer.innerHTML = `
                <div class="bg-white rounded-2xl shadow-2xl w-full max-w-5xl overflow-hidden fade-in border border-slate-200 h-[90vh] flex flex-col">
                    <div class="bg-slate-900 p-6 flex justify-between items-center text-white border-b-4 border-sonelgaz-orange shrink-0 no-print">
                        <div class="flex items-center gap-3">
                            <i class="fas fa-check-double text-sonelgaz-blue text-3xl"></i>
                            <div><h2 class="text-xl font-bold">Correction Détaillée / التصحيح المفصل</h2><p class="text-sm text-slate-400">${cand.nom} ${cand.prenom} | ${cand.percentage}%</p></div>
                        </div>
                        <div class="flex gap-3">
                            <button onclick="window.print()" class="bg-sonelgaz-blue hover:bg-blue-600 px-4 py-2 rounded-xl text-sm font-bold transition shadow-md"><i class="fas fa-file-pdf mr-2"></i> Enregistrer PDF</button>
                            <button onclick="window.renderIntro()" class="bg-slate-700 hover:bg-slate-600 px-4 py-2 rounded-xl text-sm font-bold transition shadow-md"><i class="fas fa-home mr-2"></i> Terminer</button>
                        </div>
                    </div>
                    <div class="p-6 md:p-10 flex-grow overflow-y-auto custom-scrollbar bg-slate-50 print:bg-white print:p-0">
                        <!-- En-tête visible uniquement à l'impression -->
                        <div class="hidden print:block text-center mb-8 border-b-2 pb-4">
                            <h1 class="text-2xl font-bold text-slate-800">Rapport de Test d'Habilitation SONELGAZ</h1>
                            <p class="text-lg">Candidat : ${cand.nom} ${cand.prenom} | Score : ${cand.percentage}% | Spécialité : ${cand.service}</p>
                        </div>
                        <div class="space-y-2">
                            ${detailsHtml}
                        </div>
                    </div>
                </div>
            `;
        }

        // --- DASHBOARD ADMIN ---
        window.showAdminLogin = function() {
            appContainer.innerHTML = `
                <div class="bg-white rounded-2xl shadow-2xl w-full max-w-sm overflow-hidden fade-in p-8 text-center relative border border-slate-200">
                    <button onclick="window.renderIntro()" class="absolute top-4 right-4 text-slate-400 hover:bg-slate-100 p-2 rounded-lg transition"><i class="fas fa-times"></i></button>
                    <div class="w-20 h-20 bg-slate-800 text-sonelgaz-orange rounded-full flex items-center justify-center mx-auto mb-6"><i class="fas fa-user-shield text-3xl"></i></div>
                    <h2 class="text-2xl font-bold mb-4">Espace Administrateur</h2>
                    <input type="password" id="admin-password" class="w-full px-4 py-4 bg-slate-50 border border-slate-200 rounded-xl text-center text-2xl tracking-[0.3em] mb-4 outline-none focus:ring-2 focus:ring-sonelgaz-blue" placeholder="••••••••">
                    <button onclick="window.verifyAdmin()" class="w-full bg-sonelgaz-blue text-white font-bold py-3.5 rounded-xl shadow-md hover:bg-blue-700 transition"><i class="fas fa-unlock"></i> Connexion</button>
                </div>
            `;
        }

        window.verifyAdmin = function() {
            if (document.getElementById('admin-password').value === '15041978') window.renderAdminDashboard(); 
            else showCustomAlert("Erreur", "Code d'accès administrateur incorrect.", "error");
        }

        window.exportToCSV = function() {
            if (window.allCandidatesResults.length === 0) return showCustomAlert("Exportation impossible", "La base de données est vide.", "error");
            let csvContent = "\uFEFF Date;Identifiant;Mode;Nom;Prénom;Matricule;Société;Poste;Service;District;Score;Total Questions;Pourcentage;Temps (secondes)\n";
            window.allCandidatesResults.forEach(res => {
                let row = [ res.date, res.id, res.mode, res.nom, res.prenom, res.matricule, res.societe, res.poste, res.service, res.district, res.score, res.total, res.percentage + "%", res.timeUsed ];
                csvContent += row.map(e => `"${(e || '').toString().replace(/"/g, '""')}"`).join(";") + "\n";
            });
            const blob = new Blob([csvContent], { type: 'text/csv;charset=utf-8;' });
            const url = URL.createObjectURL(blob);
            const link = document.createElement("a"); link.setAttribute("href", url); link.setAttribute("download", `Resultats_Habilitation_Sonelgaz_${new Date().toISOString().slice(0,10)}.csv`);
            document.body.appendChild(link); link.click(); document.body.removeChild(link);
        }

        window.renderAdminDashboard = function() {
            let tableRows = window.allCandidatesResults.length === 0 ? `<tr><td colspan=\"5\" class=\"p-8 text-center text-slate-400\"><i class=\"fas fa-database text-3xl mb-3 block\"></i>Base de données vide.</td></tr>` : '';
            window.allCandidatesResults.forEach((res, index) => {
                let badgeClass = res.percentage >= 80 ? "bg-green-100 text-green-800" : (res.percentage >= 60 ? "bg-orange-100 text-orange-800" : "bg-red-100 text-red-800");
                const identity = res.mode === 'declaratif' ? `<div class="font-bold text-slate-800">${res.nom} ${res.prenom}</div><div class="text-[10px] text-slate-500">Mat: ${res.matricule} | ${res.district}</div>` : `<div class="font-mono text-sonelgaz-blue font-bold">${res.id}</div>`;
                tableRows += `
                    <tr class="hover:bg-slate-50 border-b border-slate-100">
                        <td class="px-4 py-3 text-xs text-slate-500 whitespace-nowrap">${res.date.split(' ')[0]}<br>${res.date.split(' ')[1]}</td>
                        <td class="px-4 py-3">${identity}</td>
                        <td class="px-4 py-3 text-xs text-slate-600">${res.poste}<br><span class="font-bold text-sonelgaz-blue">${res.service}</span></td>
                        <td class="px-4 py-3 text-center"><span class="px-2 py-1 text-xs font-bold rounded ${badgeClass}">${res.percentage}%</span></td>
                        <td class="px-4 py-3 text-center"><button onclick="window.viewCandidateDetailsAdmin(${index})" class="text-sonelgaz-blue bg-blue-50 px-3 py-1.5 rounded-lg text-xs font-bold hover:bg-blue-100 transition"><i class="fas fa-search"></i> Détails</button></td>
                    </tr>`;
            });

            appContainer.innerHTML = `
                <div class="bg-white rounded-2xl shadow-2xl w-full max-w-6xl overflow-hidden fade-in border border-slate-200 flex flex-col h-[90vh]">
                    <div class="bg-slate-900 p-5 flex flex-wrap justify-between items-center text-white border-b-4 border-sonelgaz-orange gap-4">
                        <div>
                            <h2 class="text-xl font-bold"><i class="fas fa-chart-pie text-sonelgaz-orange mr-2"></i> Tableau de Bord Admin</h2>
                            <span class="text-green-400 text-xs"><i class="fas fa-hard-drive"></i> Mode Local Sécurisé</span>
                        </div>
                        <div class="flex flex-wrap gap-3">
                            <button onclick="window.exportToCSV()" class="bg-green-600 hover:bg-green-500 px-4 py-2 rounded-xl text-sm font-bold transition flex items-center shadow-md"><i class="fas fa-file-excel mr-2"></i> Exporter (Excel)</button>
                            <button onclick="window.confirmClearDialog()" class="bg-red-600 hover:bg-red-700 px-4 py-2 rounded-xl text-sm font-bold transition flex items-center shadow-md text-white"><i class="fas fa-trash-alt mr-2"></i> Purger</button>
                            <button onclick="window.renderIntro()" class="bg-slate-700 hover:bg-slate-600 px-4 py-2 rounded-xl text-sm font-bold transition flex items-center shadow-md"><i class="fas fa-sign-out-alt mr-2"></i> Quitter</button>
                        </div>
                    </div>
                    <div class="overflow-auto flex-grow bg-slate-50">
                        <table class="min-w-full divide-y divide-slate-200">
                            <thead class="bg-slate-100 sticky top-0 shadow-sm z-10">
                                <tr>
                                    <th class="px-4 py-3 text-left text-xs font-bold text-slate-500 uppercase">Date</th>
                                    <th class="px-4 py-3 text-left text-xs font-bold text-slate-500 uppercase">Identité</th>
                                    <th class="px-4 py-3 text-left text-xs font-bold text-slate-500 uppercase">Poste / Service</th>
                                    <th class="px-4 py-3 text-center text-xs font-bold text-slate-500 uppercase">Score</th>
                                    <th class="px-4 py-3 text-center text-xs font-bold text-slate-500 uppercase">Action</th>
                                </tr>
                            </thead>
                            <tbody class="bg-white">${tableRows}</tbody>
                        </table>
                    </div>
                </div>
            `;
        }

        window.confirmClearDialog = function() {
            showCustomConfirm(
                "Purger les données ?",
                "Cette action est définitive. Tous les rapports d'examen locaux de cette session seront effacés.",
                () => { window.allCandidatesResults = []; saveToLocalStorage(); window.renderAdminDashboard(); },
                "Oui, purger"
            );
        }

        window.viewCandidateDetailsAdmin = function(index) {
            const cand = window.allCandidatesResults[index];
            let detailsHtml = ''; 
            
            cand.answers.forEach((ans, i) => {
                const q = cand.testSnapshot[ans.questionIndex];
                const selectedText = ans.selected === -1 ? "Non répondu (Ignoré)" : q.options[ans.selected];
                const isCorrect = ans.isCorrect;
                
                const bgColor = isCorrect ? "bg-green-50 border-green-200" : "bg-red-50 border-red-200";
                const iconColor = isCorrect ? "text-green-600" : "text-red-600";
                const iconClass = isCorrect ? "fa-check-circle" : "fa-times-circle";
                const badgeBg = isCorrect ? "bg-green-200 text-green-800" : "bg-red-200 text-red-800";

                detailsHtml += `
                    <div class="mb-3 p-4 ${bgColor} border rounded-lg shadow-sm">
                        <p class="text-sm font-bold text-slate-800 mb-2"><span class="${badgeBg} px-2 py-0.5 rounded text-xs mr-2">Q${i+1} | ${q.theme}</span>${q.question}</p>
                        <p class="text-xs ${iconColor} mb-1 font-semibold"><i class="fas ${iconClass} mr-1"></i> Réponse : ${selectedText}</p>
                        ${!isCorrect ? `<p class="text-xs text-green-700 font-semibold mt-1"><i class="fas fa-check mr-1"></i> Requise : ${q.options[q.correctIndex]}</p>` : ''}
                    </div>`;
            });

            const timeStr = `${Math.floor(cand.timeUsed / 60)} min ${cand.timeUsed % 60} sec`;

            appContainer.innerHTML = `
                <div class="bg-white rounded-2xl shadow-2xl w-full max-w-5xl overflow-hidden fade-in border border-slate-200 h-[85vh] flex flex-col">
                    <div class="bg-slate-100 p-4 border-b flex justify-between shrink-0">
                        <button onclick="window.renderAdminDashboard()" class="text-slate-600 font-bold text-sm bg-white px-4 py-2 rounded-lg border shadow-sm hover:bg-slate-50"><i class="fas fa-arrow-left mr-2"></i> Retour</button>
                        <span class="font-mono text-xs text-slate-400 pt-2">Session ID: ${cand.id}</span>
                    </div>
                    <div class="p-6 flex-grow overflow-y-auto bg-slate-50 flex flex-col gap-6">
                        <div class="bg-slate-900 rounded-xl p-6 shadow-lg text-white border-b-4 border-sonelgaz-blue flex justify-between items-center">
                            <div>
                                <h3 class="font-bold text-xl mb-1 flex items-center gap-2"><i class="fas fa-brain text-sonelgaz-blue"></i> Analyse Intelligente HSE</h3>
                                <p class="text-sm text-slate-400">Générez un rapport complet sur les failles techniques de ce candidat.</p>
                            </div>
                            <button onclick="window.renderAIAnalysisPage(${index})" class="bg-sonelgaz-blue hover:bg-blue-600 text-white font-bold py-3 px-6 rounded-xl transition shadow-md flex items-center gap-2">Générer Rapport <i class="fas fa-magic"></i></button>
                        </div>
                        <div class="bg-white p-6 rounded-xl border shadow-sm">
                            <div class="flex justify-between items-start mb-4">
                                <div>
                                    <h3 class="text-2xl font-bold">${cand.nom} ${cand.prenom}</h3>
                                    <p class="text-sm font-bold text-sonelgaz-blue uppercase mt-1">${cand.service}</p>
                                    <p class="text-xs text-slate-500">${cand.poste} | ${cand.societe}</p>
                                </div>
                                <div class="text-right"><div class="text-3xl font-black ${cand.percentage >= 80 ? 'text-green-600' : 'text-red-600'}">${cand.percentage}%</div><div class="text-xs text-slate-400">${cand.score}/${cand.total}</div></div>
                            </div>
                            <div class="grid grid-cols-3 gap-2 text-xs text-slate-600 bg-slate-50 p-3 rounded-lg border">
                                <div><strong>Matricule:</strong><br>${cand.matricule}</div>
                                <div><strong>District:</strong><br>${cand.district}</div>
                                <div><strong>Temps:</strong><br>${timeStr}</div>
                            </div>
                        </div>
                        <div><h3 class="text-lg font-bold mb-3"><i class="fas fa-list-check text-sonelgaz-blue mr-2"></i> Détail des réponses</h3><div class="space-y-2">${detailsHtml}</div></div>
                    </div>
                </div>
            `;
        }

        window.renderAIAnalysisPage = function(idx) {
            const cand = window.allCandidatesResults[idx];
            appContainer.innerHTML = `
                <div class="bg-white rounded-2xl shadow-2xl w-full max-w-5xl overflow-hidden fade-in border border-slate-200 min-h-[70vh] flex flex-col items-center justify-center p-10">
                    <div class="text-sonelgaz-blue text-6xl mb-6"><i class="fas fa-brain animate-pulse"></i></div>
                    <h2 class="text-2xl font-bold text-slate-800 mb-2">Génération de l'expertise IA en cours...</h2>
                    <p class="text-slate-500 mb-8 text-center max-w-lg">L'Intelligence Artificielle analyse les erreurs de ${cand.nom} spécifiques à sa spécialité (${cand.service}) pour rédiger un rapport détaillé.</p>
                    <div class="w-64 bg-slate-200 rounded-full h-2 overflow-hidden relative"><div class="bg-sonelgaz-orange h-2 absolute w-1/2 rounded-full animate-[progress_1.5s_ease-in-out_infinite]"></div></div>
                </div>
            `;

            setTimeout(() => {
                let erreursHtml = ''; let risquesArray = []; let nbErrors = 0;
                cand.answers.forEach(a => {
                    if (!a.isCorrect && a.selected !== -1) {
                        nbErrors++; const q = cand.testSnapshot[a.questionIndex];
                        erreursHtml += `<li><strong>Faiblesse en [${q.theme}] :</strong> Le candidat a choisi "${q.options[a.selected]}" au lieu de la procédure stricte ("${q.options[q.correctIndex]}").</li>`;
                        if(q.theme.includes("SF6") || q.theme.includes("Transformateur") || q.theme.includes("Buchholz") || q.theme.includes("OLTC")) risquesArray.push("Risque matériel majeur (Explosion de cuve, Incendie des huiles).");
                        if(q.theme.includes("Consignation") || q.theme.includes("MALT") || q.theme.includes("Tension de Pas")) risquesArray.push("Risque mortel d'électrocution pour le personnel (Réalimentation accidentelle, gradient de tension).");
                        if(q.theme.includes("Protection") || q.theme.includes("Relais") || q.theme.includes("Injection") || q.theme.includes("SCADA") || q.theme.includes("Télécom") || q.theme.includes("Réseaux")) risquesArray.push("Risque de perte totale de visibilité (Blind) ou de contrôle du poste menant au black-out complet.");
                        if(q.theme.includes("Hauteur") || q.theme.includes("Point Mort") || q.theme.includes("Harnais")) risquesArray.push("Risque mortel de chute de grande hauteur lié au non-respect de l'ancrage 100%.");
                        if(q.theme.includes("Lavage") || q.theme.includes("Téléphone") || q.theme.includes("VLAN")) risquesArray.push("Risque de cyberattaque ou d'arc électrique à distance par négligence des protocoles.");
                    }
                });

                let htmlContent = nbErrors === 0 
                    ? `<p><strong>Le candidat a obtenu un excellent score.</strong> Aucune faille technique majeure détectée.</p>`
                    : `<h3>1. Résumé</h3><p>Le candidat a obtenu <strong>${cand.percentage}%</strong>. L'analyse révèle des lacunes sur ${nbErrors} point(s).</p>
                       <h3>2. Lacunes Techniques</h3><ul>${erreursHtml}</ul>
                       <h3>3. Risques Terrain / Cybersécurité</h3><ul>${[...new Set(risquesArray)].map(r=>`<li>${r}</li>`).join('')}</ul>
                       <h3>4. Recommandations</h3><ul><li>Un recyclage ciblé sur (${cand.service}) est indispensable avant toute manœuvre complexe.</li></ul>`;

                appContainer.innerHTML = `
                    <div class="bg-white rounded-2xl shadow-2xl w-full max-w-5xl overflow-hidden fade-in border border-slate-200 flex flex-col h-[85vh]">
                        <div class="bg-slate-900 p-6 flex justify-between items-center text-white border-b-4 border-sonelgaz-blue shrink-0">
                            <div class="flex items-center gap-3"><i class="fas fa-robot text-sonelgaz-blue text-3xl"></i><div><h2 class="text-xl font-bold">Rapport d'Expertise IA</h2><p class="text-sm text-slate-400">Pour ${cand.nom} ${cand.prenom}</p></div></div>
                            <div class="flex gap-3">
                                <button onclick="window.print()" class="bg-slate-700 hover:bg-slate-600 px-4 py-2 rounded-xl text-sm font-bold"><i class="fas fa-print mr-2"></i> Imprimer</button>
                                <button onclick="window.viewCandidateDetailsAdmin(${idx})" class="bg-sonelgaz-orange hover:bg-orange-600 px-4 py-2 rounded-xl text-sm font-bold"><i class="fas fa-arrow-left mr-2"></i> Retour</button>
                            </div>
                        </div>
                        <div class="p-8 overflow-y-auto flex-grow bg-slate-50"><div class="bg-white p-8 rounded-xl shadow-sm border ai-report text-slate-800">${htmlContent}</div></div>
                    </div>`;
            }, 1000); 
        }

        renderIntro();
    </script>
</body>
</html>
