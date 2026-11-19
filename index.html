<!DOCTYPE html>
<html lang="ru" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GARANT SERVICE — Премиальный сервис замены масла</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-obsidian: #07090d;
            --bg-card: rgba(17, 22, 31, 0.88);
            --border-subtle: rgba(255, 255, 255, 0.08);
        }
        body {
            font-family: 'Manrope', sans-serif;
            background-color: var(--bg-obsidian);
            background-image:
                radial-gradient(circle at 15% 0%, rgba(229, 169, 60, 0.14), transparent 42%),
                radial-gradient(circle at 88% 12%, rgba(56, 189, 248, 0.06), transparent 38%),
                linear-gradient(180deg, #07090d 0%, #0b0e14 100%);
            color: #f3f5f8;
        }
        .glass-panel {
            background: var(--bg-card);
            backdrop-filter: blur(18px);
            -webkit-backdrop-filter: blur(18px);
            border: 1px solid var(--border-subtle);
            box-shadow: 0 24px 60px -15px rgba(0, 0, 0, 0.65);
        }
        .gold-glow {
            box-shadow: 0 10px 30px -6px rgba(229, 169, 60, 0.35);
        }
        @keyframes pulseRing {
            0%, 100% { opacity: 1; transform: scale(1); }
            50% { opacity: 0.45; transform: scale(1.15); }
        }
        .live-indicator {
            animation: pulseRing 2.2s infinite ease-in-out;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col selection:bg-amber-400 selection:text-slate-950">

    <header class="sticky top-0 z-30 border-b border-white/[0.07] bg-[#07090d]/85 backdrop-blur-xl">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 py-4 flex flex-wrap items-center justify-between gap-4">
            <div id="logo-trigger" onclick="handleSecretLogoTap()" class="flex items-center gap-3.5 cursor-pointer select-none group" title="GARANT SERVICE">
                <div class="w-11 h-11 rounded-2xl bg-gradient-to-br from-amber-300 via-amber-400 to-amber-600 text-slate-950 flex items-center justify-center gold-glow transition-transform duration-200 group-active:scale-95">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2.3" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M12 2.75c-3.6 4.35-6.5 7.95-6.5 11.2a6.5 6.5 0 0013 0c0-3.25-2.9-6.85-6.5-11.2z" />
                        <path stroke-linecap="round" stroke-linejoin="round" d="M9.75 14.25a2.25 2.25 0 002.25 2.25" />
                    </svg>
                </div>
                <div>
                    <div class="flex items-center gap-2">
                        <span class="text-lg sm:text-xl font-extrabold tracking-tight text-white">GARANT</span>
                        <span class="text-lg sm:text-xl font-extrabold tracking-tight text-amber-400">SERVICE</span>
                        <span class="hidden sm:inline-block text-[10px] font-bold uppercase tracking-[0.2em] px-2 py-0.5 rounded-full bg-amber-400/10 text-amber-300 border border-amber-400/25">
                            Atelier
                        </span>
                    </div>
                    <p class="text-xs text-slate-400">Премиальный сервис замены масла • Живая запись</p>
                </div>
            </div>

            <div class="flex items-center gap-3">
                <div class="flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-white/[0.04] border border-white/[0.08]">
                    <span class="w-2 h-2 rounded-full bg-emerald-400 live-indicator"></span>
                    <span id="sync-status-text" class="text-xs font-medium text-slate-300">Синхронизация...</span>
                </div>
                <button id="dev-logout-btn" onclick="logoutDeveloperMode()" class="hidden px-3.5 py-2 rounded-xl text-xs font-bold bg-amber-400 hover:bg-amber-300 text-slate-950 gold-glow transition cursor-pointer">
                    Выйти из режима разработчика
                </button>
            </div>
        </div>
    </header>

    <section id="developer-console" class="hidden border-b border-amber-400/25 bg-gradient-to-r from-[#14110b] via-[#18140d] to-[#11151d]">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 py-4 flex flex-wrap items-center justify-between gap-4">
            <div class="space-y-1">
                <div class="flex flex-wrap items-center gap-2.5">
                    <span class="text-[11px] font-extrabold uppercase tracking-[0.16em] px-2.5 py-1 rounded-lg bg-amber-400 text-slate-950">
                        Режим разработчика
                    </span>
                    <span class="text-xs sm:text-sm text-amber-200/90 font-semibold">
                        Талонов в базе: <strong id="dev-metric-total" class="text-white">0</strong> • Новых регистраций: <strong id="dev-metric-new" class="text-amber-400">0</strong>
                    </span>
                </div>
                <p class="text-xs text-slate-400">
                    При каждом новом талоне клиента вам приходит мгновенное уведомление со всеми данными.
                </p>
            </div>
            <div class="flex flex-wrap items-center gap-2.5">
                <button id="dev-sound-btn" onclick="activateDeveloperAlerts()" class="px-3.5 py-2 rounded-xl text-xs font-bold bg-emerald-500/15 hover:bg-emerald-500/25 text-emerald-300 border border-emerald-400/35 transition cursor-pointer">
                    🔔 Включить звук и уведомления
                </button>
                <button onclick="triggerSampleDeveloperAlert()" class="px-3.5 py-2 rounded-xl text-xs font-semibold bg-white/[0.06] hover:bg-white/[0.1] text-slate-200 border border-white/10 transition cursor-pointer">
                    Тест сигнала
                </button>
            </div>
        </div>
    </section>

    <main class="flex-grow max-w-7xl w-full mx-auto px-4 sm:px-6 py-7 grid grid-cols-1 lg:grid-cols-12 gap-7">
        <div class="lg:col-span-7 space-y-6">
            <div class="glass-panel rounded-3xl p-6 sm:p-7">
                <div class="flex flex-wrap items-center justify-between gap-4 mb-6">
                    <div>
                        <span class="text-[11px] font-bold uppercase tracking-[0.18em] text-amber-400">Шаг 01</span>
                        <h2 class="text-xl font-extrabold text-white mt-0.5">Дата и временной слот</h2>
                        <p class="text-xs sm:text-sm text-slate-400 mt-0.5">Обслуживание одного авто — 30 минут • Напоминания за 40 и 20 минут</p>
                    </div>
                    <div class="flex items-center gap-2">
                        <button type="button" onclick="changeDay(-1)" class="w-10 h-10 rounded-xl bg-white/[0.04] hover:bg-white/[0.09] border border-white/[0.08] flex items-center justify-center text-slate-300 transition cursor-pointer" title="Назад">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.2" d="M15 19l-7-7 7-7"/></svg>
                        </button>
                        <input type="date" id="booking-date" class="px-3.5 py-2 rounded-xl bg-[#090c10] border border-white/[0.12] text-sm font-bold text-white focus:border-amber-400 focus:ring-2 focus:ring-amber-400/20 outline-none">
                        <button type="button" onclick="changeDay(1)" class="w-10 h-10 rounded-xl bg-white/[0.04] hover:bg-white/[0.09] border border-white/[0.08] flex items-center justify-center text-slate-300 transition cursor-pointer" title="Вперёд">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.2" d="M9 5l7 7-7 7"/></svg>
                        </button>
                    </div>
                </div>

                <div class="flex flex-wrap items-center gap-5 text-xs text-slate-400 mb-5 pb-4 border-b border-white/[0.07]">
                    <div class="flex items-center gap-2"><span class="w-3 h-3 rounded-full bg-emerald-400/80"></span><span>Свободно</span></div>
                    <div class="flex items-center gap-2"><span class="w-3 h-3 rounded-full bg-amber-400"></span><span>Выбрано</span></div>
                    <div class="flex items-center gap-2"><span class="w-3 h-3 rounded-full bg-slate-600"></span><span>Занято</span></div>
                </div>

                <div id="slots-container" class="grid grid-cols-3 sm:grid-cols-4 gap-2.5"></div>
            </div>

            <div class="glass-panel rounded-3xl p-6 sm:p-7">
                <div class="mb-6">
                    <span class="text-[11px] font-bold uppercase tracking-[0.18em] text-amber-400">Шаг 02</span>
                    <h2 class="text-xl font-extrabold text-white mt-0.5">Регистрация клиента и талон</h2>
                    <p class="text-xs sm:text-sm text-slate-400 mt-0.5">Заявка сразу попадает в очередь и отправляется разработчику</p>
                </div>

                <form id="registration-form" class="space-y-4">
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                        <div>
                            <label for="input-name" class="block text-[11px] font-bold uppercase tracking-[0.12em] text-slate-400 mb-2">Имя клиента *</label>
                            <input type="text" id="input-name" required placeholder="Например: Тимур"
                                class="w-full px-4 py-3 rounded-xl bg-[#090c10] border border-white/[0.1] text-sm text-white placeholder-slate-600 focus:border-amber-400 focus:ring-2 focus:ring-amber-400/20 outline-none transition">
                        </div>
                        <div>
                            <label for="input-phone" class="block text-[11px] font-bold uppercase tracking-[0.12em] text-slate-400 mb-2">Телефон *</label>
                            <input type="tel" id="input-phone" required placeholder="+996 555 00-00-00"
                                class="w-full px-4 py-3 rounded-xl bg-[#090c10] border border-white/[0.1] text-sm text-white placeholder-slate-600 focus:border-amber-400 focus:ring-2 focus:ring-amber-400/20 outline-none transition">
                        </div>
                    </div>

                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                        <div>
                            <label for="input-car" class="block text-[11px] font-bold uppercase tracking-[0.12em] text-slate-400 mb-2">Марка и модель *</label>
                            <input type="text" id="input-car" required placeholder="Mercedes-Benz E-Class"
                                class="w-full px-4 py-3 rounded-xl bg-[#090c10] border border-white/[0.1] text-sm text-white placeholder-slate-600 focus:border-amber-400 focus:ring-2 focus:ring-amber-400/20 outline-none transition">
                        </div>
                        <div>
                            <label for="input-plate" class="block text-[11px] font-bold uppercase tracking-[0.12em] text-slate-400 mb-2">Государственный номер *</label>
                            <input type="text" id="input-plate" required placeholder="01 KG 001 VIP"
                                class="w-full px-4 py-3 rounded-xl bg-[#090c10] border border-white/[0.1] text-sm font-mono uppercase text-white placeholder-slate-600 focus:border-amber-400 focus:ring-2 focus:ring-amber-400/20 outline-none transition">
                        </div>
                    </div>

                    <div>
                        <label for="input-service" class="block text-[11px] font-bold uppercase tracking-[0.12em] text-slate-400 mb-2">Пакет обслуживания</label>
                        <select id="input-service" class="w-full px-4 py-3 rounded-xl bg-[#090c10] border border-white/[0.1] text-sm text-white focus:border-amber-400 focus:ring-2 focus:ring-amber-400/20 outline-none transition">
                            <option value="Premium Synthetic 5W-30 + оригинальный фильтр">Premium Synthetic 5W-30 + оригинальный фильтр</option>
                            <option value="Premium Synthetic 5W-40 + оригинальный фильтр">Premium Synthetic 5W-40 + оригинальный фильтр</option>
                            <option value="Ultra Low-Viscosity 0W-20 + фильтр">Ultra Low-Viscosity 0W-20 + фильтр</option>
                            <option value="LongLife 10W-40 + фильтр">LongLife 10W-40 + фильтр</option>
                            <option value="Полная замена масла в АКПП / DSG">Полная замена масла в АКПП / DSG</option>
                            <option value="Сервис с расходниками клиента">Сервис с расходниками клиента</option>
                        </select>
                    </div>

                    <div class="rounded-2xl bg-amber-400/[0.08] border border-amber-400/25 px-4 py-3.5 flex items-center justify-between gap-3">
                        <div class="text-xs sm:text-sm">
                            <span class="text-slate-400">Выбранный слот:</span>
                            <strong id="summary-slot-label" class="text-amber-300 ml-1.5">Не выбран</strong>
                        </div>
                        <span class="text-[10px] font-extrabold uppercase tracking-[0.15em] px-2.5 py-1 rounded-lg bg-amber-400/20 text-amber-300">
                            GARANT PASS
                        </span>
                    </div>

                    <button type="submit" id="submit-registration-btn" disabled
                        class="w-full py-3.5 px-6 rounded-xl text-sm font-extrabold uppercase tracking-wider bg-white/[0.06] text-slate-500 border border-white/[0.06] cursor-not-allowed transition">
                        Оформить талон
                    </button>
                </form>
            </div>
        </div>

        <div class="lg:col-span-5 space-y-6">
            <div id="dev-stream-card" class="hidden glass-panel rounded-3xl p-6 border-amber-400/35">
                <div class="flex items-center justify-between gap-2 mb-4 pb-3 border-b border-white/[0.08]">
                    <div>
                        <span class="text-[10px] font-extrabold uppercase tracking-[0.18em] text-amber-400">Поток разработчика</span>
                        <h3 class="text-base font-extrabold text-white mt-0.5">Входящие талоны клиентов</h3>
                    </div>
                    <button type="button" onclick="clearDeveloperStream()" class="text-xs font-semibold px-3 py-1.5 rounded-xl bg-white/[0.05] hover:bg-white/[0.1] text-slate-300 border border-white/[0.08] transition cursor-pointer">
                        Очистить
                    </button>
                </div>
                <div id="dev-stream-list" class="space-y-2.5 max-h-64 overflow-y-auto pr-1 text-xs">
                    <p class="text-slate-500 text-center py-4">Ожидание новых талонов...</p>
                </div>
            </div>

            <div class="glass-panel rounded-3xl p-6 sm:p-7">
                <div class="flex items-center justify-between gap-3 mb-5 pb-4 border-b border-white/[0.08]">
                    <div>
                        <span class="text-[10px] font-bold uppercase tracking-[0.18em] text-amber-400">Live Queue</span>
                        <h2 class="text-xl font-extrabold text-white mt-0.5">Очередь на <span id="board-date-title">сегодня</span></h2>
                    </div>
                    <div class="text-right">
                        <div id="board-ticket-counter" class="text-3xl font-extrabold text-amber-400 leading-none">0</div>
                        <div class="text-[11px] text-slate-400 mt-1">автомобилей</div>
                    </div>
                </div>
                <div id="board-tickets-list" class="space-y-3 max-h-[560px] overflow-y-auto pr-1">
                    <div class="text-center py-12 text-slate-500 text-sm">Загрузка талонов...</div>
                </div>
            </div>
        </div>
    </main>

    <footer class="border-t border-white/[0.06] py-5 text-center text-xs text-slate-500">
        © 2026 <button type="button" onclick="openDeveloperAuthModal()" class="font-bold text-slate-300 hover:text-amber-400 transition cursor-pointer">GARANT SERVICE</button> • Премиальная система электронной очереди
    </footer>

    <div id="toast-notification" class="fixed bottom-5 right-5 z-50 transform translate-y-24 opacity-0 transition-all duration-300 glass-panel rounded-2xl px-4 py-3.5 flex items-center gap-3 max-w-sm border-amber-400/25">
        <span id="toast-badge" class="text-amber-400 text-base font-bold">✦</span>
        <p id="toast-message-text" class="text-xs sm:text-sm font-medium text-white"></p>
    </div>

    <div id="dev-popup-alert" class="fixed top-20 right-5 z-50 hidden max-w-sm w-full rounded-2xl bg-[#12161f]/95 backdrop-blur-xl border border-amber-400/60 p-4 shadow-2xl gold-glow">
        <div class="flex items-start justify-between gap-2">
            <div class="flex items-center gap-2">
                <span class="px-2 py-0.5 rounded-md bg-amber-400 text-slate-950 text-[10px] font-extrabold uppercase tracking-wider">Новый талон</span>
                <span id="popup-slot-time" class="text-xs font-bold text-amber-300"></span>
            </div>
            <button type="button" onclick="closeDeveloperPopup()" class="text-slate-400 hover:text-white text-sm font-bold cursor-pointer">✕</button>
        </div>
        <div class="mt-2.5 space-y-1">
            <p id="popup-car-info" class="text-sm font-extrabold text-white"></p>
            <p id="popup-client-info" class="text-xs text-slate-300"></p>
            <p id="popup-service-info" class="text-xs text-amber-300/90"></p>
        </div>
    </div>

    <div id="dev-auth-modal" class="fixed inset-0 bg-black/80 backdrop-blur-md z-50 hidden items-center justify-center p-4">
        <div class="glass-panel rounded-3xl max-w-xs w-full p-6 border-amber-400/25">
            <span class="text-[10px] font-extrabold uppercase tracking-[0.18em] text-amber-400">Private Access</span>
            <h3 class="text-lg font-extrabold text-white mt-1">Вход разработчика</h3>
            <p class="text-xs text-slate-400 mt-1 mb-4">Введите код доступа</p>
            <input type="password" id="dev-code-input" maxlength="10" placeholder="••••" inputmode="numeric"
                class="w-full text-center text-2xl tracking-[0.35em] font-extrabold px-4 py-3 rounded-xl bg-[#080a0e] border border-white/[0.14] text-white focus:border-amber-400 focus:ring-2 focus:ring-amber-400/20 outline-none mb-5">
            <div class="flex justify-end gap-2.5">
                <button type="button" onclick="closeDeveloperAuthModal()" class="px-4 py-2 rounded-xl text-xs font-semibold text-slate-400 hover:text-white hover:bg-white/[0.06] transition cursor-pointer">Отмена</button>
                <button type="button" onclick="verifyDeveloperCode()" class="px-4 py-2 rounded-xl text-xs font-extrabold bg-amber-400 hover:bg-amber-300 text-slate-950 transition cursor-pointer">Войти</button>
            </div>
        </div>
    </div>

    <div id="cancel-confirm-modal" class="fixed inset-0 bg-black/80 backdrop-blur-md z-50 hidden items-center justify-center p-4">
        <div class="glass-panel rounded-3xl max-w-sm w-full p-6">
            <h3 class="text-lg font-extrabold text-white mb-2">Отменить талон?</h3>
            <p id="cancel-confirm-text" class="text-xs sm:text-sm text-slate-400 mb-6">Слот снова станет свободным.</p>
            <div class="flex justify-end gap-3">
                <button type="button" onclick="closeCancelConfirmModal()" class="px-4 py-2 rounded-xl text-xs font-semibold text-slate-300 hover:bg-white/[0.06] transition cursor-pointer">Оставить</button>
                <button type="button" id="execute-cancel-btn" class="px-4 py-2 rounded-xl text-xs font-bold bg-rose-600 hover:bg-rose-500 text-white transition cursor-pointer">Отменить талон</button>
            </div>
        </div>
    </div>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
        import { getAuth, signInAnonymously, signInWithCustomToken, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
        import { getFirestore, collection, doc, setDoc, deleteDoc, updateDoc, onSnapshot } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";

        const DEVELOPER_ACCESS_CODE = "7777";
        const SERVICE_SLOTS = [
            "09:00", "09:30", "10:00", "10:30", "11:00", "11:30",
            "12:00", "12:30", "13:00", "13:30", "14:00", "14:30",
            "15:00", "15:30", "16:00", "16:30", "17:00", "17:30",
            "18:00", "18:30", "19:00", "19:30"
        ];

        let activeUser = null;
        let currentDate = getTodayDateStr();
        let chosenSlot = null;
        let allTickets = [];
        let developerModeEnabled = false;
        let firstSnapshotLoaded = false;
        let knownIds = new Set();
        let incomingDeveloperQueue = [];
        let targetDeleteTicketId = null;
        let logoTapCount = 0;
        let logoTapResetTimer = null;

        // Храним отправленные напоминания (40 мин и 20 мин) для каждого талона клиента
        const sentClientReminders = new Set();

        const appId = typeof __app_id !== 'undefined' ? __app_id : 'garant-service-atelier';
        const firebaseConfig = typeof __firebase_config !== 'undefined'
            ? JSON.parse(__firebase_config)
            : {
                apiKey: "REPLACE_WITH_YOUR_API_KEY",
                authDomain: "REPLACE_WITH_PROJECT.firebaseapp.com",
                projectId: "REPLACE_WITH_PROJECT_ID",
                storageBucket: "REPLACE_WITH_PROJECT.appspot.com",
                messagingSenderId: "000000000000",
                appId: "1:000000000000:web:000000000000"
            };

        const firebaseApp = initializeApp(firebaseConfig);
        const auth = getAuth(firebaseApp);
        const db = getFirestore(firebaseApp);

        const bookingDateInput = document.getElementById('booking-date');
        const slotsContainer = document.getElementById('slots-container');
        const boardTicketsList = document.getElementById('board-tickets-list');
        const boardTicketCounter = document.getElementById('board-ticket-counter');
        const boardDateTitle = document.getElementById('board-date-title');
        const summarySlotLabel = document.getElementById('summary-slot-label');
        const submitRegistrationBtn = document.getElementById('submit-registration-btn');
        const registrationForm = document.getElementById('registration-form');

        bookingDateInput.value = currentDate;
        bookingDateInput.min = getTodayDateStr();
        updateBoardDateLabel();

        // Запрос разрешения на отправку уведомлений при входе в приложение
        async function requestNotificationPermissionOnEntry() {
            if (!("Notification" in window)) return;
            if (Notification.permission === "default") {
                try {
                    await Notification.requestPermission();
                } catch (err) {
                    console.warn("Запрос разрешения на уведомления отклонён или заблокирован:", err);
                }
            }
        }

        // Парсим дату и время слота в объект Date
        function parseSlotDateTime(dateStr, timeStr) {
            const [y, m, d] = dateStr.split('-').map(Number);
            const [hh, mm] = timeStr.split(':').map(Number);
            return new Date(y, m - 1, d, hh, mm, 0, 0);
        }

        // Отправка уведомления клиенту (системное уведомление браузера + тост-уведомление в приложении)
        function sendClientReminderAlert(title, message) {
            playChimeSound();
            showNotificationToast(message, "⏰");

            if ("Notification" in window && Notification.permission === "granted") {
                try {
                    new Notification(title, { body: message });
                } catch (err) {
                    console.warn("Ошибка показа системного уведомления:", err);
                }
            }
        }

        // Проверка талонов текущего клиента: напоминание за 40 минут и повторное за 20 минут
        function checkClientUpcomingReminders() {
            if (!activeUser || allTickets.length === 0) return;

            const now = new Date();
            const myTickets = allTickets.filter(t => t.userId === activeUser.uid && t.status !== 'done');

            myTickets.forEach((ticket) => {
                const slotDate = parseSlotDateTime(ticket.date, ticket.time);
                const diffMinutes = (slotDate.getTime() - now.getTime()) / 60000;

                // Напоминание за 40 минут до записи (окно от 39 до 40 минут)
                const key40 = `${ticket.id}_40m`;
                if (diffMinutes <= 40 && diffMinutes > 20 && !sentClientReminders.has(key40)) {
                    sentClientReminders.add(key40);
                    sendClientReminderAlert(
                        "GARANT SERVICE: Напоминание о записи",
                        `Через 40 минут (${ticket.time}) у вас сегодня запись на ${ticket.carModel} (${ticket.carPlate}).`
                    );
                }

                // Повторное напоминание за 20 минут до записи (окно до 20 минут)
                const key20 = `${ticket.id}_20m`;
                if (diffMinutes <= 20 && diffMinutes >= -15 && !sentClientReminders.has(key20)) {
                    sentClientReminders.add(key20);
                    sendClientReminderAlert(
                        "GARANT SERVICE: Осталось 20 минут!",
                        `У вас сегодня запись в ${ticket.time} (${ticket.carModel}) — вы можете опоздать, выезжайте в сервис.`
                    );
                }
            });
        }

        async function initializeService() {
            await requestNotificationPermissionOnEntry();
            try {
                if (typeof __initial_auth_token !== 'undefined' && __initial_auth_token) {
                    await signInWithCustomToken(auth, __initial_auth_token);
                } else {
                    await signInAnonymously(auth);
                }
            } catch (err) {
                console.error(err);
                document.getElementById('sync-status-text').textContent = "Нет связи";
                showNotificationToast("Проверьте подключение к базе данных", "⚠️");
            }
        }

        onAuthStateChanged(auth, (user) => {
            if (user) {
                activeUser = user;
                document.getElementById('sync-status-text').textContent = "Онлайн • Live";
                subscribeToTicketsStream();
            }
        });

        function subscribeToTicketsStream() {
            if (!activeUser) return;
            const ticketsRef = collection(db, 'artifacts', appId, 'public', 'data', 'garant_service_atelier_tickets');

            onSnapshot(ticketsRef, (snapshot) => {
                const list = [];
                const freshTickets = [];

                snapshot.forEach((docSnap) => {
                    const ticket = { id: docSnap.id, ...docSnap.data() };
                    list.push(ticket);
                    if (firstSnapshotLoaded && !knownIds.has(docSnap.id)) {
                        freshTickets.push(ticket);
                    }
                    knownIds.add(docSnap.id);
                });

                if (firstSnapshotLoaded && freshTickets.length > 0) {
                    freshTickets.forEach((ticket) => {
                        incomingDeveloperQueue.unshift(ticket);
                        if (developerModeEnabled) {
                            renderDeveloperStream();
                            notifyDeveloper(ticket);
                        }
                    });
                    refreshDeveloperCounters();
                }

                firstSnapshotLoaded = true;
                allTickets = list;
                refreshDeveloperCounters();
                renderSlotGrid();
                renderTicketBoard();
                checkClientUpcomingReminders();
            }, (err) => {
                console.error(err);
                showNotificationToast("Не удалось обновить очередь", "⚠️");
            });
        }

        function renderSlotGrid() {
            slotsContainer.innerHTML = '';
            const dayTickets = allTickets.filter(t => t.date === currentDate);
            const bookedMap = new Map(dayTickets.map(t => [t.time, t]));

            const now = new Date();
            const isToday = currentDate === getTodayDateStr();
            const nowMins = now.getHours() * 60 + now.getMinutes();

            SERVICE_SLOTS.forEach((slot) => {
                const booked = bookedMap.get(slot);
                const [h, m] = slot.split(':').map(Number);
                const slotMins = h * 60 + m;
                const isPast = isToday && slotMins < nowMins;

                const btn = document.createElement('button');
                btn.type = 'button';

                if (booked) {
                    const isMine = activeUser && booked.userId === activeUser.uid;
                    btn.disabled = true;
                    btn.className = isMine
                        ? "py-2.5 px-2 rounded-xl text-xs sm:text-sm font-bold bg-sky-500/15 text-sky-300 border border-sky-400/40 cursor-not-allowed flex flex-col items-center"
                        : "py-2.5 px-2 rounded-xl text-xs sm:text-sm font-medium bg-white/[0.02] text-slate-600 border border-white/[0.05] cursor-not-allowed flex flex-col items-center";
                    btn.innerHTML = `<span>${slot}</span><span class="text-[10px] font-semibold uppercase mt-0.5">${isMine ? 'Ваш талон' : 'Занято'}</span>`;
                } else if (isPast) {
                    btn.disabled = true;
                    btn.className = "py-2.5 px-2 rounded-xl text-xs sm:text-sm font-medium bg-white/[0.01] text-slate-700 border border-white/[0.04] cursor-not-allowed flex flex-col items-center";
                    btn.innerHTML = `<span>${slot}</span><span class="text-[10px] mt-0.5">Прошло</span>`;
                } else {
                    const isSelected = chosenSlot === slot;
                    btn.className = isSelected
                        ? "py-2.5 px-2 rounded-xl text-xs sm:text-sm font-extrabold bg-amber-400 text-slate-950 border border-amber-300 gold-glow transition flex flex-col items-center cursor-pointer"
                        : "py-2.5 px-2 rounded-xl text-xs sm:text-sm font-semibold bg-emerald-400/[0.08] hover:bg-emerald-400/[0.15] text-emerald-300 border border-emerald-400/25 transition flex flex-col items-center cursor-pointer";
                    btn.innerHTML = `<span>${slot}</span><span class="text-[10px] ${isSelected ? 'text-slate-950 font-bold' : 'text-emerald-400/80'} mt-0.5">Свободно</span>`;
                    btn.onclick = () => selectSlot(slot);
                }

                slotsContainer.appendChild(btn);
            });

            if (chosenSlot && bookedMap.has(chosenSlot)) {
                chosenSlot = null;
                updateSubmitButtonState();
                showNotificationToast("Выбранное время только что заняли", "⚠️");
            }
        }

        function renderTicketBoard() {
            const dayTickets = allTickets
                .filter(t => t.date === currentDate)
                .sort((a, b) => a.time.localeCompare(b.time));

            boardTicketCounter.textContent = dayTickets.length;

            if (dayTickets.length === 0) {
                boardTicketsList.innerHTML = `
                    <div class="text-center py-12 px-4 rounded-2xl border border-dashed border-white/[0.1]">
                        <p class="text-slate-300 font-semibold text-sm">На выбранную дату записей нет</p>
                        <p class="text-xs text-slate-500 mt-1">Выберите свободный слот слева, чтобы забронировать время</p>
                    </div>
                `;
                return;
            }

            boardTicketsList.innerHTML = '';
            dayTickets.forEach((ticket, idx) => {
                const isMine = activeUser && ticket.userId === activeUser.uid;
                const canDelete = isMine || developerModeEnabled;
                const status = ticket.status || 'waiting';

                let statusBadge = `<span class="text-[10px] font-bold uppercase tracking-wider px-2.5 py-1 rounded-lg bg-amber-400/15 text-amber-300 border border-amber-400/30">В очереди</span>`;
                if (status === 'in_progress') {
                    statusBadge = `<span class="text-[10px] font-bold uppercase tracking-wider px-2.5 py-1 rounded-lg bg-emerald-400/15 text-emerald-300 border border-emerald-400/35">В работе</span>`;
                } else if (status === 'done') {
                    statusBadge = `<span class="text-[10px] font-bold uppercase tracking-wider px-2.5 py-1 rounded-lg bg-white/[0.06] text-slate-400 border border-white/[0.08]">Готово</span>`;
                }

                const visiblePhone = (isMine || developerModeEnabled) ? ticket.phone : maskPhone(ticket.phone);

                const card = document.createElement('div');
                card.className = `p-4 rounded-2xl border transition ${
                    isMine
                        ? 'bg-amber-400/[0.06] border-amber-400/45'
                        : 'bg-white/[0.025] border-white/[0.07]'
                }`;

                card.innerHTML = `
                    <div class="flex items-start justify-between gap-3">
                        <div class="flex items-center gap-3">
                            <div class="px-3 py-2 rounded-xl bg-amber-400 text-slate-950 font-extrabold text-sm">
                                ${escapeHtml(ticket.time)}
                            </div>
                            <div>
                                <div class="flex items-center gap-2 flex-wrap">
                                    <span class="font-bold text-white text-sm">${escapeHtml(ticket.carModel)}</span>
                                    ${isMine ? '<span class="text-[10px] font-extrabold uppercase tracking-wider px-2 py-0.5 rounded bg-amber-400/20 text-amber-300">Ваш талон</span>' : ''}
                                </div>
                                <div class="mt-1 inline-block text-xs font-mono text-slate-300 bg-black/50 px-2.5 py-0.5 rounded-lg border border-white/[0.08]">
                                    ${escapeHtml(ticket.carPlate)}
                                </div>
                            </div>
                        </div>
                        <div class="flex flex-col items-end gap-1.5">
                            ${statusBadge}
                            <span class="text-[11px] text-slate-500 font-semibold">#${idx + 1}</span>
                        </div>
                    </div>

                    <div class="mt-3.5 pt-3 border-t border-white/[0.07] flex flex-wrap items-center justify-between gap-2 text-xs text-slate-400">
                        <div>
                            <span class="text-slate-200 font-semibold">${escapeHtml(ticket.clientName)}</span>
                            <span class="mx-1.5 text-slate-600">•</span>
                            <span>${escapeHtml(visiblePhone)}</span>
                            <div class="text-[11px] text-slate-400 mt-1">${escapeHtml(ticket.serviceType)}</div>
                        </div>
                        <div class="flex items-center gap-2">
                            ${developerModeEnabled ? `
                                <button type="button" onclick="changeTicketStatus('${ticket.id}', '${status}')" class="px-3 py-1.5 rounded-xl bg-indigo-500/20 hover:bg-indigo-500/35 text-indigo-200 border border-indigo-400/30 font-semibold transition cursor-pointer">
                                    Статус
                                </button>
                            ` : ''}
                            ${canDelete ? `
                                <button type="button" onclick="askCancelTicket('${ticket.id}', '${escapeHtml(ticket.time)}')" class="px-3 py-1.5 rounded-xl bg-rose-500/15 hover:bg-rose-500/30 text-rose-300 border border-rose-400/30 font-semibold transition cursor-pointer">
                                    Отменить
                                </button>
                            ` : ''}
                        </div>
                    </div>
                `;
                boardTicketsList.appendChild(card);
            });
        }

        function selectSlot(slot) {
            chosenSlot = slot;
            renderSlotGrid();
            updateSubmitButtonState();
        }

        function updateSubmitButtonState() {
            if (chosenSlot) {
                summarySlotLabel.textContent = `${formatDateDisplay(currentDate)} в ${chosenSlot}`;
                submitRegistrationBtn.disabled = false;
                submitRegistrationBtn.className = "w-full py-3.5 px-6 rounded-xl text-sm font-extrabold uppercase tracking-wider bg-amber-400 hover:bg-amber-300 text-slate-950 gold-glow transition cursor-pointer";
            } else {
                summarySlotLabel.textContent = "Не выбран";
                submitRegistrationBtn.disabled = true;
                submitRegistrationBtn.className = "w-full py-3.5 px-6 rounded-xl text-sm font-extrabold uppercase tracking-wider bg-white/[0.06] text-slate-500 border border-white/[0.06] cursor-not-allowed transition";
            }
        }

        registrationForm.addEventListener('submit', async (e) => {
            e.preventDefault();
            if (!chosenSlot) {
                showNotificationToast("Сначала выберите свободный слот", "⚠️");
                return;
            }
            if (!activeUser) {
                showNotificationToast("Подождите подключения к сервису...", "⏳");
                return;
            }

            await requestNotificationPermissionOnEntry();

            const alreadyTaken = allTickets.some(t => t.date === currentDate && t.time === chosenSlot);
            if (alreadyTaken) {
                showNotificationToast("Это время уже забронировано", "⚠️");
                renderSlotGrid();
                return;
            }

            const clientName = document.getElementById('input-name').value.trim();
            const phone = document.getElementById('input-phone').value.trim();
            const carModel = document.getElementById('input-car').value.trim();
            const carPlate = document.getElementById('input-plate').value.trim().toUpperCase();
            const serviceType = document.getElementById('input-service').value;

            const docId = `${currentDate}_${chosenSlot.replace(':', '')}`;
            const payload = {
                date: currentDate,
                time: chosenSlot,
                clientName,
                phone,
                carModel,
                carPlate,
                serviceType,
                status: 'waiting',
                userId: activeUser.uid,
                createdAt: new Date().toISOString()
            };

            try {
                submitRegistrationBtn.disabled = true;
                submitRegistrationBtn.textContent = "Создание талона...";

                const docRef = doc(db, 'artifacts', appId, 'public', 'data', 'garant_service_atelier_tickets', docId);
                await setDoc(docRef, payload);

                knownIds.add(docId);

                if (developerModeEnabled) {
                    const entry = { id: docId, ...payload };
                    incomingDeveloperQueue.unshift(entry);
                    refreshDeveloperCounters();
                    renderDeveloperStream();
                    notifyDeveloper(entry);
                }

                showNotificationToast(`Талон на ${chosenSlot} оформлен • Напомним за 40 и 20 мин`, "✦");
                registrationForm.reset();
                chosenSlot = null;
                updateSubmitButtonState();
            } catch (err) {
                console.error(err);
                showNotificationToast("Не удалось оформить талон", "⚠️");
            } finally {
                submitRegistrationBtn.textContent = "Оформить талон";
                updateSubmitButtonState();
            }
        });

        // Каждые 30 секунд проверяем время до записи клиента (за 40 и за 20 минут)
        setInterval(checkClientUpcomingReminders, 30000);

        bookingDateInput.addEventListener('change', (e) => {
            if (!e.target.value) return;
            currentDate = e.target.value;
            chosenSlot = null;
            updateSubmitButtonState();
            updateBoardDateLabel();
            renderSlotGrid();
            renderTicketBoard();
        });

        window.changeDay = (deltaDays) => {
            const base = new Date(currentDate + "T00:00:00");
            base.setDate(base.getDate() + deltaDays);
            const offset = base.getTimezoneOffset() * 60000;
            const nextStr = new Date(base.getTime() - offset).toISOString().split('T')[0];
            if (nextStr < getTodayDateStr()) return;

            currentDate = nextStr;
            bookingDateInput.value = currentDate;
            chosenSlot = null;
            updateSubmitButtonState();
            updateBoardDateLabel();
            renderSlotGrid();
            renderTicketBoard();
        };

        window.handleSecretLogoTap = () => {
            if (developerModeEnabled) return;
            logoTapCount += 1;
            clearTimeout(logoTapResetTimer);
            logoTapResetTimer = setTimeout(() => { logoTapCount = 0; }, 1500);
            if (logoTapCount >= 5) {
                logoTapCount = 0;
                openDeveloperAuthModal();
            }
        };

        window.openDeveloperAuthModal = () => {
            if (developerModeEnabled) return;
            const modal = document.getElementById('dev-auth-modal');
            const input = document.getElementById('dev-code-input');
            input.value = '';
            modal.classList.remove('hidden');
            modal.classList.add('flex');
            setTimeout(() => input.focus(), 80);
        };

        window.closeDeveloperAuthModal = () => {
            const modal = document.getElementById('dev-auth-modal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        };

        window.verifyDeveloperCode = () => {
            const enteredCode = document.getElementById('dev-code-input').value.trim();
            if (enteredCode === DEVELOPER_ACCESS_CODE) {
                developerModeEnabled = true;
                closeDeveloperAuthModal();
                document.getElementById('developer-console').classList.remove('hidden');
                document.getElementById('dev-stream-card').classList.remove('hidden');
                document.getElementById('dev-logout-btn').classList.remove('hidden');
                refreshDeveloperCounters();
                renderDeveloperStream();
                renderTicketBoard();
                playChimeSound();
                showNotificationToast("Режим разработчика активирован", "✦");
            } else {
                showNotificationToast("Неверный код доступа", "❌");
            }
        };

        window.logoutDeveloperMode = () => {
            developerModeEnabled = false;
            document.getElementById('developer-console').classList.add('hidden');
            document.getElementById('dev-stream-card').classList.add('hidden');
            document.getElementById('dev-logout-btn').classList.add('hidden');
            closeDeveloperPopup();
            renderTicketBoard();
            showNotificationToast("Режим разработчика закрыт", "✦");
        };

        document.getElementById('dev-code-input').addEventListener('keydown', (e) => {
            if (e.key === 'Enter') verifyDeveloperCode();
        });

        function playChimeSound() {
            try {
                const AudioCtx = window.AudioContext || window.webkitAudioContext;
                const ctx = new AudioCtx();
                const osc = ctx.createOscillator();
                const gain = ctx.createGain();
                osc.type = 'sine';
                osc.frequency.setValueAtTime(1046.5, ctx.currentTime);
                osc.frequency.setValueAtTime(1318.5, ctx.currentTime + 0.12);
                gain.gain.setValueAtTime(0.2, ctx.currentTime);
                gain.gain.exponentialRampToValueAtTime(0.001, ctx.currentTime + 0.45);
                osc.connect(gain);
                gain.connect(ctx.destination);
                osc.start();
                osc.stop(ctx.currentTime + 0.45);
            } catch (err) {
                console.warn(err);
            }
        }

        window.activateDeveloperAlerts = async () => {
            playChimeSound();
            if (!("Notification" in window)) {
                showNotificationToast("Звуковые уведомления включены", "🔔");
                return;
            }
            const perm = await Notification.requestPermission();
            if (perm === "granted") {
                document.getElementById('dev-sound-btn').textContent = "🔔 Уведомления активны";
                showNotificationToast("Звук и системные уведомления включены", "✅");
            } else {
                showNotificationToast("Включён звуковой сигнал в приложении", "🔔");
            }
        };

        window.triggerSampleDeveloperAlert = () => {
            const sample = {
                date: currentDate,
                time: "16:00",
                clientName: "Данияр",
                phone: "+996 777 44-55-66",
                carModel: "Porsche Cayenne",
                carPlate: "01 KG 999 GAR",
                serviceType: "Premium Synthetic 5W-40 + оригинальный фильтр"
            };
            incomingDeveloperQueue.unshift(sample);
            refreshDeveloperCounters();
            renderDeveloperStream();
            notifyDeveloper(sample);
        };

        function notifyDeveloper(ticket) {
            playChimeSound();
            const popup = document.getElementById('dev-popup-alert');
            document.getElementById('popup-slot-time').textContent = `${formatDateDisplay(ticket.date)} • ${ticket.time}`;
            document.getElementById('popup-car-info').textContent = `${ticket.carModel} (${ticket.carPlate})`;
            document.getElementById('popup-client-info').textContent = `${ticket.clientName} • ${ticket.phone}`;
            document.getElementById('popup-service-info').textContent = ticket.serviceType;
            popup.classList.remove('hidden');

            if ("Notification" in window && Notification.permission === "granted") {
                new Notification(`GARANT SERVICE: Талон на ${ticket.time}`, {
                    body: `${ticket.carModel} (${ticket.carPlate}) — ${ticket.clientName}, ${ticket.phone}`
                });
            }
        }

        window.closeDeveloperPopup = () => {
            document.getElementById('dev-popup-alert').classList.add('hidden');
        };

        function refreshDeveloperCounters() {
            document.getElementById('dev-metric-total').textContent = allTickets.length;
            document.getElementById('dev-metric-new').textContent = incomingDeveloperQueue.length;
        }

        function renderDeveloperStream() {
            const streamEl = document.getElementById('dev-stream-list');
            if (incomingDeveloperQueue.length === 0) {
                streamEl.innerHTML = `<p class="text-slate-500 text-center py-4">Ожидание новых талонов...</p>`;
                return;
            }
            streamEl.innerHTML = incomingDeveloperQueue.slice(0, 10).map((t) => `
                <div class="p-3 rounded-2xl bg-white/[0.03] border border-amber-400/20">
                    <div class="flex items-center justify-between font-bold text-amber-300">
                        <span>${escapeHtml(formatDateDisplay(t.date))} в ${escapeHtml(t.time)}</span>
                        <span class="font-mono">${escapeHtml(t.carPlate)}</span>
                    </div>
                    <div class="text-white font-semibold mt-1">${escapeHtml(t.carModel)} — ${escapeHtml(t.clientName)}</div>
                    <div class="text-slate-400 mt-0.5">${escapeHtml(t.phone)} • ${escapeHtml(t.serviceType)}</div>
                </div>
            `).join('');
        }

        window.clearDeveloperStream = () => {
            incomingDeveloperQueue = [];
            refreshDeveloperCounters();
            renderDeveloperStream();
        };

        window.changeTicketStatus = async (ticketId, currentStatus) => {
            if (!activeUser || !developerModeEnabled) return;
            const cycle = { waiting: 'in_progress', in_progress: 'done', done: 'waiting' };
            const nextStatus = cycle[currentStatus] || 'waiting';
            try {
                const docRef = doc(db, 'artifacts', appId, 'public', 'data', 'garant_service_atelier_tickets', ticketId);
                await updateDoc(docRef, { status: nextStatus });
                showNotificationToast("Статус талона обновлён", "✦");
            } catch (err) {
                console.error(err);
                showNotificationToast("Не удалось сменить статус", "⚠️");
            }
        };

        window.askCancelTicket = (ticketId, slotTime) => {
            targetDeleteTicketId = ticketId;
            document.getElementById('cancel-confirm-text').textContent = `Освободить слот ${slotTime} в очереди GARANT SERVICE?`;
            const modal = document.getElementById('cancel-confirm-modal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        };

        window.closeCancelConfirmModal = () => {
            targetDeleteTicketId = null;
            const modal = document.getElementById('cancel-confirm-modal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        };

        document.getElementById('execute-cancel-btn').addEventListener('click', async () => {
            if (!targetDeleteTicketId || !activeUser) return;
            try {
                const docRef = doc(db, 'artifacts', appId, 'public', 'data', 'garant_service_atelier_tickets', targetDeleteTicketId);
                await deleteDoc(docRef);
                showNotificationToast("Талон отменён", "✦");
            } catch (err) {
                console.error(err);
                showNotificationToast("Не удалось отменить талон", "⚠️");
            } finally {
                closeCancelConfirmModal();
            }
        });

        function getTodayDateStr() {
            const now = new Date();
            const offset = now.getTimezoneOffset() * 60000;
            return new Date(now.getTime() - offset).toISOString().split('T')[0];
        }

        function formatDateDisplay(iso) {
            const [y, m, d] = iso.split('-');
            return `${d}.${m}.${y}`;
        }

        function updateBoardDateLabel() {
            boardDateTitle.textContent = currentDate === getTodayDateStr() ? "сегодня" : formatDateDisplay(currentDate);
        }

        function maskPhone(phone) {
            if (!phone || phone.length < 5) return "***";
            return phone.slice(0, 4) + " *** ** " + phone.slice(-2);
        }

        function escapeHtml(value) {
            if (!value) return '';
            return String(value).replace(/[&<>"']/g, (ch) => ({
                '&': '&amp;', '<': '&lt;', '>': '&gt;', '"': '&quot;', "'": '&#39;'
            }[ch]));
        }

        let toastTimer;
        function showNotificationToast(message, badge = "✦") {
            const box = document.getElementById('toast-notification');
            document.getElementById('toast-message-text').textContent = message;
            document.getElementById('toast-badge').textContent = badge;
            box.classList.remove('translate-y-24', 'opacity-0');
            clearTimeout(toastTimer);
            toastTimer = setTimeout(() => {
                box.classList.add('translate-y-24', 'opacity-0');
            }, 3400);
        }

        initializeService();
    </script>
</body>
</html>
