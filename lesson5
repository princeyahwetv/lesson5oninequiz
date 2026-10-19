<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GAME-ON Action Research Assessment Portal</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts: Inter & Outfit -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Outfit:wght@600;700;800&display=swap" rel="stylesheet">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        mono: {
                            50: '#f9fafb',
                            100: '#f3f4f6',
                            200: '#e5e7eb',
                            300: '#d1d5db',
                            400: '#9ca3af',
                            500: '#6b7280',
                            600: '#4b5563',
                            700: '#374151',
                            800: '#1f2937',
                            900: '#111827',
                            950: '#030712'
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        display: ['Outfit', 'sans-serif']
                    }
                }
            }
        }
    </script>

    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f3f4f6;
            color: #111827;
            min-height: 100vh;
        }

        /* Printable area styles */
        @media print {
            body * {
                visibility: hidden;
            }
            #print-area, #print-area * {
                visibility: visible;
            }
            #print-area {
                position: absolute;
                left: 0;
                top: 0;
                width: 100%;
            }
            .no-print {
                display: none !important;
            }
        }

        .custom-radio:checked + label {
            border-color: #111827;
            background-color: #f9fafb;
            box-shadow: 0 0 0 2px #111827;
        }

        .badge-glow {
            animation: subtlePulse 2.5s infinite ease-in-out;
        }

        @keyframes subtlePulse {
            0%, 100% { transform: scale(1); filter: drop-shadow(0 4px 6px rgba(0, 0, 0, 0.1)); }
            50% { transform: scale(1.03); filter: drop-shadow(0 10px 15px rgba(0, 0, 0, 0.15)); }
        }
    </style>
