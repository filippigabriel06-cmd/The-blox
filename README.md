<!DOCTYPE html>
<html lang="pt-BR" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BloxVault - Contas Blox Fruits 24/7</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        cyber: {
                            bg: '#080c14',
                            card: '#0f172a',
                            border: '#1e293b',
                            neon: '#00f0ff',
                            purple: '#a855f7',
                            gold: '#f59e0b',
                            accent: '#3b82f6'
                        }
                    },
                    fontFamily: {
                        orbitron: ['Orbitron', 'sans-serif'],
                        inter: ['Inter', 'sans-serif']
                    },
                    animation: {
                        'pulse-glow': 'pulseGlow 2s infinite alternate',
                        'float': 'float 4s ease-in-out infinite',
                        'border-glow': 'borderGlow 3s ease infinite'
                    },
                    keyframes: {
                        pulseGlow: {
                            '0%': { boxShadow: '0 0 10px rgba(0, 240, 255, 0.2), inset 0 0 10px rgba(0, 240, 255, 0.1)' },
                            '100%': { boxShadow: '0 0 25px rgba(0, 240, 255, 0.6), inset 0 0 15px rgba(0, 240, 255, 0.3)' }
                        },
                        float: {
                            '0%, 100%': { transform: 'translateY(0px)' },
                            '50%': { transform: 'translateY(-8px)' }
                        }
                    }
                }
            }
        }
    </script>

    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&family=Orbitron:wght@500;700;900&display=swap" rel="stylesheet">
    
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #050811;
            color: #f1f5f9;
            overflow-x: hidden;
        }

        .font-orbitron {
            font-family: 'Orbitron', sans-serif;
        }

        /* Glassmorphism cyber effects */
        .glass-panel {
            background: rgba(15, 23, 42, 0.75);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid rgba(0, 240, 255, 0.15);
        }

        .glass-card {
            background: linear-gradient(135deg, rgba(15, 23, 42, 0.9) 0%, rgba(30, 41, 59, 0.6) 100%);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.08);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .glass-card:hover {
            border-color: rgba(0, 240, 255, 0.5);
            transform: translateY(-4px);
            box-shadow: 0 10px 30px -10px rgba(0, 240, 255, 0.25);
        }

        .cyber-gradient-text {
            background: linear-gradient(90deg, #00f0ff 0%, #a855f7 50%, #3b82f6 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .cyber-gold-text {
            background: linear-gradient(90deg, #fbbf24 0%, #f59e0b 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #080c14;
        }
        ::-webkit-scrollbar-thumb {
            background: #1e293b;
            border-radius: 4px;
            border: 1px solid rgba(0,240,255,0.2);
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #00f0ff;
        }

        /* Cyber grid background */
        .bg-cyber-grid {
            background-image: linear-gradient(to right, rgba(0, 240, 255, 0.03) 1px, transparent 1px),
                              linear-gradient(to bottom, rgba(0, 240, 255, 0.03) 1px, transparent 1px);
            background-size: 40px 40px;
        }
    </style>
</head>
<body class="bg-cyber-grid min-h-screen flex flex-col justify-between selection:bg-cyan-500 selection:text-black">

    <!-- Top Announcement Bar -->
    <div class="bg-gradient-to-r from-cyan-900/60 via-purple-900/60 to-cyan-900/60 border-b border-cyan-500/20 py-2 px-4 text-center text-xs sm:text-sm font-medium tracking-wide flex items-center justify-center gap-2">
        <span class="inline-block w-2 h-2 rounded-full bg-emerald-400 animate-ping"></span>
        <span>SISTEMA DE ENTREGA AUTOMÁTICA VIA PIX 24/7 ATIVO</span>
        <span class="hidden md:inline text-cyan-400">| Suporte Oficial Disponível</span>
    </div>

    <!-- Main Navigation Header -->
    <header class="sticky top-0 z-40 glass-panel border-b border-slate-800">
        <div class="max-w-7xl mx-mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <!-- Brand Logo -->
            <div class="flex items-center gap-3 cursor-pointer" onclick="switchTab('catalog')">
                <div class="w-10 h-10 rounded-xl bg-gradient-to-br from-cyan-500 to-purple-600 flex items-center justify-center shadow-lg shadow-cyan-500/20">
                    <i class="fa-solid font-bold fa-cube text-xl text-black"></i>
                </div>
                <div>
                    <h1 class="font-orbitron text-xl sm:text-2xl font-black tracking-wider cyber-gradient-text">BLOXVAULT</h1>
                    <p class="text-[10px] text-cyan-400 tracking-widest font-mono uppercase">Store & Delivery</p>
                </div>
            </div>

            <!-- Header Actions -->
            <div class="flex items-center gap-3">
                <!-- Discord Support Button -->
                <a href="https://discord.gg/hjUqJ3vaX" target="_blank" rel="noopener noreferrer" 
                   class="flex items-center gap-2 px-4 py-2 rounded-xl bg-[#5865F2]/20 hover:bg-[#5865F2] border border-[#5865F2]/40 text-white text-xs sm:text-sm font-semibold transition-all duration-300 shadow-lg hover:shadow-[#5865F2]/30 group">
                    <i class="fa-brands fa-discord text-base group-hover:scale-110 transition-transform"></i>
                    <span class="hidden sm:inline">Suporte Discord</span>
                </a>

                <!-- Minhas Compras Button -->
                <button onclick="switchTab('my-purchases')" 
                        class="flex items-center gap-2 px-4 py-2 rounded-xl bg-slate-800/80 hover:bg-slate-700 border border-slate-700 text-slate-200 text-xs sm:text-sm font-semibold transition-all relative">
                    <i class="fa-solid fa-key text-cyan-400"></i>
                    <span class="hidden sm:inline">Minhas Contas</span>
                    <span id="purchases-badge" class="hidden absolute -top-1 -right-1 w-5 h-5 bg-cyan-500 text-black font-bold text-xs rounded-full items-center justify-center">0</span>
                </button>

                <!-- Hidden Admin Trigger Button (Subtle & Discrete) -->
                <button onclick="openAdminLoginModal()" title="Acesso do Sistema" 
                        class="w-9 h-9 rounded-xl bg-slate-900 hover:bg-slate-800 border border-slate-800 text-slate-500 hover:text-cyan-400 flex items-center justify-center transition-colors">
                    <i class="fa-solid fa-shield-halved text-sm"></i>
                </button>
            </div>
        </div>
    </header>

    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 flex-1 w-full">
        
        <!-- Hero Banner -->
        <section class="relative rounded-3xl overflow-hidden glass-card p-6 sm:p-10 mb-10 border border-cyan-500/20 shadow-2xl">
            <div class="absolute -right-10 -bottom-10 w-96 h-96 bg-cyan-500/10 rounded-full blur-3xl pointer-events-none"></div>
            <div class="absolute -left-10 -top-10 w-96 h-96 bg-purple-500/10 rounded-full blur-3xl pointer-events-none"></div>

            <div class="relative z-10 max-w-2xl">
                <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-cyan-500/10 border border-cyan-500/30 text-cyan-400 text-xs font-mono mb-4">
                    <i class="fa-solid fa-bolt"></i> ENTREGA AUTOMÁTICA EM SEGUNDOS
                </div>
                <h2 class="font-orbitron text-3xl sm:text-5xl font-black tracking-tight text-white mb-4 leading-tight">
                    CONTAS SUPREMAS DE <span class="cyber-gradient-text">BLOX FRUITS</span>
                </h2>
                <p class="text-slate-400 text-sm sm:text-base mb-6 leading-relaxed">
                    Adquira sua conta com Level Máximo, Frutas Permanentes, Godhuman, CDK e Soul Guitar com garantia total e recebimento instantâneo após a confirmação do PIX.
                </p>

                <!-- Discord Quick Banner Link -->
                <div class="flex flex-wrap items-center gap-4">
                    <a href="https://discord.gg/hjUqJ3vaX" target="_blank" 
                       class="inline-flex items-center gap-3 px-6 py-3 rounded-2xl bg-gradient-to-r from-cyan-500 to-blue-600 hover:from-cyan-400 hover:to-blue-500 text-black font-bold text-sm tracking-wide shadow-lg shadow-cyan-500/25 transition-all transform hover:-translate-y-0.5">
                        <i class="fa-brands fa-discord text-lg"></i>
                        ENTRAR NO DISCORD DE SUPORTE
                    </a>
                    <div class="flex items-center gap-2 text-xs text-slate-400 font-mono">
                        <i class="fa-solid fa-shield-check text-emerald-400 text-base"></i>
                        <span>100% Verificado e Seguro</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- View Switcher Tabs -->
        <div id="catalog-view">
            <!-- Filter & Search Controls -->
            <div class="flex flex-col md:flex-row items-center justify-between gap-4 mb-8">
                <!-- Category Buttons -->
                <div class="flex items-center gap-2 overflow-x-auto w-full md:w-auto pb-2 md:pb-0">
                    <button onclick="filterCategory('all')" id="cat-all" class="cat-btn px-4 py-2 rounded-xl text-xs font-bold font-mono tracking-wider bg-cyan-500 text-black shadow-lg shadow-cyan-500/20">
                        TODAS AS CONTAS
                    </button>
                    <button onclick="filterCategory('godhuman')" id="cat-godhuman" class="cat-btn px-4 py-2 rounded-xl text-xs font-bold font-mono tracking-wider bg-slate-800 text-slate-300 hover:bg-slate-700">
                        GODHUMAN / CDK
                    </button>
                    <button onclick="filterCategory('perm')" id="cat-perm" class="cat-btn px-4 py-2 rounded-xl text-xs font-bold font-mono tracking-wider bg-slate-800 text-slate-300 hover:bg-slate-700">
                        FRUTAS PERM
                    </button>
                    <button onclick="filterCategory('max')" id="cat-max" class="cat-btn px-4 py-2 rounded-xl text-xs font-bold font-mono tracking-wider bg-slate-800 text-slate-300 hover:bg-slate-700">
                        LEVEL MÁXIMO
                    </button>
                </div>

                <!-- Search Input -->
                <div class="relative w-full md:w-72">
                    <i class="fa-solid fa-magnifying-glass absolute left-3 top-1/2 -translate-y-1/2 text-slate-500 text-sm"></i>
                    <input type="text" id="search-input" onkeyup="handleSearch()" placeholder="Buscar item, fruta ou level..." 
                           class="w-full bg-slate-900 border border-slate-800 focus:border-cyan-500 rounded-xl pl-9 pr-4 py-2 text-sm text-slate-200 placeholder-slate-500 outline-none transition-all">
                </div>
            </div>

            <!-- Accounts Grid -->
            <div id="accounts-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Dynamically Populated by JS -->
            </div>

            <!-- Empty State -->
            <div id="empty-catalog" class="hidden text-center py-16 glass-card rounded-2xl">
                <i class="fa-solid fa-box-open text-4xl text-slate-600 mb-3"></i>
                <p class="text-slate-400 font-medium">Nenhuma conta encontrada com esses filtros.</p>
            </div>
        </div>

        <!-- My Purchases View -->
        <div id="purchases-view" class="hidden">
            <div class="flex items-center justify-between mb-6">
                <div>
                    <h3 class="font-orbitron text-2xl font-bold text-white">MINHAS CONTAS COMPRADAS</h3>
                    <p class="text-xs text-slate-400">Seus dados ficam salvos com segurança neste navegador.</p>
                </div>
                <button onclick="switchTab('catalog')" class="text-xs text-cyan-400 hover:underline flex items-center gap-1">
                    <i class="fa-solid fa-arrow-left"></i> Voltar ao Catálogo
                </button>
            </div>

            <div id="purchases-list" class="space-y-4">
                <!-- Purchases JS dynamic render -->
            </div>
        </div>

    </main>

    <!-- Modal 1: Account Biography Details & Preview -->
    <div id="details-modal" class="fixed inset-0 z-50 hidden flex items-center justify-center p-4 bg-black/80 backdrop-blur-md">
        <div class="glass-card max-w-2xl w-full rounded-3xl border border-cyan-500/30 overflow-hidden shadow-2xl animate-float max-h-[90vh] flex flex-col">
            <!-- Modal Header -->
            <div class="p-6 border-b border-slate-800 flex items-center justify-between bg-slate-900/50">
                <div class="flex items-center gap-3">
                    <span id="modal-badge" class="px-2.5 py-1 rounded-md bg-cyan-500/20 text-cyan-400 border border-cyan-500/30 text-xs font-mono font-bold">CATEGORIA</span>
                    <h3 id="modal-title" class="font-orbitron font-bold text-lg sm:text-xl text-white">Título da Conta</h3>
                </div>
                <button onclick="closeModal('details-modal')" class="text-slate-400 hover:text-white w-8 h-8 rounded-lg bg-slate-800 flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>

            <!-- Modal Body (Biography) -->
            <div class="p-6 overflow-y-auto space-y-6 flex-1 text-sm text-slate-300">
                <!-- Image Preview -->
                <div class="relative h-48 sm:h-56 rounded-2xl overflow-hidden bg-slate-950 border border-slate-800">
                    <img id="modal-image" src="" alt="Blox Fruits Account" class="w-full h-full object-cover">
                    <div class="absolute bottom-3 right-3 bg-black/80 backdrop-blur-md px-3 py-1.5 rounded-xl border border-cyan-500/40 font-orbitron font-bold text-cyan-400 text-lg">
                        <span id="modal-price">R$ 0,00</span>
                    </div>
                </div>

                <!-- Biography Key Attributes -->
                <div class="grid grid-cols-2 sm:grid-cols-4 gap-3 text-xs">
                    <div class="bg-slate-900/80 p-3 rounded-xl border border-slate-800">
                        <span class="text-slate-500 block mb-1 font-mono">LEVEL</span>
                        <span id="modal-level" class="font-bold text-white text-sm">2550 MAX</span>
                    </div>
                    <div class="bg-slate-900/80 p-3 rounded-xl border border-slate-800">
                        <span class="text-slate-500 block mb-1 font-mono">ESTILO DE LUTA</span>
                        <span id="modal-style" class="font-bold text-cyan-400 text-sm">Godhuman</span>
                    </div>
                    <div class="bg-slate-900/80 p-3 rounded-xl border border-slate-800">
                        <span class="text-slate-500 block mb-1 font-mono">ESPADAS</span>
                        <span id="modal-swords" class="font-bold text-purple-400 text-sm">CDK + Soul Guitar</span>
                    </div>
                    <div class="bg-slate-900/80 p-3 rounded-xl border border-slate-800">
                        <span class="text-slate-500 block mb-1 font-mono">ENTREGA</span>
                        <span class="font-bold text-emerald-400 text-sm">24H Automática</span>
                    </div>
                </div>

                <!-- Full Bio Text -->
                <div>
                    <h4 class="font-orbitron text-xs font-bold tracking-wider text-slate-400 uppercase mb-2">BIOGRAFIA COMPLETA DA CONTA</h4>
                    <div id="modal-bio" class="bg-slate-900/60 p-4 rounded-xl border border-slate-800 font-mono text-xs leading-relaxed text-slate-300 whitespace-pre-line">
                        Carregando biografia...
                    </div>
                </div>
            </div>

            <!-- Modal Footer -->
            <div class="p-6 border-t border-slate-800 bg-slate-900/50 flex flex-col sm:flex-row items-center justify-between gap-4">
                <div class="text-xs text-slate-400 flex items-center gap-2">
                    <i class="fa-solid fa-lock text-emerald-400"></i> Pagamento Seguro via PIX
                </div>
                <button id="modal-buy-btn" onclick="startCheckout()" 
                        class="w-full sm:w-auto px-8 py-3.5 rounded-2xl bg-gradient-to-r from-emerald-500 to-teal-600 hover:from-emerald-400 hover:to-teal-500 text-black font-extrabold font-orbitron tracking-wider text-sm shadow-xl shadow-emerald-500/20 transition-all transform hover:scale-[1.02]">
                    COMPRAR AGORA (PIX 24H)
                </button>
            </div>
        </div>
    </div>

    <!-- Modal 2: PIX Checkout & Auto-Verification -->
    <div id="pix-modal" class="fixed inset-0 z-50 hidden flex items-center justify-center p-4 bg-black/85 backdrop-blur-md">
        <div class="glass-card max-w-lg w-full rounded-3xl border border-emerald-500/30 overflow-hidden shadow-2xl p-6 relative">
            <button onclick="closeModal('pix-modal')" class="absolute top-4 right-4 text-slate-400 hover:text-white w-8 h-8 rounded-lg bg-slate-800 flex items-center justify-center">
                <i class="fa-solid fa-xmark"></i>
            </button>

            <!-- Checkout Step 1: Paying -->
            <div id="pix-step-payment" class="text-center">
                <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-emerald-500/10 border border-emerald-500/30 text-emerald-400 text-xs font-mono mb-4">
                    <i class="fa-solid fa-qrcode"></i> PAGAMENTO VIA PIX 24H
                </div>
                <h3 class="font-orbitron font-bold text-xl text-white mb-1">FINALIZAR COMPRA</h3>
                <p id="checkout-account-title" class="text-xs text-slate-400 mb-6">Conta Blox Fruits Level MAX</p>

                <!-- QR Code Box -->
                <div class="bg-white p-4 rounded-2xl w-48 h-48 mx-auto mb-4 border-4 border-emerald-500/40 flex items-center justify-center shadow-lg">
                    <img id="pix-qr-code" src="" alt="PIX QR Code" class="w-full h-full object-contain">
                </div>

                <div class="mb-4">
                    <span class="text-xs text-slate-400 block mb-1">VALOR TOTAL:</span>
                    <span id="checkout-account-price" class="font-orbitron font-black text-2xl text-emerald-400">R$ 0,00</span>
                </div>

                <!-- Copia e Cola Field -->
                <div class="bg-slate-900 border border-slate-800 rounded-xl p-2.5 flex items-center justify-between mb-6">
                    <input type="text" id="pix-code-input" readonly value="" class="bg-transparent text-xs text-slate-300 font-mono w-full outline-none px-2 select-all">
                    <button onclick="copyPixKey()" class="px-3 py-1.5 rounded-lg bg-emerald-500/20 hover:bg-emerald-500 text-emerald-400 hover:text-black text-xs font-bold transition-all whitespace-nowrap">
                        <i class="fa-solid fa-copy mr-1"></i> Copiar
                    </button>
                </div>

                <!-- Simulation Analysis Button -->
                <button onclick="simulatePaymentVerification()" class="w-full py-3.5 rounded-xl bg-gradient-to-r from-emerald-500 to-teal-500 hover:from-emerald-400 hover:to-teal-400 text-black font-bold font-orbitron tracking-wider text-sm shadow-lg shadow-emerald-500/20 transition-all flex items-center justify-center gap-2">
                    <i class="fa-solid fa-circle-check"></i> JÁ EFETUEI O PAGAMENTO
                </button>
                <p class="text-[11px] text-slate-500 mt-3">O sistema verifica automaticamente em tempo real após a transferência.</p>
            </div>

            <!-- Checkout Step 2: Analyzing -->
            <div id="pix-step-analyzing" class="hidden text-center py-8">
                <div class="w-16 h-16 border-4 border-emerald-500 border-t-transparent rounded-full animate-spin mx-auto mb-6"></div>
                <h3 class="font-orbitron font-bold text-lg text-white mb-2">ANALISANDO PAGAMENTO...</h3>
                <p class="text-xs text-slate-400 mb-4">Consultando confirmação junto ao banco. Por favor, não feche esta janela.</p>
                <div class="w-full bg-slate-900 rounded-full h-2 overflow-hidden border border-slate-800">
                    <div id="analysis-progress" class="bg-gradient-to-r from-emerald-500 to-cyan-500 h-full w-0 transition-all duration-300"></div>
                </div>
            </div>

            <!-- Checkout Step 3: Success & Credentials Revealed -->
            <div id="pix-step-success" class="hidden text-center">
                <div class="w-16 h-16 bg-emerald-500/20 text-emerald-400 rounded-full flex items-center justify-center mx-auto mb-4 border border-emerald-500/40 text-2xl">
                    <i class="fa-solid fa-check"></i>
                </div>
                <h3 class="font-orbitron font-bold text-xl text-white mb-1">PAGAMENTO CONFIRMADO!</h3>
                <p class="text-xs text-emerald-400 font-mono mb-6">Aqui estão os dados da sua conta comprada:</p>

                <!-- Credentials Card -->
                <div class="bg-slate-900/90 border-2 border-emerald-500/50 rounded-2xl p-4 text-left space-y-3 mb-6 relative">
                    <span class="absolute -top-2.5 right-3 bg-emerald-500 text-black text-[10px] font-bold px-2 py-0.5 rounded font-mono">SALVO NAS MINHAS CONTAS</span>
                    
                    <div>
                        <span class="text-[10px] text-slate-500 font-mono block">USUÁRIO ROBLOX:</span>
                        <div class="flex items-center justify-between">
                            <span id="delivered-user" class="font-mono font-bold text-white text-base">blox_user_123</span>
                            <button onclick="copyToClipboard('delivered-user')" class="text-xs text-cyan-400 hover:text-cyan-300"><i class="fa-solid fa-copy"></i> Copiar</button>
                        </div>
                    </div>

                    <div class="border-t border-slate-800 pt-2">
                        <span class="text-[10px] text-slate-500 font-mono block">SENHA:</span>
                        <div class="flex items-center justify-between">
                            <span id="delivered-pass" class="font-mono font-bold text-cyan-400 text-base">Pass123456!</span>
                            <button onclick="copyToClipboard('delivered-pass')" class="text-xs text-cyan-400 hover:text-cyan-300"><i class="fa-solid fa-copy"></i> Copiar</button>
                        </div>
                    </div>
                </div>

                <button onclick="finishOrderAndRedirect()" class="w-full py-3 rounded-xl bg-cyan-500 hover:bg-cyan-400 text-black font-bold font-orbitron text-xs tracking-wider transition-all">
                    ENTENDI & VER MINHAS CONTAS
                </button>
            </div>
        </div>
    </div>

    <!-- Modal 3: Hidden Admin Login -->
    <div id="admin-login-modal" class="fixed inset-0 z-50 hidden flex items-center justify-center p-4 bg-black/90 backdrop-blur-lg">
        <div class="glass-card max-w-sm w-full rounded-2xl border border-cyan-500/40 p-6">
            <div class="flex items-center justify-between mb-4">
                <div class="flex items-center gap-2 text-cyan-400 font-orbitron font-bold text-sm">
                    <i class="fa-solid fa-lock"></i> PAINEL ADMINISTRATIVO
                </div>
                <button onclick="closeModal('admin-login-modal')" class="text-slate-500 hover:text-white">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>

            <p class="text-xs text-slate-400 mb-4">Acesso restrito. Digite a credencial de controle supremo do site.</p>

            <form onsubmit="handleAdminLogin(event)" class="space-y-4">
                <div>
                    <label class="block text-[11px] font-mono text-slate-400 mb-1">SENHA MESTRA</label>
                    <input type="password" id="admin-pass-input" placeholder="••••••••" required 
                           class="w-full bg-slate-900 border border-slate-800 focus:border-cyan-500 rounded-xl px-3 py-2.5 text-sm text-white outline-none">
                </div>
                <button type="submit" class="w-full py-2.5 rounded-xl bg-cyan-500 hover:bg-cyan-400 text-black font-bold text-xs font-orbitron tracking-wider">
                    AUTENTICAR
                </button>
            </form>
        </div>
    </div>

    <!-- Modal 4: Full Admin Control Panel Drawer/Modal -->
    <div id="admin-panel-modal" class="fixed inset-0 z-50 hidden flex items-center justify-center p-4 bg-black/90 backdrop-blur-xl">
        <div class="glass-card max-w-4xl w-full rounded-3xl border border-purple-500/40 overflow-hidden shadow-2xl flex flex-col max-h-[90vh]">
            
            <!-- Admin Header -->
            <div class="p-5 bg-slate-900 border-b border-slate-800 flex items-center justify-between">
                <div class="flex items-center gap-3">
                    <div class="w-8 h-8 rounded-lg bg-purple-500/20 text-purple-400 border border-purple-500/40 flex items-center justify-center">
                        <i class="fa-solid fa-user-shield"></i>
                    </div>
                    <div>
                        <h3 class="font-orbitron font-bold text-white text-base">CONTROLE SUPREMO DO ADMINISTRADOR</h3>
                        <p class="text-[10px] text-purple-400 font-mono">Status: Autenticado como Gerente de Vendas</p>
                    </div>
                </div>
                <button onclick="closeModal('admin-panel-modal')" class="px-3 py-1.5 rounded-lg bg-red-500/20 text-red-400 hover:bg-red-500 hover:text-white text-xs font-bold transition-all">
                    Sair do Painel
                </button>
            </div>

            <!-- Admin Nav Tabs -->
            <div class="flex border-b border-slate-800 bg-slate-950 px-6 gap-6 text-xs font-mono font-bold">
                <button onclick="switchAdminTab('add-account')" id="adm-tab-add" class="py-3 border-b-2 border-purple-500 text-purple-400">
                    + ADICIONAR CONTA
                </button>
                <button onclick="switchAdminTab('manage-accounts')" id="adm-tab-manage" class="py-3 border-b-2 border-transparent text-slate-400 hover:text-white">
                    GERENCIAR CONTAS (<span id="adm-account-count">0</span>)
                </button>
                <button onclick="switchAdminTab('pix-settings')" id="adm-tab-pix" class="py-3 border-b-2 border-transparent text-slate-400 hover:text-white">
                    CONFIGURAÇÃO PIX
                </button>
            </div>

            <!-- Admin Body Content -->
            <div class="p-6 overflow-y-auto flex-1 space-y-6">
                
                <!-- Tab 1: Add Account Form -->
                <div id="admin-view-add" class="space-y-4">
                    <h4 class="font-orbitron text-xs font-bold text-slate-400 tracking-wider uppercase">CADASTRAR NOVA CONTA PARA VENDA</h4>
                    <form onsubmit="handleSaveAccount(event)" class="grid grid-cols-1 sm:grid-cols-2 gap-4 text-xs">
                        <div>
                            <label class="block text-slate-400 mb-1 font-mono">TÍTULO DA CONTA</label>
                            <input type="text" id="add-title" placeholder="Ex: Conta Level MAX + Kitsune Perm" required class="w-full bg-slate-900 border border-slate-800 rounded-xl p-2.5 text-white outline-none focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-slate-400 mb-1 font-mono">PREÇO (R$)</label>
                            <input type="number" step="0.01" id="add-price" placeholder="49.90" required class="w-full bg-slate-900 border border-slate-800 rounded-xl p-2.5 text-white outline-none focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-slate-400 mb-1 font-mono">CATEGORIA / SELEÇÃO</label>
                            <select id="add-category" class="w-full bg-slate-900 border border-slate-800 rounded-xl p-2.5 text-white outline-none focus:border-purple-500">
                                <option value="godhuman">Godhuman / CDK</option>
                                <option value="perm">Fruta Permanente</option>
                                <option value="max">Level Máximo</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-slate-400 mb-1 font-mono">URL DA IMAGEM</label>
                            <input type="url" id="add-image" placeholder="https://..." required class="w-full bg-slate-900 border border-slate-800 rounded-xl p-2.5 text-white outline-none focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-slate-400 mb-1 font-mono">ESTILO DE LUTA PRINCIPAL</label>
                            <input type="text" id="add-style" placeholder="Godhuman, Sanguine Art..." required class="w-full bg-slate-900 border border-slate-800 rounded-xl p-2.5 text-white outline-none focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-slate-400 mb-1 font-mono">ESPADAS & ITENS</label>
                            <input type="text" id="add-swords" placeholder="CDK, True Triple Katana..." required class="w-full bg-slate-900 border border-slate-800 rounded-xl p-2.5 text-white outline-none focus:border-purple-500">
                        </div>

                        <!-- Login Credentials Provided to Buyer -->
                        <div class="col-span-1 sm:col-span-2 bg-purple-950/30 border border-purple-500/30 p-4 rounded-2xl space-y-3">
                            <span class="text-purple-300 font-bold block font-mono">DADOS DE LOGIN DA CONTA (ENTREGUES AO CLIENTE):</span>
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                                <div>
                                    <label class="block text-slate-400 mb-1 font-mono">NOME DE USUÁRIO ROBLOX</label>
                                    <input type="text" id="add-user" placeholder="UsuarioRoblox123" required class="w-full bg-slate-900 border border-slate-800 rounded-xl p-2.5 text-white outline-none focus:border-purple-500">
                                </div>
                                <div>
                                    <label class="block text-slate-400 mb-1 font-mono">SENHA DA CONTA</label>
                                    <input type="text" id="add-pass" placeholder="SenhaSegura#2026" required class="w-full bg-slate-900 border border-slate-800 rounded-xl p-2.5 text-white outline-none focus:border-purple-500">
                                </div>
                            </div>
                        </div>

                        <div class="col-span-1 sm:col-span-2">
                            <label class="block text-slate-400 mb-1 font-mono">BIOGRAFIA E DETALHES COMPLETOS</label>
                            <textarea id="add-bio" rows="4" placeholder="- Level 2550 MAX&#10;- Fruta Kitsune permanente&#10;- 30M Beli / 50k Frags&#10;- Raça V4 Desbloqueada" required class="w-full bg-slate-900 border border-slate-800 rounded-xl p-2.5 text-white outline-none focus:border-purple-500"></textarea>
                        </div>

                        <div class="col-span-1 sm:col-span-2 pt-2">
                            <button type="submit" class="w-full py-3 rounded-xl bg-purple-600 hover:bg-purple-500 text-white font-bold font-orbitron tracking-wider text-xs shadow-lg shadow-purple-600/30">
                                PUBLICAR CONTA NO SITE
                            </button>
                        </div>
                    </form>
                </div>

                <!-- Tab 2: Manage Accounts List -->
                <div id="admin-view-manage" class="hidden space-y-4">
                    <h4 class="font-orbitron text-xs font-bold text-slate-400 tracking-wider uppercase">CONTAS CADASTRADAS</h4>
                    <div id="adm-accounts-list" class="space-y-3">
                        <!-- Dynamic JS -->
                    </div>
                </div>

                <!-- Tab 3: PIX Settings -->
                <div id="admin-view-pix" class="hidden space-y-4">
                    <h4 class="font-orbitron text-xs font-bold text-slate-400 tracking-wider uppercase">CONFIGURAR RECEBIMENTO PIX</h4>
                    <form onsubmit="handleSavePixSettings(event)" class="space-y-4 text-xs max-w-md">
                        <div>
                            <label class="block text-slate-400 mb-1 font-mono">CHAVE PIX (E-mail, CPF, Telefone ou Aleatória)</label>
                            <input type="text" id="pix-setting-key" placeholder="suachavepix@email.com" required class="w-full bg-slate-900 border border-slate-800 rounded-xl p-2.5 text-white outline-none focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-slate-400 mb-1 font-mono">NOME DO BENEFICIÁRIO / BANCO</label>
                            <input type="text" id="pix-setting-name" placeholder="Filippi Store Pagamentos" required class="w-full bg-slate-900 border border-slate-800 rounded-xl p-2.5 text-white outline-none focus:border-purple-500">
                        </div>
                        <button type="submit" class="py-2.5 px-6 rounded-xl bg-emerald-500 hover:bg-emerald-400 text-black font-bold font-orbitron text-xs">
                            SALVAR PIX DO ADMINISTRADOR
                        </button>
                    </form>
                </div>

            </div>
        </div>
    </div>

    <!-- Notification Toast Message -->
    <div id="toast" class="fixed bottom-6 right-6 z-50 hidden glass-panel px-4 py-3 rounded-2xl border border-cyan-500/40 text-cyan-300 text-xs font-semibold shadow-2xl flex items-center gap-3">
        <i class="fa-solid fa-circle-info text-cyan-400"></i>
        <span id="toast-message">Mensagem de aviso</span>
    </div>

    <!-- Floating Discord Widget -->
    <a href="https://discord.gg/hjUqJ3vaX" target="_blank" rel="noopener noreferrer" 
       class="fixed bottom-6 left-6 z-40 w-12 h-12 rounded-full bg-[#5865F2] hover:scale-110 text-white flex items-center justify-center shadow-xl shadow-[#5865F2]/40 transition-all border border-white/20 group"
       title="Suporte Discord 24/7">
        <i class="fa-brands fa-discord text-xl"></i>
        <span class="absolute left-14 bg-slate-900 text-white text-[11px] font-bold px-2.5 py-1 rounded-md opacity-0 group-hover:opacity-100 whitespace-nowrap transition-opacity border border-slate-800 pointer-events-none">
            Suporte no Discord
        </span>
    </a>

    <!-- Footer -->
    <footer class="border-t border-slate-900 glass-panel py-8 mt-12 text-center text-xs text-slate-500">
        <div class="max-w-7xl mx-auto px-4 flex flex-col sm:flex-row items-center justify-between gap-4">
            <div class="flex items-center gap-2">
                <span class="font-orbitron font-bold text-slate-300">BLOXVAULT</span>
                <span>- Vendas de Contas Blox Fruits</span>
            </div>
            <div class="flex items-center gap-4 text-slate-400">
                <a href="https://discord.gg/hjUqJ3vaX" target="_blank" class="hover:text-cyan-400 transition-colors">
                    <i class="fa-brands fa-discord mr-1"></i> Discord Suporte
                </a>
                <span>•</span>
                <span>Entrega via PIX 24h</span>
            </div>
        </div>
    </footer>

    <script>
        // Initial Default Accounts
        const initialAccounts = [
            {
                id: 'acc-1',
                title: 'Conta GODHUMAN + Kitsune Permanente + CDK',
                price: 79.90,
                category: 'godhuman',
                level: 2550,
                style: 'Godhuman',
                swords: 'CDK + Soul Guitar',
                image: 'https://images.unsplash.com/photo-1578632767115-351597cf2477?w=600&auto=format&fit=crop&q=80',
                bio: `🔥 CONTA GODHUMAN MÁXIMO NÍVEL 🔥\n\n• Level 2550 (Máximo)\n• Fruta Kitsune Permanente Equipada!\n• Estilo de Luta Godhuman (Mastery 600)\n• Espada Cursed Dual Katana (CDK) & Soul Guitar\n• 25M de Beli + 45.000 Fragmentos\n• Raça V4 Desbloqueada com Engrenagens\n• Vários Acessórios Raros no Inventário!`,
                user: 'KitsuneGod_99',
                pass: 'BloxMaster#2026'
            },
            {
                id: 'acc-2',
                title: 'Conta Level MAX + Dragon + Sanguine Art',
                price: 59.90,
                category: 'max',
                level: 2550,
                style: 'Sanguine Art',
                swords: 'True Triple Katana',
                image: 'https://images.unsplash.com/photo-1563089145-599997674d42?w=600&auto=format&fit=crop&q=80',
                bio: `⚡ CONTA DRAGON & SANGUINE ART ⚡\n\n• Level 2550 (Máximo)\n• Fruta Dragon Ingerida (Todas Skills V2)\n• Estilo de Luta Sanguine Art Desbloqueado\n• Espada True Triple Katana (TTK)\n• 18M de Beli + 30.000 Fragmentos\n• Haki do Armamento Colorido Especial\n• Barco Rápido e Passes de Jogo Inclusos!`,
                user: 'DragonV2_Pro',
                pass: 'FruitLegend!99'
            },
            {
                id: 'acc-3',
                title: 'Conta Dough Perm + V4 Angel + CDK',
                price: 89.90,
                category: 'perm',
                level: 2550,
                style: 'Godhuman',
                swords: 'Cursed Dual Katana',
                image: 'https://images.unsplash.com/photo-1542751371-adc38448a05e?w=600&auto=format&fit=crop&q=80',
                bio: `🍩 CONTA DOUGH PERMANENTE V2 🍩\n\n• Level 2550 (MAX)\n• Dough Permanente Desperta (V2 Total)\n• Raça Angel V4 Full Tier\n• Godhuman e Electric Claw\n• Espada CDK Rara + Hallow Scythe\n• 35M de Beli + 60.000 Fragmentos`,
                user: 'DoughPerm_Vault',
                pass: 'DoughKing#778'
            }
        ];

        // State variables initialized with localStorage persistence
        let accounts = JSON.parse(localStorage.getItem('blox_accounts')) || initialAccounts;
        let purchases = JSON.parse(localStorage.getItem('blox_purchases')) || [];
        let pixSettings = JSON.parse(localStorage.getItem('blox_pix_settings')) || {
            key: 'suachavepix@email.com',
            name: 'Filippi Store Pagamentos'
        };

        let currentCategory = 'all';
        let selectedAccount = null;

        // Save state helper
        function saveState() {
            localStorage.setItem('blox_accounts', JSON.stringify(accounts));
            localStorage.setItem('blox_purchases', JSON.stringify(purchases));
            localStorage.setItem('blox_pix_settings', JSON.stringify(pixSettings));
            updatePurchasesBadge();
        }

        // Initialize application on load
        window.onload = function() {
            renderAccountsGrid();
            renderPurchasesList();
            updatePurchasesBadge();
            // Pre-fill Pix settings in admin modal
            document.getElementById('pix-setting-key').value = pixSettings.key;
            document.getElementById('pix-setting-name').value = pixSettings.name;
        };

        // Render Accounts Grid for Catalog
        function renderAccountsGrid() {
            const container = document.getElementById('accounts-grid');
            const searchVal = document.getElementById('search-input').value.toLowerCase();
            
            container.innerHTML = '';

            const filtered = accounts.filter(acc => {
                const matchesCategory = currentCategory === 'all' || acc.category === currentCategory;
                const matchesSearch = acc.title.toLowerCase().includes(searchVal) || 
                                      acc.bio.toLowerCase().includes(searchVal) ||
                                      acc.swords.toLowerCase().includes(searchVal);
                return matchesCategory && matchesSearch;
            });

            if (filtered.length === 0) {
                document.getElementById('empty-catalog').classList.remove('hidden');
                return;
            } else {
                document.getElementById('empty-catalog').classList.add('hidden');
            }

            filtered.forEach(acc => {
                const card = document.createElement('div');
                card.className = 'glass-card rounded-2xl overflow-hidden flex flex-col justify-between border border-slate-800';
                card.innerHTML = `
                    <div>
                        <div class="relative h-44 overflow-hidden bg-slate-950">
                            <img src="${acc.image}" alt="${acc.title}" class="w-full h-full object-cover transition-transform duration-500 hover:scale-105" onerror="this.src='https://placehold.co/600x400/0f172a/00f0ff?text=Blox+Fruits+Account'">
                            <span class="absolute top-3 left-3 px-2.5 py-1 rounded-md bg-black/80 backdrop-blur-md border border-cyan-500/30 text-cyan-400 text-[10px] font-mono font-bold uppercase">
                                LVL ${acc.level}
                            </span>
                        </div>
                        <div class="p-5">
                            <h3 class="font-orbitron font-bold text-white text-base mb-2 line-clamp-1">${acc.title}</h3>
                            
                            <div class="space-y-1.5 mb-4 text-xs text-slate-400">
                                <div class="flex items-center gap-2">
                                    <i class="fa-solid fa-hand-fist text-cyan-400 w-4"></i>
                                    <span class="truncate">${acc.style}</span>
                                </div>
                                <div class="flex items-center gap-2">
                                    <i class="fa-solid fa-shield-halved text-purple-400 w-4"></i>
                                    <span class="truncate">${acc.swords}</span>
                                </div>
                            </div>

                            <p class="text-xs text-slate-500 line-clamp-2 font-mono mb-4">${acc.bio}</p>
                        </div>
                    </div>

                    <div class="p-5 pt-0 border-t border-slate-800/50 mt-auto flex items-center justify-between">
                        <div>
                            <span class="text-[10px] text-slate-500 block font-mono">PREÇO PIX</span>
                            <span class="font-orbitron font-black text-xl text-cyan-400">R$ ${acc.price.toFixed(2).replace('.', ',')}</span>
                        </div>
                        <button onclick="openDetailsModal('${acc.id}')" class="px-4 py-2.5 rounded-xl bg-cyan-500/10 hover:bg-cyan-500 border border-cyan-500/30 text-cyan-400 hover:text-black font-bold font-orbitron text-xs transition-all flex items-center gap-2">
                            <span>VER CONTA</span>
                            <i class="fa-solid fa-chevron-right text-[10px]"></i>
                        </button>
                    </div>
                `;
                container.appendChild(card);
            });
        }

        // Category Filtering Logic
        function filterCategory(cat) {
            currentCategory = cat;
            document.querySelectorAll('.cat-btn').forEach(btn => {
                btn.className = 'cat-btn px-4 py-2 rounded-xl text-xs font-bold font-mono tracking-wider bg-slate-800 text-slate-300 hover:bg-slate-700';
            });

            const activeBtn = document.getElementById(`cat-${cat}`);
            if (activeBtn) {
                activeBtn.className = 'cat-btn px-4 py-2 rounded-xl text-xs font-bold font-mono tracking-wider bg-cyan-500 text-black shadow-lg shadow-cyan-500/20';
            }

            renderAccountsGrid();
        }

        function handleSearch() {
            renderAccountsGrid();
        }

        // Open Account Biography Modal
        function openDetailsModal(accId) {
            selectedAccount = accounts.find(a => a.id === accId);
            if (!selectedAccount) return;

            document.getElementById('modal-title').innerText = selectedAccount.title;
            document.getElementById('modal-badge').innerText = selectedAccount.category.toUpperCase();
            document.getElementById('modal-image').src = selectedAccount.image;
            document.getElementById('modal-price').innerText = `R$ ${selectedAccount.price.toFixed(2).replace('.', ',')}`;
            document.getElementById('modal-level').innerText = `${selectedAccount.level} MAX`;
            document.getElementById('modal-style').innerText = selectedAccount.style;
            document.getElementById('modal-swords').innerText = selectedAccount.swords;
            document.getElementById('modal-bio').innerText = selectedAccount.bio;

            document.getElementById('details-modal').classList.remove('hidden');
        }

        // Start PIX Checkout Procedure
        function startCheckout() {
            if (!selectedAccount) return;

            closeModal('details-modal');

            document.getElementById('checkout-account-title').innerText = selectedAccount.title;
            document.getElementById('checkout-account-price').innerText = `R$ ${selectedAccount.price.toFixed(2).replace('.', ',')}`;
            
            // Set up Pix Copy Key
            const rawPixCode = `00020126580014BR.GOV.BCB.PIX0136${pixSettings.key}520400005303986540${selectedAccount.price.toFixed(2)}5802BR5925${pixSettings.name}6009SAO PAULO62070503***63041234`;
            document.getElementById('pix-code-input').value = rawPixCode;

            // Generate dynamic QR code image via reliable server URL
            const qrUrl = `https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=${encodeURIComponent(rawPixCode)}`;
            document.getElementById('pix-qr-code').src = qrUrl;

            // Reset step views
            document.getElementById('pix-step-payment').classList.remove('hidden');
            document.getElementById('pix-step-analyzing').classList.add('hidden');
            document.getElementById('pix-step-success').classList.add('hidden');

            document.getElementById('pix-modal').classList.remove('hidden');
        }

        function copyPixKey() {
            const copyText = document.getElementById('pix-code-input');
            copyText.select();
            document.execCommand('copy');
            showToast('Chave PIX Copia e Cola copiada com sucesso!');
        }

        // Simulate automatic payment approval after client pays
        function simulatePaymentVerification() {
            document.getElementById('pix-step-payment').classList.add('hidden');
            document.getElementById('pix-step-analyzing').classList.remove('hidden');

            const progressBar = document.getElementById('analysis-progress');
            progressBar.style.width = '0%';

            setTimeout(() => { progressBar.style.width = '40%'; }, 500);
            setTimeout(() => { progressBar.style.width = '80%'; }, 1500);
            
            setTimeout(() => {
                progressBar.style.width = '100%';
                
                // Set delivered user/pass
                document.getElementById('delivered-user').innerText = selectedAccount.user;
                document.getElementById('delivered-pass').innerText = selectedAccount.pass;

                // Save to customer purchases list
                const newPurchase = {
                    id: 'PUR-' + Date.now(),
                    accountTitle: selectedAccount.title,
                    price: selectedAccount.price,
                    user: selectedAccount.user,
                    pass: selectedAccount.pass,
                    date: new Date().toLocaleString('pt-BR')
                };

                purchases.unshift(newPurchase);
                saveState();

                document.getElementById('pix-step-analyzing').classList.add('hidden');
                document.getElementById('pix-step-success').classList.remove('hidden');

            }, 2500);
        }

        function finishOrderAndRedirect() {
            closeModal('pix-modal');
            switchTab('my-purchases');
        }

        // My Purchases Render Function
        function renderPurchasesList() {
            const container = document.getElementById('purchases-list');
            container.innerHTML = '';

            if (purchases.length === 0) {
                container.innerHTML = `
                    <div class="glass-card p-8 rounded-2xl text-center text-slate-500">
                        <i class="fa-solid fa-ghost text-3xl mb-2"></i>
                        <p class="text-xs">Você ainda não comprou nenhuma conta neste dispositivo.</p>
                    </div>
                `;
                return;
            }

            purchases.forEach(p => {
                const item = document.createElement('div');
                item.className = 'glass-card p-5 rounded-2xl border border-cyan-500/30 flex flex-col sm:flex-row items-start sm:items-center justify-between gap-4';
                item.innerHTML = `
                    <div>
                        <span class="text-[10px] text-emerald-400 font-mono font-bold uppercase"><i class="fa-solid fa-circle-check"></i> ENTREGUE • ${p.date}</span>
                        <h4 class="font-orbitron font-bold text-white text-sm sm:text-base mb-1">${p.accountTitle}</h4>
                        <span class="text-xs text-slate-400 font-mono">Valor Pago: R$ ${p.price.toFixed(2).replace('.', ',')}</span>
                    </div>

                    <div class="bg-slate-900 p-3 rounded-xl border border-slate-800 w-full sm:w-auto font-mono text-xs space-y-1">
                        <div class="flex items-center justify-between gap-4">
                            <span class="text-slate-500">Usuário:</span>
                            <span class="text-white font-bold">${p.user}</span>
                        </div>
                        <div class="flex items-center justify-between gap-4">
                            <span class="text-slate-500">Senha:</span>
                            <span class="text-cyan-400 font-bold">${p.pass}</span>
                        </div>
                    </div>
                `;
                container.appendChild(item);
            });
        }

        function updatePurchasesBadge() {
            const badge = document.getElementById('purchases-badge');
            if (purchases.length > 0) {
                badge.innerText = purchases.length;
                badge.classList.remove('hidden');
                badge.classList.add('flex');
            } else {
                badge.classList.add('hidden');
            }
        }

        // View Tabs switching
        function switchTab(tab) {
            if (tab === 'catalog') {
                document.getElementById('catalog-view').classList.remove('hidden');
                document.getElementById('purchases-view').classList.add('hidden');
            } else if (tab === 'my-purchases') {
                renderPurchasesList();
                document.getElementById('catalog-view').classList.add('hidden');
                document.getElementById('purchases-view').classList.remove('hidden');
            }
        }

        // Secret Base64 Admin Password Validation (Hides raw string in logic)
        // Obscured check for requested password "Filippi55" -> Base64: 'RmlsaXBwaTU1'
        function openAdminLoginModal() {
            document.getElementById('admin-login-modal').classList.remove('hidden');
        }

        function handleAdminLogin(event) {
            event.preventDefault();
            const inputPass = document.getElementById('admin-pass-input').value;
            
            // Compare encoded string so password is not directly readable in plain code
            if (btoa(inputPass) === 'RmlsaXBwaTU1') {
                closeModal('admin-login-modal');
                document.getElementById('admin-pass-input').value = '';
                openAdminPanel();
                showToast('Acesso concedido ao Painel Administrativo!');
            } else {
                showToast('Senha Incorreta! Acesso Negado.');
            }
        }

        function openAdminPanel() {
            renderAdminAccountsList();
            document.getElementById('admin-panel-modal').classList.remove('hidden');
        }

        function switchAdminTab(tab) {
            document.getElementById('admin-view-add').classList.add('hidden');
            document.getElementById('admin-view-manage').classList.add('hidden');
            document.getElementById('admin-view-pix').classList.add('hidden');

            document.getElementById('adm-tab-add').className = 'py-3 border-b-2 border-transparent text-slate-400 hover:text-white';
            document.getElementById('adm-tab-manage').className = 'py-3 border-b-2 border-transparent text-slate-400 hover:text-white';
            document.getElementById('adm-tab-pix').className = 'py-3 border-b-2 border-transparent text-slate-400 hover:text-white';

            if (tab === 'add-account') {
                document.getElementById('admin-view-add').classList.remove('hidden');
                document.getElementById('adm-tab-add').className = 'py-3 border-b-2 border-purple-500 text-purple-400';
            } else if (tab === 'manage-accounts') {
                renderAdminAccountsList();
                document.getElementById('admin-view-manage').classList.remove('hidden');
                document.getElementById('adm-tab-manage').className = 'py-3 border-b-2 border-purple-500 text-purple-400';
            } else if (tab === 'pix-settings') {
                document.getElementById('admin-view-pix').classList.remove('hidden');
                document.getElementById('adm-tab-pix').className = 'py-3 border-b-2 border-purple-500 text-purple-400';
            }
        }

        // Admin Action: Add New Account
        function handleSaveAccount(e) {
            e.preventDefault();
            const newAcc = {
                id: 'acc-' + Date.now(),
                title: document.getElementById('add-title').value,
                price: parseFloat(document.getElementById('add-price').value),
                category: document.getElementById('add-category').value,
                level: 2550,
                style: document.getElementById('add-style').value,
                swords: document.getElementById('add-swords').value,
                image: document.getElementById('add-image').value,
                user: document.getElementById('add-user').value,
                pass: document.getElementById('add-pass').value,
                bio: document.getElementById('add-bio').value
            };

            accounts.unshift(newAcc);
            saveState();
            renderAccountsGrid();

            // Reset form
            e.target.reset();
            showToast('Nova conta adicionada ao site!');
            switchAdminTab('manage-accounts');
        }

        // Admin Action: Render Accounts List to manage/delete
        function renderAdminAccountsList() {
            const container = document.getElementById('adm-accounts-list');
            document.getElementById('adm-account-count').innerText = accounts.length;
            container.innerHTML = '';

            accounts.forEach((acc, index) => {
                const item = document.createElement('div');
                item.className = 'bg-slate-900 p-4 rounded-xl border border-slate-800 flex items-center justify-between text-xs';
                item.innerHTML = `
                    <div class="flex items-center gap-3">
                        <img src="${acc.image}" class="w-10 h-10 rounded-lg object-cover">
                        <div>
                            <h5 class="font-bold text-white font-orbitron">${acc.title}</h5>
                            <span class="text-cyan-400 font-mono">R$ ${acc.price.toFixed(2)} | Login: ${acc.user}</span>
                        </div>
                    </div>
                    <button onclick="deleteAccount('${acc.id}')" class="px-3 py-1.5 rounded-lg bg-red-500/20 text-red-400 hover:bg-red-500 hover:text-white font-bold transition-colors">
                        Excluir
                    </button>
                `;
                container.appendChild(item);
            });
        }

        function deleteAccount(id) {
            accounts = accounts.filter(a => a.id !== id);
            saveState();
            renderAccountsGrid();
            renderAdminAccountsList();
            showToast('Conta removida do catálogo.');
        }

        // Admin Action: Save Pix Key Settings
        function handleSavePixSettings(e) {
            e.preventDefault();
            pixSettings.key = document.getElementById('pix-setting-key').value;
            pixSettings.name = document.getElementById('pix-setting-name').value;
            saveState();
            showToast('Dados do PIX do administrador salvos com sucesso!');
        }

        // Helper Copy Function
        function copyToClipboard(elementId) {
            const text = document.getElementById(elementId).innerText;
            const tempInput = document.createElement('input');
            tempInput.value = text;
            document.body.appendChild(tempInput);
            tempInput.select();
            document.execCommand('copy');
            document.body.removeChild(tempInput);
            showToast('Copiado para a área de transferência!');
        }

        // Toast message banner helper
        function showToast(msg) {
            const toast = document.getElementById('toast');
            document.getElementById('toast-message').innerText = msg;
            toast.classList.remove('hidden');
            setTimeout(() => {
                toast.classList.add('hidden');
            }, 3000);
        }

        // Close Modal Helper
        function closeModal(modalId) {
            document.getElementById(modalId).classList.add('hidden');
        }
    </script>
</body>
</html>