</head>
<body class="flex flex-col min-h-screen justify-between p-3 sm:p-6 md:p-8 bg-gray-100">

    <!-- HEADER -->
    <header class="w-full max-w-4xl mx-auto mb-6 text-center no-print">
        <div class="bg-white p-6 sm:p-8 rounded-2xl border border-gray-200 shadow-sm relative overflow-hidden">
            <div class="absolute top-0 left-0 w-full h-1.5 bg-gray-900"></div>
            
            <div class="inline-block px-3 py-1 mb-3 rounded-full bg-gray-100 border border-gray-300 text-gray-700 text-xs font-semibold tracking-wider uppercase">
                Interactive Assessment Portal
            </div>
            
            <h1 class="font-display text-xl sm:text-2xl md:text-3xl font-extrabold text-gray-900 tracking-tight uppercase">
                GAME-ON ACTION RESEARCH PROPOSAL OF JOEL P. RODRIGUEZ LPT MAVED
            </h1>
            
            <div class="mt-2 flex items-center justify-center space-x-2 text-xs sm:text-sm font-medium text-gray-600">
                <span>Subject: Empowerment Technologies / ICT</span>
                <span>•</span>
                <span>Topic: Applying Hyperlinks and Custom Animations in Microsoft PowerPoint (Module 5)</span>
            </div>
        </div>
    </header>

    <!-- MAIN CONTAINER -->
    <main class="w-full max-w-4xl mx-auto flex-grow flex flex-col justify-center">

        <!-- SCREEN 1: REGISTRATION & LEADERBOARD -->
        <div id="start-screen" class="w-full grid grid-cols-1 lg:grid-cols-3 gap-6 transition-all duration-300">
            
            <!-- REGISTRATION FORM -->
            <div class="lg:col-span-2 bg-white p-6 sm:p-8 rounded-2xl border border-gray-200 shadow-sm flex flex-col justify-between">
                <div>
                    <div class="text-center sm:text-left mb-6">
                        <div class="inline-flex items-center justify-center w-12 h-12 rounded-xl bg-gray-100 text-gray-900 mb-3 border border-gray-300">
                            <i class="fa-solid fa-id-card text-xl"></i>
                        </div>
                        <h2 class="font-display text-2xl font-bold text-gray-900">Student Registration</h2>
                        <p class="text-gray-500 text-sm mt-1">Provide your credentials to begin the evaluation and record your score online.</p>
                    </div>

                    <form id="registration-form" onsubmit="event.preventDefault(); startQuiz();" class="space-y-4">
                        <div>
                            <label class="block text-xs font-bold uppercase tracking-wider text-gray-700 mb-1">
                                <i class="fa-solid fa-user text-gray-500 mr-2"></i>Full Name (Student)
                            </label>
                            <input type="text" id="student-name" placeholder="Enter full name" required
                                class="w-full px-4 py-3 bg-gray-50 border border-gray-300 rounded-xl text-gray-900 placeholder-gray-400 focus:outline-none focus:border-gray-900 focus:bg-white focus:ring-1 focus:ring-gray-900 transition-all text-sm font-medium"
                                oninput="validateForm()">
                        </div>

                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                            <div>
                                <label class="block text-xs font-bold uppercase tracking-wider text-gray-700 mb-1">
                                    <i class="fa-solid fa-graduation-cap text-gray-500 mr-2"></i>Grade Level
                                </label>
                                <select id="student-grade" required onchange="validateForm()"
                                    class="w-full px-4 py-3 bg-gray-50 border border-gray-300 rounded-xl text-gray-900 focus:outline-none focus:border-gray-900 focus:bg-white focus:ring-1 focus:ring-gray-900 transition-all text-sm font-medium">
                                    <option value="" disabled selected>Select Grade</option>
                                    <option value="Grade 11">Grade 11</option>
                                    <option value="Grade 12">Grade 12</option>
                                </select>
                            </div>
                            <div>
                                <label class="block text-xs font-bold uppercase tracking-wider text-gray-700 mb-1">
                                    <i class="fa-solid fa-users text-gray-500 mr-2"></i>Section
                                </label>
                                <input type="text" id="student-section" placeholder="e.g. St. Thomas" required
                                    class="w-full px-4 py-3 bg-gray-50 border border-gray-300 rounded-xl text-gray-900 placeholder-gray-400 focus:outline-none focus:border-gray-900 focus:bg-white focus:ring-1 focus:ring-gray-900 transition-all text-sm font-medium"
                                    oninput="validateForm()">
                            </div>
                        </div>

                        <!-- RULES SUMMARY BOX -->
                        <div class="bg-gray-50 p-4 rounded-xl border border-gray-200 text-xs text-gray-600 space-y-2 mt-4">
                            <div class="font-bold text-gray-800 uppercase tracking-wider flex items-center">
                                <i class="fa-solid fa-circle-info text-gray-700 mr-2"></i> Assessment Guidelines:
                            </div>
                            <ul class="list-disc list-inside space-y-1">
                                <li><strong>10 Multiple Choice Questions</strong> on MS PowerPoint interactive features.</li>
                                <li>Timer: <strong>10 Minutes (600 seconds)</strong> total time limit.</li>
                                <li>Question & option orders are <strong>randomized</strong>.</li>
                                <li>Passing score to earn the <strong>50 POINTS BADGE</strong>: <strong>10/10 (100% Perfect Score)</strong>.</li>
                            </ul>
                        </div>

                        <button type="submit" id="start-btn" disabled
                            class="w-full py-3.5 bg-gray-900 hover:bg-black disabled:opacity-40 disabled:cursor-not-allowed font-display font-bold text-white rounded-xl shadow-sm transition-all flex items-center justify-center space-x-2 text-sm mt-4">
                            <span>START ONLINE ASSESSMENT</span>
                            <i class="fa-solid fa-arrow-right"></i>
                        </button>
                    </form>
                </div>

                <div class="mt-6 pt-4 border-t border-gray-200 flex justify-between items-center text-xs text-gray-500">
                    <span id="sync-status"><i class="fa-solid fa-cloud text-gray-400 mr-1"></i> Syncing database...</span>
                    <button onclick="toggleTeacherPortal()" class="underline font-semibold hover:text-gray-900">
                        Teacher Dashboard
                    </button>
                </div>
            </div>

            <!-- TOP 3 LEADERBOARD -->
            <div class="bg-white p-6 rounded-2xl border border-gray-200 shadow-sm flex flex-col justify-between">
                <div>
                    <div class="flex items-center space-x-2 border-b border-gray-200 pb-3 mb-4">
                        <i class="fa-solid fa-trophy text-gray-900 text-lg"></i>
                        <h3 class="font-display font-bold text-lg text-gray-900">All Student Rankings</h3>
                    </div>

                    <p class="text-xs text-gray-500 mb-4">Live rankings of all submitted students, sorted by score and completion speed.</p>

                    <div id="top-3-container" class="space-y-3">
                        <div class="text-center py-8 text-xs text-gray-400">Loading top records...</div>
                    </div>
                </div>

                <div class="mt-4 pt-3 border-t border-gray-200 text-center">
                    <span class="text-[11px] text-gray-400"><i class="fa-solid fa-arrows-rotate mr-1"></i> Live online synchronization</span>
                </div>
            </div>
        </div>

        <!-- SCREEN 2: QUIZ INTERFACE -->
        <div id="quiz-screen" class="w-full max-w-3xl mx-auto bg-white p-6 sm:p-8 rounded-2xl border border-gray-200 shadow-sm hidden transition-all duration-300">
            <!-- TIMER & PROGRESS BAR TOP DOCK -->
            <div class="flex flex-col sm:flex-row items-center justify-between gap-4 mb-6 pb-4 border-b border-gray-200">
                <!-- Question Tracker -->
                <div class="flex items-center space-x-2">
                    <span class="text-xs font-bold text-gray-500 uppercase tracking-wider">Question</span>
                    <span id="question-tracker" class="px-3 py-1 bg-gray-100 text-gray-900 font-display font-bold text-xs rounded-lg border border-gray-300">
                        1 / 10
                    </span>
                </div>

                <!-- Countdown Timer -->
                <div class="flex items-center space-x-2 bg-gray-100 px-4 py-2 rounded-xl border border-gray-300">
                    <i class="fa-solid fa-stopwatch text-gray-700"></i>
                    <span class="text-xs text-gray-500 uppercase font-bold tracking-wider">Time Left:</span>
                    <span id="timer-display" class="font-display font-bold text-base text-gray-900">10:00</span>
                </div>
            </div>

            <!-- Progress Bar -->
            <div class="w-full bg-gray-100 h-2 rounded-full overflow-hidden mb-6 border border-gray-200">
                <div id="progress-bar" class="bg-gray-900 h-full w-0 transition-all duration-300"></div>
            </div>

            <!-- Question Card -->
            <div class="mb-6">
                <h3 id="question-text" class="text-base sm:text-lg font-semibold text-gray-900 leading-relaxed mb-6">
                    Loading question...
                </h3>

                <!-- Choices Container -->
                <div id="choices-container" class="space-y-3">
                    <!-- Dynamic Choices Insertion -->
                </div>
            </div>

            <!-- Navigation Bar -->
            <div class="flex items-center justify-between pt-4 border-t border-gray-200">
                <button id="prev-btn" onclick="previousQuestion()" class="px-4 py-2.5 bg-gray-100 hover:bg-gray-200 text-gray-700 rounded-xl font-semibold text-xs sm:text-sm transition-all flex items-center space-x-2 disabled:opacity-30 disabled:cursor-not-allowed border border-gray-300">
                    <i class="fa-solid fa-arrow-left"></i>
                    <span>Previous</span>
                </button>

                <button id="next-btn" onclick="nextQuestion()" class="px-6 py-2.5 bg-gray-900 hover:bg-black text-white font-bold rounded-xl text-xs sm:text-sm transition-all shadow-sm flex items-center space-x-2">
                    <span id="next-btn-text">Next</span>
                    <i id="next-btn-icon" class="fa-solid fa-arrow-right"></i>
                </button>
            </div>
        </div>

        <!-- SCREEN 3: RESULTS & BADGE & PRINT CERTIFICATE -->
        <div id="result-screen" class="w-full max-w-2xl mx-auto bg-white p-6 sm:p-10 rounded-2xl border border-gray-200 shadow-sm text-center hidden transition-all duration-300">
            
            <div id="print-area">
                <!-- BADGE ALERT HEADER (Displayed if Perfect Score 10/10) -->
                <div id="badge-container" class="hidden mb-6">
                    <div class="relative inline-block my-2">
                        <div class="w-28 h-28 sm:w-36 sm:h-36 bg-gray-900 rounded-full flex items-center justify-center p-1 badge-glow mx-auto border-4 border-gray-300 shadow-xl">
                            <div class="w-full h-full bg-white rounded-full flex flex-col items-center justify-center p-2 border border-gray-300">
                                <i class="fa-solid fa-award text-3xl sm:text-4xl text-gray-900 mb-1"></i>
                                <span class="font-display text-[10px] sm:text-xs font-black text-gray-600 tracking-wider uppercase">PERFECT</span>
                                <span class="font-display text-sm sm:text-base font-black text-gray-900">50 POINTS</span>
                            </div>
                        </div>
                    </div>
                    <div class="inline-block bg-gray-100 text-gray-900 border border-gray-300 px-3 py-1 rounded-full text-xs font-bold uppercase tracking-wider mb-2">
                        🏆 Official Recognition
                    </div>
                    <h2 class="font-display text-2xl font-black text-gray-900">50 POINTS BADGE EARNED</h2>
                    <p class="text-xs sm:text-sm text-gray-500 mt-1 max-w-md mx-auto">Mastery demonstrated! You achieved a perfect passing score of 10 out of 10.</p>
                </div>

                <!-- STANDARD RESULT HEADER (If score < 10) -->
                <div id="standard-result-header" class="mb-6">
                    <div class="inline-flex items-center justify-center w-14 h-14 rounded-full bg-gray-100 text-gray-800 border border-gray-300 mb-3">
                        <i class="fa-solid fa-clipboard-check text-2xl"></i>
                    </div>
                    <h2 class="font-display text-2xl font-bold text-gray-900">Assessment Complete</h2>
                    <p class="text-sm text-gray-500">Summary of your Empowerment Technologies test results.</p>
                </div>

                <!-- SUMMARY CARD -->
                <div class="bg-gray-50 rounded-xl p-5 sm:p-6 border border-gray-200 text-left max-w-md mx-auto mb-6 space-y-3">
                    <div class="flex justify-between items-center border-b border-gray-200 pb-2">
                        <span class="text-xs text-gray-500 font-bold uppercase">Student Name</span>
                        <span id="res-name" class="font-bold text-gray-900 text-sm"></span>
                    </div>
                    <div class="flex justify-between items-center border-b border-gray-200 pb-2">
                        <span class="text-xs text-gray-500 font-bold uppercase">Grade & Section</span>
                        <span id="res-grade-sec" class="font-bold text-gray-900 text-sm"></span>
                    </div>
                    <div class="flex justify-between items-center border-b border-gray-200 pb-2">
                        <span class="text-xs text-gray-500 font-bold uppercase">Duration Taken</span>
                        <span id="res-time" class="font-bold text-gray-700 text-sm"></span>
                    </div>
                    <div class="flex justify-between items-center border-b border-gray-200 pb-2">
                        <span class="text-xs text-gray-500 font-bold uppercase">Final Score</span>
                        <span id="res-score" class="font-display font-extrabold text-lg text-gray-900"></span>
                    </div>
                    <div class="flex justify-between items-center pt-1">
                        <span class="text-xs text-gray-500 font-bold uppercase">Badge Status</span>
                        <span id="res-badge-status" class="font-bold text-xs uppercase px-2.5 py-1 rounded-md"></span>
                    </div>
                </div>
            </div>

            <!-- ACTION BUTTONS -->
            <div class="flex flex-col sm:flex-row items-center justify-center gap-3 no-print">
                <button onclick="openReviewModal()" class="w-full sm:w-auto px-5 py-3 bg-gray-100 hover:bg-gray-200 text-gray-800 font-semibold rounded-xl border border-gray-300 text-xs sm:text-sm transition-all flex items-center justify-center space-x-2">
                    <i class="fa-solid fa-list-check"></i>
                    <span>Review Answers</span>
                </button>

                <button onclick="window.print()" class="w-full sm:w-auto px-5 py-3 bg-gray-100 hover:bg-gray-200 text-gray-800 font-semibold rounded-xl border border-gray-300 text-xs sm:text-sm transition-all flex items-center justify-center space-x-2">
                    <i class="fa-solid fa-print"></i>
                    <span>Print Certificate</span>
                </button>

                <button onclick="restartQuiz()" class="w-full sm:w-auto px-6 py-3 bg-gray-900 hover:bg-black font-display font-bold text-white rounded-xl shadow-sm text-xs sm:text-sm transition-all flex items-center justify-center space-x-2">
                    <i class="fa-solid fa-rotate-right"></i>
                    <span>RESTART QUIZ</span>
                </button>
            </div>
        </div>

        <!-- TEACHER DASHBOARD / DATABASE PANEL -->
        <div id="teacher-screen" class="w-full bg-white p-6 sm:p-8 rounded-2xl border border-gray-200 shadow-sm hidden transition-all duration-300">
            <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-4 mb-6 pb-4 border-b border-gray-200">
                <div>
                    <h2 class="font-display text-2xl font-bold text-gray-900">Teacher Online Dashboard</h2>
                    <p class="text-xs text-gray-500">Live Firebase records and responses from all participating students.</p>
                </div>
                <div class="flex items-center gap-2">
                    <button onclick="exportToCSV()" class="px-4 py-2 bg-gray-900 hover:bg-black text-white rounded-xl text-xs font-bold transition-all flex items-center space-x-1">
                        <i class="fa-solid fa-file-csv"></i>
                        <span>Export CSV</span>
                    </button>
                    <button onclick="toggleTeacherPortal()" class="px-4 py-2 bg-gray-100 hover:bg-gray-200 text-gray-700 rounded-xl text-xs font-bold border border-gray-300">
                        Back to Quiz
                    </button>
                </div>
            </div>

            <!-- RECORDS TABLE -->
            <div class="overflow-x-auto">
                <table class="w-full text-left text-xs text-gray-600">
                    <thead class="bg-gray-50 text-gray-700 font-bold uppercase border-b border-gray-200">
                        <tr>
                            <th class="p-3">Student Name</th>
                            <th class="p-3">Grade & Section</th>
                            <th class="p-3">Score</th>
                            <th class="p-3">Time</th>
                            <th class="p-3">Badge Status</th>
                            <th class="p-3">Date</th>
                            <th class="p-3 text-right">Actions</th>
                        </tr>
                    </thead>
                    <tbody id="student-records-body" class="divide-y divide-gray-100">
                        <!-- Dynamic Records -->
                    </tbody>
                </table>
            </div>
        </div>

    </main>

    <!-- ANSWER REVIEW MODAL -->
    <div id="review-modal" class="fixed inset-0 bg-gray-900/60 backdrop-blur-sm hidden items-center justify-center p-4 z-50 no-print">
        <div class="bg-white border border-gray-200 w-full max-w-2xl max-h-[85vh] rounded-2xl shadow-xl flex flex-col">
            <div class="p-5 border-b border-gray-200 flex justify-between items-center">
                <h3 class="font-display font-bold text-lg text-gray-900" id="review-modal-title">Answers Review</h3>
                <button onclick="closeReviewModal()" class="text-gray-400 hover:text-gray-700 text-xl font-bold p-1">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div id="review-list" class="p-5 overflow-y-auto space-y-4 text-left flex-grow">
                <!-- Dynamic Review List -->
            </div>
            <div class="p-4 border-t border-gray-200 bg-gray-50 text-right rounded-b-2xl">
                <button onclick="closeReviewModal()" class="px-5 py-2 bg-gray-900 text-white rounded-xl font-semibold text-xs">
                    Close Review
                </button>
            </div>
        </div>
    </div>

    <!-- FOOTER -->
    <footer class="w-full max-w-4xl mx-auto mt-8 text-center text-xs text-gray-500 no-print">
        <p>© GAME-ON Educational Research Framework • Author: Joel P. Rodriguez LPT MAVED</p>
        <p class="mt-1">Online rankings require your own Firebase project and Firestore configuration.</p>
    </footer>

    <!-- FIREBASE & APPLICATION LOGIC -->
    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
        import { getAuth, signInAnonymously, signInWithCustomToken, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
        import { getFirestore, collection, doc, addDoc, onSnapshot } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";

        // Environment variables setup
        const appId = typeof __app_id !== 'undefined' ? __app_id : 'gameon-quiz-app';
        // IMPORTANT: Replace these placeholders with your own Firebase Web App config.
        // Firebase Console > Project settings > Your apps > Web app > SDK setup and configuration.
        const firebaseConfig = typeof __firebase_config !== 'undefined' ? JSON.parse(__firebase_config) : {
            apiKey: "PASTE_YOUR_FIREBASE_API_KEY",
            authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
            projectId: "YOUR_PROJECT_ID",
            storageBucket: "YOUR_PROJECT_ID.firebasestorage.app",
            messagingSenderId: "PASTE_YOUR_MESSAGING_SENDER_ID",
            appId: "PASTE_YOUR_FIREBASE_APP_ID"
        };

        const app = initializeApp(firebaseConfig);
        const auth = getAuth(app);
        const db = getFirestore(app);

        let currentUser = null;
        let allOnlineRecords = [];

        function escapeHtml(value) {
            return String(value ?? '').replace(/[&<>"']/g, (ch) => ({
                '&': '&amp;', '<': '&lt;', '>': '&gt;', '"': '&quot;', "'": '&#39;'
            }[ch]));
        }

        // Authenticate immediately
        async function initAuth() {
            try {
                if (typeof __initial_auth_token !== 'undefined' && __initial_auth_token) {
                    const cred = await signInWithCustomToken(auth, __initial_auth_token);
                    currentUser = cred.user;
                } else {
                    const cred = await signInAnonymously(auth);
                    currentUser = cred.user;
                }
                document.getElementById('sync-status').innerHTML = '<i class="fa-solid fa-cloud-check text-green-600 mr-1"></i> Live Firebase Online';
                listenToLeaderboardAndRecords();
            } catch (err) {
                console.error("Firebase setup/auth error:", err);
                document.getElementById('sync-status').innerHTML = '<i class="fa-solid fa-circle-exclamation text-amber-500 mr-1"></i> Firebase setup needed — scores may not sync';
            }
        }

        // Live Firestore listener following mandatory rule path
        function listenToLeaderboardAndRecords() {
            if (!currentUser) return;

            // Path: /artifacts/{appId}/public/data/scores
            const scoresCollection = collection(db, 'artifacts', appId, 'public', 'data', 'scores');

            onSnapshot(scoresCollection, (snapshot) => {
                const records = [];
                snapshot.forEach((doc) => {
                    records.push({ id: doc.id, ...doc.data() });
                });

                allOnlineRecords = records;
                renderTop3Leaderboard(records);
                renderTeacherTable(records);
            }, (error) => {
                console.error("Firestore listener error:", error);
            });
        }

        // Render All Student Rankings
        function renderTop3Leaderboard(records) {
            const container = document.getElementById('top-3-container');
            if (!records || records.length === 0) {
                container.innerHTML = `<div class="text-center py-8 text-xs text-gray-400">No submissions recorded yet. Be the first!</div>`;
                return;
            }

            // Sort: Highest score first, then lowest time spent
            const sorted = [...records].sort((a, b) => {
                if (b.score !== a.score) return b.score - a.score;
                return a.timeSeconds - b.timeSeconds;
            });

            container.innerHTML = sorted.map((rec, i) => `
                <div class="flex items-center justify-between p-3 rounded-xl border border-gray-200 bg-gray-50 gap-2">
                    <div class="flex items-center space-x-3 overflow-hidden">
                        <span class="w-8 h-8 rounded-lg ${i === 0 ? 'bg-gray-900 text-white' : 'bg-gray-200 text-gray-800'} flex items-center justify-center font-bold text-xs shrink-0">
                            ${i === 0 ? '<i class="fa-solid fa-trophy text-xs"></i>' : `#${i + 1}`}
                        </span>
                        <div class="truncate">
                            <h4 class="font-bold text-xs text-gray-900 truncate">${escapeHtml(rec.name || 'Unnamed student')}</h4>
                            <p class="text-[10px] text-gray-500">${escapeHtml(rec.gradeSec || '')}</p>
                        </div>
                    </div>
                    <div class="text-right shrink-0">
                        <span class="font-display font-extrabold text-sm text-gray-900">${Number(rec.score) || 0}/10</span>
                        <p class="text-[10px] text-gray-400">${escapeHtml(rec.timeSpent || '')}</p>
                    </div>
                </div>
            `).join('');
        }

        // Render Teacher Table
        function renderTeacherTable(records) {
            const tbody = document.getElementById('student-records-body');
            if (!records || records.length === 0) {
                tbody.innerHTML = `<tr><td colspan="7" class="p-4 text-center text-gray-400">No student records found.</td></tr>`;
                return;
            }

            const sorted = [...records].sort((a, b) => b.timestamp - a.timestamp);

            tbody.innerHTML = sorted.map((r, i) => `
                <tr class="hover:bg-gray-50">
                    <td class="p-3 font-semibold text-gray-900">${escapeHtml(r.name)}</td>
                    <td class="p-3">${escapeHtml(r.gradeSec)}</td>
                    <td class="p-3 font-bold text-gray-900">${r.score}/10</td>
                    <td class="p-3">${escapeHtml(r.timeSpent)}</td>
                    <td class="p-3">
                        <span class="px-2 py-0.5 rounded text-[10px] font-bold ${r.score === 10 ? 'bg-gray-900 text-white' : 'bg-gray-200 text-gray-700'}">
                            ${r.score === 10 ? '50 PTS BADGE' : 'NO BADGE'}
                        </span>
                    </td>
                    <td class="p-3 text-[10px] text-gray-400">${new Date(r.timestamp).toLocaleDateString()}</td>
                    <td class="p-3 text-right">
                        <button onclick="window.viewStudentDetails(${i})" class="px-2 py-1 bg-gray-100 hover:bg-gray-200 text-gray-800 rounded text-[11px] font-semibold">
                            View Responses
                        </button>
                    </td>
                </tr>
            `).join('');
        }

        // Export CSV Functionality
        window.exportToCSV = function() {
            if (allOnlineRecords.length === 0) {
                alert("No records to export.");
                return;
            }

            const headers = ["Student Name", "Grade & Section", "Score", "Time Spent", "Badge Earned", "Timestamp"];
            const rows = allOnlineRecords.map(r => [
                `"${r.name}"`,
                `"${r.gradeSec}"`,
                `"${r.score}/10"`,
                `"${r.timeSpent}"`,
                `"${r.score === 10 ? '50 POINTS BADGE' : 'NO BADGE'}"`,
                `"${new Date(r.timestamp).toLocaleString()}"`
            ]);

            const csvContent = "data:text/csv;charset=utf-8," + [headers.join(","), ...rows.map(e => e.join(","))].join("\n");
            const encodedUri = encodeURI(csvContent);
            const link = document.createElement("a");
            link.setAttribute("href", encodedUri);
            link.setAttribute("download", `GAME_ON_Scores_${new Date().toISOString().slice(0,10)}.csv`);
            document.body.appendChild(link);
            link.click();
            document.body.removeChild(link);
        };

        // Save submission to Firestore
        window.saveSubmissionToFirebase = async function(submission) {
            if (!currentUser) return;
            try {
                const scoresCollection = collection(db, 'artifacts', appId, 'public', 'data', 'scores');
                await addDoc(scoresCollection, submission);
            } catch (err) {
                console.error("Error saving submission:", err);
            }
        };

        window.viewStudentDetails = function(index) {
            const sorted = [...allOnlineRecords].sort((a, b) => b.timestamp - a.timestamp);
            const student = sorted[index];
            if (!student || !student.responses) return;

            const reviewList = document.getElementById('review-list');
            document.getElementById('review-modal-title').textContent = `${student.name} - Breakdown`;
            reviewList.innerHTML = '';

            student.responses.forEach((resp, idx) => {
                const item = document.createElement('div');
                item.className = `p-4 rounded-xl border ${resp.isCorrect ? 'border-gray-300 bg-gray-50' : 'border-gray-300 bg-gray-100'}`;
                item.innerHTML = `
                    <div class="flex items-start justify-between mb-1">
                        <span class="text-xs font-bold ${resp.isCorrect ? 'text-gray-900' : 'text-gray-600'}">
                            Q${idx + 1}: ${resp.isCorrect ? '✓ Correct' : '✗ Incorrect'}
                        </span>
                    </div>
                    <p class="text-xs font-semibold text-gray-900 mb-1">${resp.question}</p>
                    <p class="text-xs text-gray-600">Selected: <strong>${resp.selectedChoice}</strong></p>
                    ${!resp.isCorrect ? `<p class="text-xs text-gray-900 font-medium">Correct: ${resp.correctChoice}</p>` : ''}
                `;
                reviewList.appendChild(item);
            });

            document.getElementById('review-modal').classList.remove('hidden');
            document.getElementById('review-modal').classList.add('flex');
        };

        // Initialize Authentication on load
        initAuth();
    </script>

    <script>
        // Module 5 PowerPoint Assessment Questions
        const rawQuestions = [
            {
                question: "What is the main purpose of creating an interactive PowerPoint game dashboard?",
                options: [
                    "To create an engaging and interactive presentation",
                    "To organize files on a computer",
                    "To edit photographs and videos",
                    "To calculate students' grades automatically"
                ],
                answer: 0
            },
            {
                question: "Which PowerPoint feature allows users to jump from one slide to another by clicking text or an object?",
                options: [
                    "Hyperlink",
                    "WordArt",
                    "Slide Design",
                    "Spell Check"
                ],
                answer: 0
            },
            {
                question: "What is the purpose of custom animations in PowerPoint?",
                options: [
                    "To add movement and visual effects to objects",
                    "To delete unnecessary slides",
                    "To change the computer settings",
                    "To organize files into folders"
                ],
                answer: 0
            },
            {
                question: "Which PowerPoint feature can be used to create clickable navigation controls?",
                options: [
                    "Action Buttons",
                    "Page Borders",
                    "Text Formatting",
                    "Slide Background"
                ],
                answer: 0
            },
            {
                question: "According to Module 5, how many difficulty categories must the game dashboard contain?",
                options: [
                    "Three categories",
                    "Two categories",
                    "Four categories",
                    "Five categories"
                ],
                answer: 0
            },
            {
                question: "If each difficulty category contains 10 questions, how many questions should the entire quiz contain?",
                options: [
                    "30 questions",
                    "20 questions",
                    "25 questions",
                    "40 questions"
                ],
                answer: 0
            },
            {
                question: "What is the primary function of slide navigation in an interactive presentation?",
                options: [
                    "To help users move between slides",
                    "To change the computer password",
                    "To print all presentation slides",
                    "To remove all animations"
                ],
                answer: 0
            },
            {
                question: "Which of the following is an example of an interactive PowerPoint element?",
                options: [
                    "A clickable button that opens another slide",
                    "A printed worksheet without links",
                    "A static picture with no clickable feature",
                    "A paragraph displayed on a slide"
                ],
                answer: 0
            },
            {
                question: "What should students consider when designing their PowerPoint game dashboard?",
                options: [
                    "Making the presentation engaging, organized, and interactive",
                    "Using only plain text on every slide",
                    "Removing all navigation features",
                    "Placing all questions on one slide"
                ],
                answer: 0
            },
            {
                question: "Which combination of features best supports the creation of an interactive PowerPoint quiz?",
                options: [
                    "Hyperlinks, slide navigation, action buttons, and custom animations",
                    "Spell Check, Word Count, and Page Margins",
                    "Crop, Brightness, and Picture Borders",
                    "File Explorer, Calculator, and Notepad"
                ],
                answer: 0
            }
        ];

        // Quiz State
        let quizQuestions = [];
        let userAnswers = {};
        let currentQuestionIdx = 0;
        let timerInterval = null;
        let timeRemaining = 600;
        let studentData = { name: '', grade: '', section: '' };

        function validateForm() {
            const name = document.getElementById('student-name').value.trim();
            const grade = document.getElementById('student-grade').value.trim();
            const section = document.getElementById('student-section').value.trim();
            document.getElementById('start-btn').disabled = !(name && grade && section);
        }

        function shuffleArray(array) {
            const arr = [...array];
            for (let i = arr.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [arr[i], arr[j]] = [arr[j], arr[i]];
            }
            return arr;
        }

        function prepareQuestions() {
            const shuffledRaw = shuffleArray(rawQuestions);
            quizQuestions = shuffledRaw.map(q => {
                const choices = q.options.map((opt, idx) => ({
                    text: opt,
                    isCorrect: idx === q.answer
                }));
                return {
                    question: q.question,
                    choices: shuffleArray(choices)
                };
            });
        }

        function startQuiz() {
            studentData.name = document.getElementById('student-name').value.trim();
            studentData.grade = document.getElementById('student-grade').value.trim();
            studentData.section = document.getElementById('student-section').value.trim();

            prepareQuestions();
            userAnswers = {};
            currentQuestionIdx = 0;
            timeRemaining = 600;

            document.getElementById('start-screen').classList.add('hidden');
            document.getElementById('quiz-screen').classList.remove('hidden');

            startTimer();
            renderQuestion();
        }

        function startTimer() {
            clearInterval(timerInterval);
            updateTimerDisplay();
            timerInterval = setInterval(() => {
                timeRemaining--;
                updateTimerDisplay();
                if (timeRemaining <= 0) {
                    clearInterval(timerInterval);
                    submitQuiz(true);
                }
            }, 1000);
        }

        function updateTimerDisplay() {
            const minutes = Math.floor(timeRemaining / 60);
            const seconds = timeRemaining % 60;
            const timerElem = document.getElementById('timer-display');
            timerElem.textContent = `${minutes.toString().padStart(2, '0')}:${seconds.toString().padStart(2, '0')}`;
        }

        function renderQuestion() {
            const qData = quizQuestions[currentQuestionIdx];
            document.getElementById('question-tracker').textContent = `${currentQuestionIdx + 1} / ${quizQuestions.length}`;
            document.getElementById('question-text').textContent = `${currentQuestionIdx + 1}. ${qData.question}`;

            document.getElementById('progress-bar').style.width = `${((currentQuestionIdx + 1) / quizQuestions.length) * 100}%`;

            const container = document.getElementById('choices-container');
            container.innerHTML = '';

            qData.choices.forEach((choice, idx) => {
                const isSelected = userAnswers[currentQuestionIdx] === idx;
                const choiceBtn = document.createElement('div');
                choiceBtn.innerHTML = `
                    <input type="radio" id="choice-${idx}" name="quiz-option" value="${idx}" ${isSelected ? 'checked' : ''} class="hidden custom-radio" onchange="selectOption(${idx})">
                    <label for="choice-${idx}" class="flex items-start p-3.5 rounded-xl border border-gray-300 bg-white hover:bg-gray-50 cursor-pointer transition-all">
                        <span class="w-6 h-6 rounded-md border border-gray-400 bg-gray-100 flex items-center justify-center text-xs font-bold mr-3 text-gray-800 shrink-0 mt-0.5">
                            ${String.fromCharCode(65 + idx)}
                        </span>
                        <span class="text-xs sm:text-sm text-gray-800 font-medium leading-relaxed">${choice.text}</span>
                    </label>
                `;
                container.appendChild(choiceBtn);
            });

            document.getElementById('prev-btn').disabled = currentQuestionIdx === 0;
            const nextBtnText = document.getElementById('next-btn-text');
            const nextBtnIcon = document.getElementById('next-btn-icon');

            if (currentQuestionIdx === quizQuestions.length - 1) {
                nextBtnText.textContent = "FINISH & SUBMIT";
                nextBtnIcon.className = "fa-solid fa-check-double";
            } else {
                nextBtnText.textContent = "Next";
                nextBtnIcon.className = "fa-solid fa-arrow-right";
            }
        }

        function selectOption(idx) {
            userAnswers[currentQuestionIdx] = idx;
        }

        function nextQuestion() {
            if (currentQuestionIdx < quizQuestions.length - 1) {
                currentQuestionIdx++;
                renderQuestion();
            } else {
                submitQuiz(false);
            }
        }

        function previousQuestion() {
            if (currentQuestionIdx > 0) {
                currentQuestionIdx--;
                renderQuestion();
            }
        }

        async function submitQuiz(isTimeout = false) {
            clearInterval(timerInterval);

            let score = 0;
            const detailedResponses = [];

            quizQuestions.forEach((q, idx) => {
                const selectedIdx = userAnswers[idx];
                const isCorrect = selectedIdx !== undefined && q.choices[selectedIdx].isCorrect;
                if (isCorrect) score++;

                const correctChoice = q.choices.find(c => c.isCorrect)?.text || '';
                const selectedChoice = selectedIdx !== undefined ? q.choices[selectedIdx].text : 'Unanswered';

                detailedResponses.push({
                    question: q.question,
                    selectedChoice,
                    correctChoice,
                    isCorrect
                });
            });

            const timeSpentSecs = 600 - timeRemaining;
            const minsSpent = Math.floor(timeSpentSecs / 60);
            const secsSpent = timeSpentSecs % 60;
            const timeString = `${minsSpent}m ${secsSpent}s`;

            // Prepare record object
            const record = {
                name: studentData.name,
                gradeSec: `${studentData.grade} - ${studentData.section}`,
                score: score,
                timeSpent: timeString,
                timeSeconds: timeSpentSecs,
                timestamp: Date.now(),
                responses: detailedResponses
            };

            // Save to Firebase Cloud DB
            if (window.saveSubmissionToFirebase) {
                await window.saveSubmissionToFirebase(record);
            }

            // Update UI Screen
            document.getElementById('res-name').textContent = studentData.name;
            document.getElementById('res-grade-sec').textContent = record.gradeSec;
            document.getElementById('res-time').textContent = timeString;
            document.getElementById('res-score').textContent = `${score} / 10`;

            const badgeContainer = document.getElementById('badge-container');
            const standardHeader = document.getElementById('standard-result-header');
            const badgeStatusElem = document.getElementById('res-badge-status');

            if (score === 10) {
                badgeContainer.classList.remove('hidden');
                standardHeader.classList.add('hidden');
                badgeStatusElem.textContent = "UNLOCKED (50 PTS)";
                badgeStatusElem.className = "font-bold text-xs uppercase px-2.5 py-1 rounded-md bg-gray-900 text-white border border-gray-900";
            } else {
                badgeContainer.classList.add('hidden');
                standardHeader.classList.remove('hidden');
                badgeStatusElem.textContent = "LOCKED (Requires 10/10)";
                badgeStatusElem.className = "font-bold text-xs uppercase px-2.5 py-1 rounded-md bg-gray-200 text-gray-700 border border-gray-300";
            }

            document.getElementById('quiz-screen').classList.add('hidden');
            document.getElementById('result-screen').classList.remove('hidden');
        }

        function openReviewModal() {
            document.getElementById('review-modal-title').textContent = "Answers Review";
            const reviewList = document.getElementById('review-list');
            reviewList.innerHTML = '';

            quizQuestions.forEach((q, idx) => {
                const selectedIdx = userAnswers[idx];
                const correctChoice = q.choices.find(c => c.isCorrect);
                const userChoice = selectedIdx !== undefined ? q.choices[selectedIdx] : null;
                const isCorrect = userChoice && userChoice.isCorrect;

                const item = document.createElement('div');
                item.className = `p-4 rounded-xl border ${isCorrect ? 'border-gray-300 bg-gray-50' : 'border-gray-300 bg-gray-100'}`;
                item.innerHTML = `
                    <div class="flex items-start justify-between mb-1">
                        <span class="text-xs font-bold ${isCorrect ? 'text-gray-900' : 'text-gray-600'}">
                            Q${idx + 1}: ${isCorrect ? '✓ Correct' : '✗ Incorrect'}
                        </span>
                    </div>
                    <p class="text-xs font-semibold text-gray-900 mb-1">${q.question}</p>
                    <p class="text-xs text-gray-600">Selected: <strong>${userChoice ? userChoice.text : 'Unanswered'}</strong></p>
                    ${!isCorrect ? `<p class="text-xs text-gray-900 font-medium">Correct: ${correctChoice.text}</p>` : ''}
                `;
                reviewList.appendChild(item);
            });

            document.getElementById('review-modal').classList.remove('hidden');
            document.getElementById('review-modal').classList.add('flex');
        }

        function closeReviewModal() {
            document.getElementById('review-modal').classList.add('hidden');
            document.getElementById('review-modal').classList.remove('flex');
        }

        function restartQuiz() {
            document.getElementById('result-screen').classList.add('hidden');
            document.getElementById('teacher-screen').classList.add('hidden');
            document.getElementById('start-screen').classList.remove('hidden');
            validateForm();
        }

        function toggleTeacherPortal() {
            const teacherScreen = document.getElementById('teacher-screen');
            const startScreen = document.getElementById('start-screen');

            if (teacherScreen.classList.contains('hidden')) {
                startScreen.classList.add('hidden');
                teacherScreen.classList.remove('hidden');
            } else {
                teacherScreen.classList.add('hidden');
                startScreen.classList.remove('hidden');
            }
        }
    </script>
</body>
</html>
