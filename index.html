<!DOCTYPE html>
<html lang="ko">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>베스트론 - 클라우드 공유</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
    
    <!-- Firebase SDK -->
    <script type="module">
        import { initializeApp } from 'https://www.gstatic.com/firebasejs/10.7.1/firebase-app.js';
        import { getFirestore, collection, addDoc, getDocs, doc, updateDoc, deleteDoc, onSnapshot, query, orderBy } from 'https://www.gstatic.com/firebasejs/10.7.1/firebase-firestore.js';
        
        // Firebase 설정 (실제 설정으로 업데이트됨)
        const firebaseConfig = {
            apiKey: "AIzaSyDkwYnI7Lp4qGZSyrVFdVqpiaTEvixnqYY",
            authDomain: "bestroncompany.firebaseapp.com",
            projectId: "bestroncompany",
            storageBucket: "bestroncompany.firebasestorage.app",
            messagingSenderId: "279464057042",
            appId: "1:279464057042:web:71d1c39a852ef31de7f50b",
            measurementId: "G-ERXFT62XQ"
        };

        // Firebase 앱 초기화
        const app = initializeApp(firebaseConfig);
        const db = getFirestore(app);
        
        // 전역에서 사용할 수 있도록 설정
        window.firebaseDb = db;
        window.firebaseModules = {
            collection,
            addDoc,
            getDocs,
            doc,
            updateDoc,
            deleteDoc,
            onSnapshot,
            query,
            orderBy
        };
        
        // Firebase 초기화 완료 이벤트 발생
        window.dispatchEvent(new Event('firebaseReady'));
    </script>
    
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300;400;500;600;700;800&display=swap');

        * {
            font-family: 'Noto Sans KR', sans-serif;
        }

        body {
            background: linear-gradient(135deg, #000000 0%, #1a1a1a 50%, #000000 100%);
            min-height: 100vh;
        }

        .login-bg {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url(https://cdn.pixabay.com/photo/2016/11/23/15/23/cosmos-1853491_1280.jpg);
            background-size: cover;
            background-position: center;
            min-height: 100vh;
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.98);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
        }

        .status-badge {
            transition: all 0.3s ease;
        }

        .status-badge:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
        }

        .table-row {
            transition: all 0.3s ease;
        }

        .table-row:hover {
            background: rgba(0, 0, 0, 0.05);
        }

        .btn-primary {
            background: linear-gradient(135deg, #000000 0%, #333333 100%);
            transition: all 0.3s ease;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.4);
        }

        .btn-success {
            background: linear-gradient(135deg, #10b981 0%, #059669 100%);
            transition: all 0.3s ease;
        }

        .btn-success:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(16, 185, 129, 0.4);
        }

        .btn-info {
            background: linear-gradient(135deg, #3b82f6 0%, #1d4ed8 100%);
            transition: all 0.3s ease;
        }

        .btn-info:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(59, 130, 246, 0.4);
        }

        .modal-overlay {
            background: rgba(0, 0, 0, 0.7);
            backdrop-filter: blur(5px);
        }

        .animate-fade-in {
            animation: fadeIn 0.5s ease-in-out;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .status-waiting {
            background: #fbbf24;
            color: #fbbf24;
        }

        .status-first-call {
            background: #dbeafe;
            color: #1e40af;
        }

        .status-in-progress {
            background: #f97316;
            color: #f97316;
        }

        .status-approved {
            background: #ec4899;
            color: #ec4899;
        }

        .status-absent {
            background: #374151;
            color: #374151;
        }

        .status-rejected {
            background: #ef4444;
            color: #ef4444;
        }

        .status-as {
            background: #8b5cf6;
            color: #8b5cf6;
        }

        .status-recontact {
            background: #a16207;
            color: #a16207;
        }

        .category-tab {
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .category-tab.active {
            background: linear-gradient(135deg, #000000 0%, #333333 100%);
            color: white;
        }

        .category-tab:not(.active):hover {
            background: rgba(0, 0, 0, 0.1);
        }

        .logo-text {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .checkbox-custom {
            width: 16px;
            height: 16px;
            accent-color: #000000;
        }

        .editable-field {
            cursor: pointer;
            padding: 1px 4px;
            border-radius: 3px;
            transition: all 0.3s ease;
        }

        .editable-field:hover {
            background: rgba(0, 0, 0, 0.05);
            color: #2563eb;
        }

        .compact-table {
            table-layout: fixed;
            width: 100%;
            border-collapse: collapse;
        }

        .compact-table th {
            padding: 6px 2px;
            font-size: 12px;
            text-align: center;
            border-right: 1px solid #e5e7eb;
        }

        .compact-table td {
            padding: 5px 2px;
            font-size: 13px;
            text-align: center;
            border-right: 1px solid #e5e7eb;
        }

        .compact-table th:first-child,
        .compact-table td:first-child {
            width: 4%;
        }

        .compact-table th:nth-child(2),
        .compact-table td:nth-child(2) {
            width: 6%;
        }

        .compact-table th:nth-child(3),
        .compact-table td:nth-child(3) {
            width: 8%;
        }

        .compact-table th:nth-child(4),
        .compact-table td:nth-child(4) {
            width: 10%;
        }

        .compact-table th:nth-child(5),
        .compact-table td:nth-child(5) {
            width: 8%;
        }

        .compact-table th:nth-child(6),
        .compact-table td:nth-child(6) {
            width: 12%;
        }

        .compact-table th:nth-child(7),
        .compact-table td:nth-child(7) {
            width: 8%;
        }

        .compact-table th:nth-child(8),
        .compact-table td:nth-child(8) {
            width: 12%;
        }

        .compact-table th:nth-child(9),
        .compact-table td:nth-child(9) {
            width: 12%;
        }

        .compact-table th:nth-child(10),
        .compact-table td:nth-child(10) {
            width: 8%;
        }

        .compact-table th:nth-child(11),
        .compact-table td:nth-child(11) {
            width: 12%;
        }

        .status-select,
        .manager-select {
            background: transparent;
            border: none;
            outline: none;
            cursor: pointer;
            appearance: none;
            -webkit-appearance: none;
            -moz-appearance: none;
            text-align: center;
            width: 100%;
            font-size: 12px;
        }

        .status-select:focus,
        .manager-select:focus {
            outline: 2px solid #3b82f6;
            outline-offset: 1px;
        }

        .compact-btn {
            padding: 6px 10px;
            font-size: 12px;
        }

        .cloud-status {
            position: fixed;
            top: 20px;
            right: 20px;
            background: rgba(255, 255, 255, 0.9);
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: 600;
            z-index: 1000;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }

        .cloud-status.connected {
            color: #10b981;
            border: 2px solid #10b981;
        }

        .cloud-status.disconnected {
            color: #ef4444;
            border: 2px solid #ef4444;
        }

        .cloud-status.syncing {
            color: #f59e0b;
            border: 2px solid #f59e0b;
        }

        .realtime-indicator {
            display: inline-block;
            width: 8px;
            height: 8px;
            background: #10b981;
            border-radius: 50%;
            margin-right: 6px;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { opacity: 1; }
            50% { opacity: 0.5; }
            100% { opacity: 1; }
        }

        .pagination {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 8px;
            margin-top: 20px;
        }

        .pagination button {
            padding: 8px 12px;
            border: 1px solid #d1d5db;
            background: white;
            color: #374151;
            border-radius: 6px;
            cursor: pointer;
            transition: all 0.2s;
            font-size: 14px;
        }

        .pagination button:hover:not(:disabled) {
            background: #f3f4f6;
            border-color: #9ca3af;
        }

        .pagination button.active {
            background: #000000;
            color: white;
            border-color: #000000;
        }

        .pagination button:disabled {
            opacity: 0.5;
            cursor: not-allowed;
        }

        .items-per-page {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 14px;
            color: #374151;
        }

        .items-per-page select {
            padding: 4px 8px;
            border: 1px solid #d1d5db;
            border-radius: 4px;
            background: white;
        }

        /* 모바일 반응형 스타일 */
        @media (max-width: 768px) {
            .container {
                padding-left: 8px;
                padding-right: 8px;
            }

            .glass-card {
                margin: 4px;
                padding: 12px;
            }

            .mobile-header-buttons {
                display: flex;
                flex-direction: column;
                gap: 8px;
                width: 100%;
            }

            .mobile-header-buttons button {
                width: 100%;
                text-align: center;
                padding: 12px;
                font-size: 14px;
            }

            .mobile-table-container {
                overflow-x: auto;
                -webkit-overflow-scrolling: touch;
            }

            .compact-table {
                min-width: 800px;
            }

            .compact-table th,
            .compact-table td {
                padding: 8px 4px;
                font-size: 11px;
                white-space: nowrap;
            }

            .category-tabs-container {
                overflow-x: auto;
                -webkit-overflow-scrolling: touch;
            }

            .category-tabs {
                display: flex;
                flex-wrap: nowrap;
                min-width: max-content;
            }

            .category-tab {
                flex-shrink: 0;
                padding: 12px 16px;
                font-size: 14px;
                white-space: nowrap;
            }

            .mobile-search-container {
                flex-direction: column;
                gap: 8px;
            }

            .mobile-search-container input {
                width: 100%;
            }

            .mobile-search-container button {
                width: 100%;
            }

            .mobile-stats-grid {
                grid-template-columns: 1fr 1fr;
                gap: 8px;
            }

            .mobile-stats-card {
                padding: 12px;
                text-align: center;
            }

            .mobile-stats-card p:first-child {
                font-size: 12px;
            }

            .mobile-stats-card p:last-child {
                font-size: 18px;
            }

            .mobile-modal {
                margin: 8px;
                max-height: 90vh;
                overflow-y: auto;
            }

            .mobile-modal .grid {
                grid-template-columns: 1fr;
                gap: 12px;
            }

            .mobile-modal input,
            .mobile-modal select {
                padding: 12px;
                font-size: 16px;
            }

            .mobile-login-form {
                margin: 16px;
                padding: 24px;
            }

            .mobile-login-form input {
                padding: 16px;
                font-size: 16px;
            }

            .cloud-status {
                position: fixed;
                top: 10px;
                right: 10px;
                font-size: 10px;
                padding: 6px 12px;
            }

            .pagination {
                flex-wrap: wrap;
                gap: 4px;
            }

            .pagination button {
                padding: 6px 8px;
                font-size: 12px;
            }

            .items-per-page {
                font-size: 12px;
            }
        }

        @media (max-width: 480px) {
            .compact-table th,
            .compact-table td {
                padding: 6px 2px;
                font-size: 10px;
            }

            .category-tab {
                padding: 10px 12px;
                font-size: 12px;
            }

            .mobile-stats-card p:last-child {
                font-size: 16px;
            }
        }
    </style>
</head>

<body>
    <!-- 클라우드 연결 상태 표시 -->
    <div id="cloudStatus" class="cloud-status disconnected">
        <span class="realtime-indicator"></span>
        연결 중...
    </div>

    <!-- Login Screen -->
    <div id="loginScreen" class="login-bg flex items-center justify-center">
        <div class="glass-card rounded-2xl p-8 w-full max-w-md mobile-login-form">
            <div class="text-center mb-8">
                <h1 class="text-4xl font-bold logo-text mb-2">베스트론</h1>
                <p class="text-gray-600">실시간 클라우드 공유</p>
            </div>

            <form onsubmit="handleLogin(event)">
                <div class="mb-4">
                    <label class="block text-sm font-medium text-gray-700 mb-2">아이디</label>
                    <input type="text" id="loginId"
                        class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                        placeholder="아이디를 입력하세요">
                </div>
                <div class="mb-6">
                    <label class="block text-sm font-medium text-gray-700 mb-2">비밀번호</label>
                    <input type="password" id="loginPassword"
                        class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                        placeholder="비밀번호를 입력하세요">
                </div>
                <button type="submit"
                    class="w-full btn-primary text-white px-6 py-3 rounded-lg font-semibold">로그인</button>
            </form>
        </div>
    </div>

    <!-- Main Application -->
    <div id="mainApp" class="hidden">
        <div class="container mx-auto px-4 py-6">
            <!-- Header -->
            <div class="glass-card rounded-2xl p-5 mb-5 animate-fade-in">
                <div class="flex flex-col md:flex-row items-center justify-between">
                    <div class="mb-4 md:mb-0">
                        <h1 class="text-2xl font-bold text-gray-900 mb-1">베스트론</h1>
                        <p class="text-sm text-gray-600">실시간 클라우드 동기화</p>
                    </div>
                    <div class="w-full md:w-auto">
                        <!-- Desktop buttons -->
                        <div class="hidden md:flex space-x-2">
                            <button onclick="toggleRegistration()"
                                class="flex items-center space-x-2 btn-success text-white compact-btn rounded-lg font-medium">
                                <svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M12 6v6m0 0v6m0-6h6m-6 0H6"></path>
                                </svg>
                                <span>상담등록</span>
                            </button>

                            <button onclick="downloadBackup()"
                                class="flex items-center space-x-2 bg-purple-600 hover:bg-purple-700 text-white compact-btn rounded-lg font-medium transition-all">
                                <svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M12 10v6m0 0l-3-3m3 3l3-3M3 17V7a2 2 0 012-2h6l2 2h6a2 2 0 012 2v10a2 2 0 01-2 2H5a2 2 0 01-2-2z">
                                    </path>
                                </svg>
                                <span>백업다운로드</span>
                            </button>

                            <button onclick="openBatchStatusModal()"
                                class="flex items-center space-x-2 btn-info text-white compact-btn rounded-lg font-medium opacity-50 cursor-not-allowed"
                                id="batchStatusBtn" disabled>
                                <svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M4 6h16M4 12h16M4 18h16"></path>
                                </svg>
                                <span>체크목록 상태변경</span>
                            </button>

                            <button onclick="openBatchDeleteModal()"
                                class="flex items-center space-x-2 bg-red-600 hover:bg-red-700 text-white compact-btn rounded-lg font-medium transition-all opacity-50 cursor-not-allowed"
                                id="batchDeleteBtn" disabled>
                                <svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M19 7l-.867 12.142A2 2 0 0116.138 21H7.862a2 2 0 01-1.995-1.858L5 7m5 4v6m4-6v6m1-10V4a1 1 0 00-1-1h-4a1 1 0 00-1 1v3M4 7h16">
                                    </path>
                                </svg>
                                <span>체크목록 삭제</span>
                            </button>

                            <button onclick="logout()"
                                class="flex items-center space-x-2 text-red-600 hover:text-red-800 compact-btn border border-red-600 rounded-lg font-medium transition-colors">
                                <svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M17 16l4-4m0 0l-4-4m4 4H7m6 4v1a3 3 0 01-3 3H6a3 3 0 01-3-3V7a3 3 0 013-3h4a3 3 0 013 3v1">
                                    </path>
                                </svg>
                                <span>로그아웃</span>
                            </button>
                        </div>

                        <!-- Mobile buttons -->
                        <div class="md:hidden mobile-header-buttons">
                            <button onclick="toggleRegistration()"
                                class="flex items-center justify-center space-x-2 btn-success text-white rounded-lg font-medium">
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M12 6v6m0 0v6m0-6h6m-6 0H6"></path>
                                </svg>
                                <span>상담등록</span>
                            </button>

                            <button onclick="downloadBackup()"
                                class="flex items-center justify-center space-x-2 bg-purple-600 hover:bg-purple-700 text-white rounded-lg font-medium transition-all">
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M12 10v6m0 0l-3-3m3 3l3-3M3 17V7a2 2 0 012-2h6l2 2h6a2 2 0 012 2v10a2 2 0 01-2 2H5a2 2 0 01-2-2z">
                                    </path>
                                </svg>
                                <span>백업다운로드</span>
                            </button>

                            <button onclick="openBatchStatusModal()"
                                class="flex items-center justify-center space-x-2 btn-info text-white rounded-lg font-medium opacity-50 cursor-not-allowed"
                                id="batchStatusBtnMobile" disabled>
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M4 6h16M4 12h16M4 18h16"></path>
                                </svg>
                                <span>체크목록 상태변경</span>
                            </button>

                            <button onclick="openBatchDeleteModal()"
                                class="flex items-center justify-center space-x-2 bg-red-600 hover:bg-red-700 text-white rounded-lg font-medium transition-all opacity-50 cursor-not-allowed"
                                id="batchDeleteBtnMobile" disabled>
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M19 7l-.867 12.142A2 2 0 0116.138 21H7.862a2 2 0 01-1.995-1.858L5 7m5 4v6m4-6v6m1-10V4a1 1 0 00-1-1h-4a1 1 0 00-1 1v3M4 7h16">
                                    </path>
                                </svg>
                                <span>체크목록 삭제</span>
                            </button>

                            <button onclick="logout()"
                                class="flex items-center justify-center space-x-2 text-red-600 hover:text-red-800 border border-red-600 rounded-lg font-medium transition-colors">
                                <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M17 16l4-4m0 0l-4-4m4 4H7m6 4v1a3 3 0 01-3 3H6a3 3 0 01-3-3V7a3 3 0 013-3h4a3 3 0 013 3v1">
                                    </path>
                                </svg>
                                <span>로그아웃</span>
                            </button>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Registration Modal -->
            <div id="registrationModal" class="fixed inset-0 modal-overlay hidden items-center justify-center z-50">
                <div class="glass-card rounded-2xl p-6 max-w-2xl w-full mx-4 mobile-modal">
                    <div class="flex items-center justify-between mb-6">
                        <h3 class="text-lg font-semibold text-gray-900">상담 등록</h3>
                        <button onclick="closeRegistration()" class="text-gray-500 hover:text-gray-700">
                            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                    d="M6 18L18 6M6 6l12 12"></path>
                            </svg>
                        </button>
                    </div>

                    <div class="flex flex-col md:flex-row space-y-4 md:space-y-0 md:space-x-4 mb-6">
                        <!-- File Upload Button -->
                        <input id="file-upload" name="file-upload" type="file" accept=".xls,.xlsx" class="hidden"
                            onchange="handleFileUpload(event)">
                        <button onclick="document.getElementById('file-upload').click()"
                            class="flex items-center justify-center space-x-2 btn-success text-white px-4 py-2 rounded-lg font-medium">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                    d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12">
                                </path>
                            </svg>
                            <span>Excel 업로드</span>
                        </button>

                        <!-- Toggle Manual Input Button -->
                        <button onclick="toggleManualInput()"
                            class="flex items-center justify-center space-x-2 btn-info text-white px-4 py-2 rounded-lg font-medium">
                            <svg id="toggleIcon" class="w-4 h-4 transition-transform" fill="none" stroke="currentColor"
                                viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                    d="M19 9l-7 7-7-7"></path>
                            </svg>
                            <span>개별 등록</span>
                        </button>
                    </div>

                    <!-- Manual Input Section -->
                    <div id="manualInputSection" class="hidden">
                        <div class="grid grid-cols-1 md:grid-cols-6 gap-4">
                            <input type="text" id="customerName" placeholder="고객명"
                                class="px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent">
                            <select id="customerJob"
                                class="px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent">
                                <option value="">직업 선택</option>
                                <option value="직장인">직장인</option>
                                <option value="사업자">사업자</option>
                                <option value="프리랜서">프리랜서</option>
                            </select>
                            <input type="tel" id="customerPhone" placeholder="연락처"
                                class="px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent">
                            <select id="customerCarrier"
                                class="px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent">
                                <option value="">통신사 선택</option>
                                <option value="SKT">SKT</option>
                                <option value="KT">KT</option>
                                <option value="LG">LG</option>
                                <option value="SK알뜰">SK알뜰</option>
                                <option value="KT알뜰">KT알뜰</option>
                                <option value="LG알뜰">LG알뜰</option>
                            </select>
                            <input type="text" id="birthDate" placeholder="생년월일 (예: 1990-01-01)"
                                class="px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent">
                            <button onclick="addConsultation()"
                                class="btn-primary text-white px-6 py-3 rounded-lg font-semibold">등록</button>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Stats Cards -->
            <div class="grid grid-cols-1 md:grid-cols-4 mobile-stats-grid gap-4 mb-6">
                <div class="glass-card rounded-xl p-4 mobile-stats-card animate-fade-in">
                    <p class="text-sm text-gray-600">총 상담</p>
                    <p class="text-2xl font-bold text-gray-900" id="totalCount">0</p>
                </div>
                <div class="glass-card rounded-xl p-4 mobile-stats-card animate-fade-in">
                    <p class="text-sm text-gray-600">진행 중</p>
                    <p class="text-2xl font-bold text-orange-600" id="progressCount">0</p>
                </div>
                <div class="glass-card rounded-xl p-4 mobile-stats-card animate-fade-in">
                    <p class="text-sm text-gray-600">승인 완료</p>
                    <p class="text-2xl font-bold text-green-600" id="approvedCount">0</p>
                </div>
                <div class="glass-card rounded-xl p-4 mobile-stats-card animate-fade-in">
                    <p class="text-sm text-gray-600">선택된 항목</p>
                    <p class="text-2xl font-bold text-blue-600" id="selectedCount">0</p>
                </div>
            </div>

            <!-- Category Tabs -->
            <div class="glass-card rounded-2xl mb-6 animate-fade-in">
                <!-- Search Bar -->
                <div class="p-4 border-b">
                    <div class="flex flex-col md:flex-row mobile-search-container items-center space-y-4 md:space-y-0 md:space-x-4">
                        <div class="flex-1 w-full">
                            <div class="relative">
                                <input type="text" id="searchInput" placeholder="고객명 또는 연락처로 검색 (부분 검색 가능)"
                                    class="w-full pl-10 pr-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent text-sm"
                                    onkeyup="handleSearch(event)">
                                <div class="absolute inset-y-0 left-0 pl-3 flex items-center pointer-events-none">
                                    <svg class="h-5 w-5 text-gray-400" fill="none" stroke="currentColor"
                                        viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path>
                                    </svg>
                                </div>
                            </div>
                        </div>
                        <button onclick="clearSearch()"
                            class="px-4 py-3 text-gray-600 hover:text-gray-800 border border-gray-300 rounded-lg transition-colors">
                            초기화
                        </button>
                    </div>
                </div>

                <div class="category-tabs-container">
                    <div class="flex flex-wrap category-tabs border-b">
                        <button onclick="showCategory('all')" class="category-tab active px-6 py-4 font-medium text-sm"
                            data-category="all">전체</button>
                        <button onclick="showCategory('상담대기')" class="category-tab px-6 py-4 font-medium text-sm"
                            data-category="상담대기">상담대기</button>
                        <button onclick="showCategory('1차콜완료')" class="category-tab px-6 py-4 font-medium text-sm"
                            data-category="1차콜완료">1차콜완료</button>
                        <button onclick="showCategory('진행중')" class="category-tab px-6 py-4 font-medium text-sm"
                            data-category="진행중">진행중</button>
                        <button onclick="showCategory('❤️승인완료❤️')" class="category-tab px-6 py-4 font-medium text-sm"
                            data-category="❤️승인완료❤️">❤️승인완료❤️</button>
                        <button onclick="showCategory('부재')" class="category-tab px-6 py-4 font-medium text-sm"
                            data-category="부재">부재</button>
                        <button onclick="showCategory('부결')" class="category-tab px-6 py-4 font-medium text-sm"
                            data-category="부결">부결</button>
                        <button onclick="showCategory('A/S')" class="category-tab px-6 py-4 font-medium text-sm"
                            data-category="A/S">A/S</button>
                        <button onclick="showCategory('재컨택')" class="category-tab px-6 py-4 font-medium text-sm"
                            data-category="재컨택">재컨택</button>
                    </div>
                </div>

                <!-- Consultation List -->
                <div class="p-5">
                    <!-- Items per page and pagination controls -->
                    <div class="flex flex-col md:flex-row justify-between items-center mb-4">
                        <div class="items-per-page mb-2 md:mb-0">
                            <label for="itemsPerPage">페이지당 항목:</label>
                            <select id="itemsPerPage" onchange="changeItemsPerPage()">
                                <option value="10">10개</option>
                                <option value="20" selected>20개</option>
                                <option value="50">50개</option>
                                <option value="100">100개</option>
                            </select>
                        </div>
                        <div class="text-sm text-gray-600">
                            총 <span id="totalItems">0</span>건 중 <span id="currentRange">0-0</span>건 표시
                        </div>
                    </div>

                    <div class="mobile-table-container">
                        <table class="w-full compact-table">
                            <thead class="bg-gray-50">
                                <tr>
                                    <th class="text-left">
                                        <input type="checkbox" id="selectAll" onchange="toggleSelectAll()"
                                            class="checkbox-custom">
                                    </th>
                                    <th class="text-left text-xs font-medium text-gray-500 uppercase">DB</th>
                                    <th class="text-left text-xs font-medium text-gray-500 uppercase">고객명</th>
                                    <th class="text-left text-xs font-medium text-gray-500 uppercase">생년월일</th>
                                    <th class="text-left text-xs font-medium text-gray-500 uppercase">직업</th>
                                    <th class="text-left text-xs font-medium text-gray-500 uppercase">연락처</th>
                                    <th class="text-left text-xs font-medium text-gray-500 uppercase">통신사</th>
                                    <th class="text-left text-xs font-medium text-gray-500 uppercase">메모</th>
                                    <th class="text-left text-xs font-medium text-gray-500 uppercase">상담상태</th>
                                    <th class="text-left text-xs font-medium text-gray-500 uppercase">담당자</th>
                                    <th class="text-left text-xs font-medium text-gray-500 uppercase">등록일</th>
                                </tr>
                            </thead>
                            <tbody id="consultationList" class="bg-white divide-y divide-gray-100">
                                <!-- Data will be populated by JavaScript -->
                            </tbody>
                        </table>
                    </div>

                    <!-- Pagination -->
                    <div class="pagination" id="pagination">
                        <!-- Pagination buttons will be generated by JavaScript -->
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- 모든 기존 모달들 -->
    <!-- Batch Status Change Modal -->
    <div id="batchStatusModal" class="fixed inset-0 modal-overlay hidden items-center justify-center z-50">
        <div class="glass-card rounded-2xl p-6 max-w-md w-full mx-4 mobile-modal">
            <h3 class="text-lg font-semibold text-gray-900 mb-4">체크목록 상태변경</h3>
            <div class="mb-4">
                <label class="block text-sm font-medium text-gray-700 mb-2">선택된 항목</label>
                <p id="batchSelectedCount" class="text-gray-900 font-semibold">0개</p>
            </div>
            <div class="mb-6">
                <label class="block text-sm font-medium text-gray-700 mb-2">변경할 상태</label>
                <select id="batchNewStatus"
                    class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent">
                    <option value="상담대기">상담대기</option>
                    <option value="1차콜완료">1차콜완료</option>
                    <option value="진행중">진행중</option>
                    <option value="❤️승인완료❤️">❤️승인완료❤️</option>
                    <option value="부재">부재</option>
                    <option value="부결">부결</option>
                    <option value="A/S">A/S</option>
                    <option value="재컨택">재컨택</option>
                </select>
            </div>
            <div class="flex justify-end space-x-3">
                <button onclick="closeBatchModal()"
                    class="px-4 py-2 text-gray-700 bg-gray-200 rounded-lg hover:bg-gray-300 transition-colors">취소</button>
                <button onclick="updateBatchStatus()" class="btn-primary text-white px-4 py-2 rounded-lg">일괄 변경</button>
            </div>
        </div>
    </div>

    <!-- Batch Delete Modal -->
    <div id="batchDeleteModal" class="fixed inset-0 modal-overlay hidden items-center justify-center z-50">
        <div class="glass-card rounded-2xl p-6 max-w-md w-full mx-4 mobile-modal">
            <h3 class="text-lg font-semibold text-gray-900 mb-4">체크목록 삭제</h3>
            <div class="mb-4">
                <p class="text-gray-700">선택된 <span id="deleteSelectedCount" class="font-semibold text-red-600">0개</span>
                    항목을 삭제하시겠습니까?</p>
                <p class="text-sm text-red-500 mt-2">⚠️ 삭제된 데이터는 복구할 수 없습니다.</p>
            </div>
            <div class="flex justify-end space-x-3">
                <button onclick="closeBatchDeleteModal()"
                    class="px-4 py-2 text-gray-700 bg-gray-200 rounded-lg hover:bg-gray-300 transition-colors">취소</button>
                <button onclick="deleteBatchItems()"
                    class="px-4 py-2 bg-red-600 hover:bg-red-700 text-white rounded-lg transition-colors">삭제</button>
            </div>
        </div>
    </div>

    <!-- Memo Modal -->
    <div id="memoModal" class="fixed inset-0 modal-overlay hidden items-center justify-center z-50">
        <div class="glass-card rounded-2xl p-6 max-w-lg w-full mx-4 mobile-modal">
            <div class="flex items-center justify-between mb-4">
                <h3 class="text-lg font-semibold text-gray-900">메모 편집</h3>
                <button onclick="closeMemoModal()" class="text-gray-500 hover:text-gray-700">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12">
                        </path>
                    </svg>
                </button>
            </div>
            <div class="mb-4">
                <label class="block text-sm font-medium text-gray-700 mb-2">고객명</label>
                <p id="memoCustomerName" class="text-gray-900 font-semibold"></p>
            </div>
            <div class="mb-6">
                <label class="block text-sm font-medium text-gray-700 mb-2">메모</label>
                <textarea id="memoText" rows="4"
                    class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent"
                    placeholder="메모를 입력하세요..."></textarea>
            </div>
            <div class="flex justify-end space-x-3">
                <button onclick="closeMemoModal()"
                    class="px-4 py-2 text-gray-700 bg-gray-200 rounded-lg hover:bg-gray-300 transition-colors">취소</button>
                <button onclick="saveMemo()" class="btn-primary text-white px-4 py-2 rounded-lg">저장</button>
            </div>
        </div>
    </div>

    <!-- Edit Name Modal -->
    <div id="editNameModal" class="fixed inset-0 modal-overlay hidden items-center justify-center z-50">
        <div class="glass-card rounded-2xl p-6 max-w-md w-full mx-4 mobile-modal">
            <div class="flex items-center justify-between mb-4">
                <h3 class="text-lg font-semibold text-gray-900">고객명 편집</h3>
                <button onclick="closeEditNameModal()" class="text-gray-500 hover:text-gray-700">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12">
                        </path>
                    </svg>
                </button>
            </div>
            <div class="mb-6">
                <label class="block text-sm font-medium text-gray-700 mb-2">고객명</label>
                <input type="text" id="editNameInput"
                    class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent"
                    placeholder="고객명을 입력하세요">
            </div>
            <div class="flex justify-end space-x-3">
                <button onclick="closeEditNameModal()"
                    class="px-4 py-2 text-gray-700 bg-gray-200 rounded-lg hover:bg-gray-300 transition-colors">취소</button>
                <button onclick="saveEditName()" class="btn-primary text-white px-4 py-2 rounded-lg">저장</button>
            </div>
        </div>
    </div>

    <!-- Edit Phone Modal -->
    <div id="editPhoneModal" class="fixed inset-0 modal-overlay hidden items-center justify-center z-50">
        <div class="glass-card rounded-2xl p-6 max-w-md w-full mx-4 mobile-modal">
            <div class="flex items-center justify-between mb-4">
                <h3 class="text-lg font-semibold text-gray-900">연락처 편집</h3>
                <button onclick="closeEditPhoneModal()" class="text-gray-500 hover:text-gray-700">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12">
                        </path>
                    </svg>
                </button>
            </div>
            <div class="mb-6">
                <label class="block text-sm font-medium text-gray-700 mb-2">연락처</label>
                <input type="tel" id="editPhoneInput"
                    class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent"
                    placeholder="연락처를 입력하세요">
            </div>
            <div class="flex justify-end space-x-3">
                <button onclick="closeEditPhoneModal()"
                    class="px-4 py-2 text-gray-700 bg-gray-200 rounded-lg hover:bg-gray-300 transition-colors">취소</button>
                <button onclick="saveEditPhone()" class="btn-primary text-white px-4 py-2 rounded-lg">저장</button>
            </div>
        </div>
    </div>

    <!-- Edit Job Modal -->
    <div id="editJobModal" class="fixed inset-0 modal-overlay hidden items-center justify-center z-50">
        <div class="glass-card rounded-2xl p-6 max-w-md w-full mx-4 mobile-modal">
            <div class="flex items-center justify-between mb-4">
                <h3 class="text-lg font-semibold text-gray-900">직업 편집</h3>
                <button onclick="closeEditJobModal()" class="text-gray-500 hover:text-gray-700">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12">
                        </path>
                    </svg>
                </button>
            </div>
            <div class="mb-6">
                <label class="block text-sm font-medium text-gray-700 mb-2">직업</label>
                <select id="editJobSelect"
                    class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent">
                    <option value="">직업 선택</option>
                    <option value="직장인">직장인</option>
                    <option value="사업자">사업자</option>
                    <option value="프리랜서">프리랜서</option>
                </select>
            </div>
            <div class="flex justify-end space-x-3">
                <button onclick="closeEditJobModal()"
                    class="px-4 py-2 text-gray-700 bg-gray-200 rounded-lg hover:bg-gray-300 transition-colors">취소</button>
                <button onclick="saveEditJob()" class="btn-primary text-white px-4 py-2 rounded-lg">저장</button>
            </div>
        </div>
    </div>

    <!-- Edit Carrier Modal -->
    <div id="editCarrierModal" class="fixed inset-0 modal-overlay hidden items-center justify-center z-50">
        <div class="glass-card rounded-2xl p-6 max-w-md w-full mx-4 mobile-modal">
            <div class="flex items-center justify-between mb-4">
                <h3 class="text-lg font-semibold text-gray-900">통신사 편집</h3>
                <button onclick="closeEditCarrierModal()" class="text-gray-500 hover:text-gray-700">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12">
                        </path>
                    </svg>
                </button>
            </div>
            <div class="mb-6">
                <label class="block text-sm font-medium text-gray-700 mb-2">통신사</label>
                <select id="editCarrierSelect"
                    class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent">
                    <option value="">통신사 선택</option>
                    <option value="SKT">SKT</option>
                    <option value="KT">KT</option>
                    <option value="LG">LG</option>
                    <option value="SK알뜰">SK알뜰</option>
                    <option value="KT알뜰">KT알뜰</option>
                    <option value="LG알뜰">LG알뜰</option>
                </select>
            </div>
            <div class="flex justify-end space-x-3">
                <button onclick="closeEditCarrierModal()"
                    class="px-4 py-2 text-gray-700 bg-gray-200 rounded-lg hover:bg-gray-300 transition-colors">취소</button>
                <button onclick="saveEditCarrier()" class="btn-primary text-white px-4 py-2 rounded-lg">저장</button>
            </div>
        </div>
    </div>

    <!-- Edit Birth Modal -->
    <div id="editBirthModal" class="fixed inset-0 modal-overlay hidden items-center justify-center z-50">
        <div class="glass-card rounded-2xl p-6 max-w-md w-full mx-4 mobile-modal">
            <div class="flex items-center justify-between mb-4">
                <h3 class="text-lg font-semibold text-gray-900">생년월일 편집</h3>
                <button onclick="closeEditBirthModal()" class="text-gray-500 hover:text-gray-700">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12">
                        </path>
                    </svg>
                </button>
            </div>
            <div class="mb-6">
                <label class="block text-sm font-medium text-gray-700 mb-2">생년월일</label>
                <input type="text" id="editBirthInput"
                    class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-black focus:border-transparent"
                    placeholder="생년월일을 입력하세요 (예: 1990-01-01)">
            </div>
            <div class="flex justify-end space-x-3">
                <button onclick="closeEditBirthModal()"
                    class="px-4 py-2 text-gray-700 bg-gray-200 rounded-lg hover:bg-gray-300 transition-colors">취소</button>
                <button onclick="saveEditBirth()" class="btn-primary text-white px-4 py-2 rounded-lg">저장</button>
            </div>
        </div>
    </div>

    <script>
        // ===== 로그인 상태 관리 시스템 =====
        class LoginManager {
            constructor() {
                this.storageKey = 'bestron_login_state';
                this.sessionTimeout = 24 * 60 * 60 * 1000; // 24시간
            }

            setLoginState(isLoggedIn) {
                const loginData = {
                    isLoggedIn: isLoggedIn,
                    timestamp: Date.now()
                };
                localStorage.setItem(this.storageKey, JSON.stringify(loginData));
            }

            getLoginState() {
                try {
                    const stored = localStorage.getItem(this.storageKey);
                    if (!stored) return false;

                    const loginData = JSON.parse(stored);
                    const now = Date.now();
                    
                    // 세션 타임아웃 체크
                    if (now - loginData.timestamp > this.sessionTimeout) {
                        this.clearLoginState();
                        return false;
                    }

                    return loginData.isLoggedIn;
                } catch (error) {
                    console.error('로그인 상태 확인 실패:', error);
                    return false;
                }
            }

            clearLoginState() {
                localStorage.removeItem(this.storageKey);
            }

            refreshSession() {
                const loginData = {
                    isLoggedIn: true,
                    timestamp: Date.now()
                };
                localStorage.setItem(this.storageKey, JSON.stringify(loginData));
            }
        }

        // ===== 페이지네이션 시스템 =====
        class PaginationManager {
            constructor() {
                this.currentPage = 1;
                this.itemsPerPage = 20;
                this.totalItems = 0;
            }

            setItemsPerPage(items) {
                this.itemsPerPage = items;
                this.currentPage = 1; // 페이지당 항목 수 변경 시 첫 페이지로
            }

            setTotalItems(total) {
                this.totalItems = total;
            }

            getTotalPages() {
                return Math.ceil(this.totalItems / this.itemsPerPage);
            }

            getStartIndex() {
                return (this.currentPage - 1) * this.itemsPerPage;
            }

            getEndIndex() {
                return Math.min(this.getStartIndex() + this.itemsPerPage, this.totalItems);
            }

            goToPage(page) {
                const totalPages = this.getTotalPages();
                if (page >= 1 && page <= totalPages) {
                    this.currentPage = page;
                    return true;
                }
                return false;
            }

            getCurrentPageData(data) {
                const start = this.getStartIndex();
                const end = this.getEndIndex();
                return data.slice(start, start + this.itemsPerPage);
            }

            renderPagination() {
                const totalPages = this.getTotalPages();
                const pagination = document.getElementById('pagination');
                
                if (totalPages <= 1) {
                    pagination.innerHTML = '';
                    return;
                }

                let html = '';

                // 이전 페이지 버튼
                html += `<button onclick="goToPreviousPage()" ${this.currentPage === 1 ? 'disabled' : ''}>‹ 이전</button>`;

                // 페이지 번호 버튼들
                const startPage = Math.max(1, this.currentPage - 2);
                const endPage = Math.min(totalPages, this.currentPage + 2);

                if (startPage > 1) {
                    html += `<button onclick="goToPage(1)">1</button>`;
                    if (startPage > 2) {
                        html += `<span class="px-2">...</span>`;
                    }
                }

                for (let i = startPage; i <= endPage; i++) {
                    html += `<button onclick="goToPage(${i})" ${i === this.currentPage ? 'class="active"' : ''}>${i}</button>`;
                }

                if (endPage < totalPages) {
                    if (endPage < totalPages - 1) {
                        html += `<span class="px-2">...</span>`;
                    }
                    html += `<button onclick="goToPage(${totalPages})">${totalPages}</button>`;
                }

                // 다음 페이지 버튼
                html += `<button onclick="goToNextPage()" ${this.currentPage === totalPages ? 'disabled' : ''}>다음 ›</button>`;

                pagination.innerHTML = html;
            }

            updateRangeDisplay() {
                const start = this.getStartIndex() + 1;
                const end = this.getEndIndex();
                document.getElementById('currentRange').textContent = `${start}-${end}`;
                document.getElementById('totalItems').textContent = this.totalItems;
            }
        }

        // ===== 실시간 클라우드 데이터베이스 시스템 =====
        class RealTimeCloudManager {
            constructor() {
                this.db = null;
                this.modules = null;
                this.unsubscribe = null;
                this.isConnected = false;
                this.init();
            }

            async init() {
                // Firebase 초기화 대기
                if (window.firebaseDb) {
                    this.setupFirebase();
                } else {
                    window.addEventListener('firebaseReady', () => {
                        this.setupFirebase();
                    });
                }
            }

            setupFirebase() {
                this.db = window.firebaseDb;
                this.modules = window.firebaseModules;
                this.isConnected = true;
                this.updateConnectionStatus('connected');
                console.log('✅ 실시간 클라우드 데이터베이스 연결 완료');
                
                // 실시간 데이터 리스너 시작
                this.startRealtimeListener();
                
                // 초기 데이터 로드
                this.loadInitialData();
            }

            updateConnectionStatus(status) {
                const statusEl = document.getElementById('cloudStatus');
                if (!statusEl) return;

                switch(status) {
                    case 'connected':
                        statusEl.className = 'cloud-status connected';
                        statusEl.innerHTML = '<span class="realtime-indicator"></span>실시간 연결됨';
                        break;
                    case 'disconnected':
                        statusEl.className = 'cloud-status disconnected';
                        statusEl.innerHTML = '<span class="realtime-indicator" style="background:#ef4444"></span>연결 끊어짐';
                        break;
                    case 'syncing':
                        statusEl.className = 'cloud-status syncing';
                        statusEl.innerHTML = '<span class="realtime-indicator" style="background:#f59e0b"></span>동기화 중...';
                        break;
                }
            }

            async startRealtimeListener() {
                if (!this.db || !this.modules) return;

                try {
                    const { collection, onSnapshot, query, orderBy } = this.modules;
                    const consultationsRef = collection(this.db, 'consultations');
                    const q = query(consultationsRef, orderBy('dbNumber'));

                    this.unsubscribe = onSnapshot(q, (snapshot) => {
                        const cloudConsultations = [];
                        snapshot.forEach((doc) => {
                            cloudConsultations.push({
                                firebaseId: doc.id,
                                ...doc.data()
                            });
                        });

                        // 로컬 데이터와 병합
                        consultations = cloudConsultations;
                        updateConsultationList();
                        updateStats();
                        
                        console.log('📡 실시간 데이터 업데이트:', consultations.length, '건');
                    }, (error) => {
                        console.error('❌ 실시간 리스너 오류:', error);
                        this.updateConnectionStatus('disconnected');
                    });
                } catch (error) {
                    console.error('❌ 실시간 리스너 시작 실패:', error);
                    this.updateConnectionStatus('disconnected');
                }
            }

            async loadInitialData() {
                if (!this.db || !this.modules) {
                    this.loadSampleData();
                    return;
                }

                try {
                    const { collection, getDocs, query, orderBy } = this.modules;
                    const consultationsRef = collection(this.db, 'consultations');
                    const q = query(consultationsRef, orderBy('dbNumber'));
                    const snapshot = await getDocs(q);

                    const cloudConsultations = [];
                    snapshot.forEach((doc) => {
                        cloudConsultations.push({
                            firebaseId: doc.id,
                            ...doc.data()
                        });
                    });

                    if (cloudConsultations.length > 0) {
                        consultations = cloudConsultations;
                        console.log('📡 초기 클라우드 데이터 로드:', consultations.length, '건');
                    } else {
                        this.loadSampleData();
                        // 샘플 데이터를 클라우드에 저장
                        await this.uploadSampleDataToCloud();
                    }

                    updateConsultationList();
                    updateStats();
                } catch (error) {
                    console.error('❌ 초기 데이터 로드 실패:', error);
                    this.loadSampleData();
                    updateConsultationList();
                    updateStats();
                }
            }

            loadSampleData() {
                const today = new Date().toLocaleDateString('ko-KR');
                const yesterday = new Date(Date.now() - 86400000).toLocaleDateString('ko-KR');

                consultations = [
                    {
                        id: 1,
                        dbNumber: 1,
                        name: '김철수',
                        job: '직장인',
                        phone: '010-1234-5678',
                        carrier: 'SKT',
                        birthDate: '1985-03-15',
                        date: today,
                        status: '상담대기',
                        memo: '오후 3시 이후 통화 가능',
                        manager: '상현'
                    },
                    {
                        id: 2,
                        dbNumber: 2,
                        name: '박영희',
                        job: '사업자',
                        phone: '010-9876-5432',
                        carrier: 'KT',
                        birthDate: '1978-11-22',
                        date: yesterday,
                        status: '진행중',
                        memo: '서류 검토 중',
                        manager: '민성'
                    },
                    {
                        id: 3,
                        dbNumber: 3,
                        name: '이민수',
                        job: '프리랜서',
                        phone: '010-5555-7777',
                        carrier: 'LG',
                        birthDate: '1990-07-08',
                        date: today,
                        status: '❤️승인완료❤️',
                        memo: '승인 완료됨',
                        manager: '상현'
                    }
                ];
                console.log('📊 샘플 데이터 로드 완료');
            }

            async uploadSampleDataToCloud() {
                if (!this.db || !this.modules) return;

                try {
                    const { collection, addDoc } = this.modules;
                    const consultationsRef = collection(this.db, 'consultations');

                    for (const consultation of consultations) {
                        await addDoc(consultationsRef, {
                            ...consultation,
                            createdAt: new Date(),
                            updatedAt: new Date()
                        });
                    }
                    console.log('📤 샘플 데이터 클라우드 업로드 완료');
                } catch (error) {
                    console.error('❌ 샘플 데이터 업로드 실패:', error);
                }
            }

            async addConsultation(consultationData) {
                if (!this.db || !this.modules) {
                    // 오프라인 모드
                    consultations.push(consultationData);
                    return consultationData;
                }

                try {
                    this.updateConnectionStatus('syncing');
                    const { collection, addDoc } = this.modules;
                    const consultationsRef = collection(this.db, 'consultations');

                    const docRef = await addDoc(consultationsRef, {
                        ...consultationData,
                        createdAt: new Date(),
                        updatedAt: new Date()
                    });

                    console.log('📤 새 상담 클라우드 저장 완료:', docRef.id);
                    this.updateConnectionStatus('connected');
                    return { ...consultationData, firebaseId: docRef.id };
                } catch (error) {
                    console.error('❌ 상담 저장 실패:', error);
                    this.updateConnectionStatus('disconnected');
                    // 오프라인으로 폴백
                    consultations.push(consultationData);
                    return consultationData;
                }
            }

            async updateConsultation(index, updates) {
                const consultation = consultations[index];
                if (!consultation) return;

                // 로컬 업데이트
                Object.assign(consultations[index], updates);

                if (!this.db || !this.modules || !consultation.firebaseId) {
                    return;
                }

                try {
                    this.updateConnectionStatus('syncing');
                    const { doc, updateDoc } = this.modules;
                    const consultationRef = doc(this.db, 'consultations', consultation.firebaseId);

                    await updateDoc(consultationRef, {
                        ...updates,
                        updatedAt: new Date()
                    });

                    console.log('📤 상담 정보 클라우드 업데이트 완료');
                    this.updateConnectionStatus('connected');
                } catch (error) {
                    console.error('❌ 상담 업데이트 실패:', error);
                    this.updateConnectionStatus('disconnected');
                }
            }

            async deleteConsultations(indices) {
                if (!this.db || !this.modules) {
                    // 오프라인 모드
                    indices.sort((a, b) => b - a).forEach(index => {
                        consultations.splice(index, 1);
                    });
                    return;
                }

                try {
                    this.updateConnectionStatus('syncing');
                    const { doc, deleteDoc } = this.modules;

                    for (const index of indices.sort((a, b) => b - a)) {
                        const consultation = consultations[index];
                        if (consultation && consultation.firebaseId) {
                            const consultationRef = doc(this.db, 'consultations', consultation.firebaseId);
                            await deleteDoc(consultationRef);
                        }
                        consultations.splice(index, 1);
                    }

                    console.log('📤 상담 삭제 클라우드 동기화 완료');
                    this.updateConnectionStatus('connected');
                } catch (error) {
                    console.error('❌ 상담 삭제 실패:', error);
                    this.updateConnectionStatus('disconnected');
                }
            }

            async uploadBulkData(consultationsData) {
                if (!this.db || !this.modules) {
                    consultations.push(...consultationsData);
                    return;
                }

                try {
                    this.updateConnectionStatus('syncing');
                    const { collection, addDoc } = this.modules;
                    const consultationsRef = collection(this.db, 'consultations');

                    for (const consultation of consultationsData) {
                        await addDoc(consultationsRef, {
                            ...consultation,
                            createdAt: new Date(),
                            updatedAt: new Date()
                        });
                    }

                    console.log('📤 대량 데이터 클라우드 업로드 완료:', consultationsData.length, '건');
                    this.updateConnectionStatus('connected');
                } catch (error) {
                    console.error('❌ 대량 업로드 실패:', error);
                    this.updateConnectionStatus('disconnected');
                    // 오프라인으로 폴백
                    consultations.push(...consultationsData);
                }
            }

            disconnect() {
                if (this.unsubscribe) {
                    this.unsubscribe();
                }
                this.isConnected = false;
                this.updateConnectionStatus('disconnected');
            }
        }

        // 전역 변수들
        let consultations = [];
        let currentEditIndex = -1;
        let currentCategory = 'all';
        let selectedItems = new Set();
        let currentMemoIndex = -1;
        let currentEditNameIndex = -1;
        let currentEditPhoneIndex = -1;
        let currentEditJobIndex = -1;
        let currentEditCarrierIndex = -1;
        let currentEditBirthIndex = -1;
        let searchTerm = '';

        // 매니저 인스턴스들
        let cloudManager;
        let loginManager;
        let paginationManager;

        const statusStyles = {
            '상담대기': 'status-waiting',
            '1차콜완료': 'status-first-call',
            '진행중': 'status-in-progress',
            '❤️승인완료❤️': 'status-approved',
            '부재': 'status-absent',
            '부결': 'status-rejected',
            'A/S': 'status-as',
            '재컨택': 'status-recontact'
        };

        // DOM 로드 완료 시 초기화
        document.addEventListener('DOMContentLoaded', function() {
            loginManager = new LoginManager();
            paginationManager = new PaginationManager();
            cloudManager = new RealTimeCloudManager();
            
            // 로그인 상태 확인
            checkLoginState();
            
            console.log('🚀 베스트론 실시간 클라우드 시스템 시작');
        });

        // 페이지 로드 시 새로고침 상태 확인
        function checkLoginState() {
            if (loginManager.getLoginState()) {
                // 로그인 상태 유지
                document.getElementById('loginScreen').classList.add('hidden');
                document.getElementById('mainApp').classList.remove('hidden');
                initializeApp();
                console.log('✅ 로그인 상태 유지됨');
            } else {
                // 로그인 화면 표시
                document.getElementById('loginScreen').classList.remove('hidden');
                document.getElementById('mainApp').classList.add('hidden');
            }
        }

        // 페이지네이션 함수들
        function changeItemsPerPage() {
            const select = document.getElementById('itemsPerPage');
            paginationManager.setItemsPerPage(parseInt(select.value));
            updateConsultationList();
        }

        function goToPage(page) {
            if (paginationManager.goToPage(page)) {
                updateConsultationList();
                clearSelection();
            }
        }

        function goToPreviousPage() {
            goToPage(paginationManager.currentPage - 1);
        }

        function goToNextPage() {
            goToPage(paginationManager.currentPage + 1);
        }

        // 기존 함수들 (로그인 상태 관리 추가)
        function handleLogin(event) {
            event.preventDefault();
            const id = document.getElementById('loginId').value;
            const password = document.getElementById('loginPassword').value;

            if (id === 'best101' && password === 'best101') {
                // 로그인 상태 저장
                loginManager.setLoginState(true);
                
                document.getElementById('loginScreen').classList.add('hidden');
                document.getElementById('mainApp').classList.remove('hidden');
                initializeApp();
                
                console.log('✅ 로그인 성공 - 상태 저장됨');
            } else {
                alert('아이디 또는 비밀번호가 올바르지 않습니다.');
            }
        }

        function logout() {
            if (confirm('로그아웃 하시겠습니까?')) {
                // 로그인 상태 삭제
                loginManager.clearLoginState();
                
                // 클라우드 연결 해제
                if (cloudManager) {
                    cloudManager.disconnect();
                }
                
                document.getElementById('mainApp').classList.add('hidden');
                document.getElementById('loginScreen').classList.remove('hidden');
                document.getElementById('loginId').value = '';
                document.getElementById('loginPassword').value = '';
                
                console.log('✅ 로그아웃 완료');
            }
        }

        function initializeApp() {
            // 세션 갱신
            loginManager.refreshSession();
            updateConsultationList();
            updateStats();
        }

        function toggleRegistration() {
            document.getElementById('registrationModal').classList.remove('hidden');
            document.getElementById('registrationModal').classList.add('flex');
        }

        function closeRegistration() {
            document.getElementById('registrationModal').classList.add('hidden');
            document.getElementById('registrationModal').classList.remove('flex');
        }

        function toggleManualInput() {
            const section = document.getElementById('manualInputSection');
            const icon = document.getElementById('toggleIcon');

            if (section.classList.contains('hidden')) {
                section.classList.remove('hidden');
                icon.style.transform = 'rotate(180deg)';
            } else {
                section.classList.add('hidden');
                icon.style.transform = 'rotate(0deg)';
            }
        }

        async function addConsultation() {
            const name = document.getElementById('customerName').value.trim();
            const job = document.getElementById('customerJob').value;
            const phone = document.getElementById('customerPhone').value.trim();
            const carrier = document.getElementById('customerCarrier').value;
            const birthDate = document.getElementById('birthDate').value.trim();

            if (!name || !job || !phone || !carrier || !birthDate) {
                alert('모든 항목을 입력해주세요.');
                return;
            }

            const newDbNumber = consultations.length > 0 ? Math.max(...consultations.map(c => c.dbNumber || 0)) + 1 : 1;

            const consultation = {
                id: Date.now(),
                dbNumber: newDbNumber,
                name: name,
                job: job,
                phone: phone,
                carrier: carrier,
                birthDate: birthDate,
                date: new Date().toLocaleDateString('ko-KR'),
                status: '상담대기',
                memo: '',
                manager: ''
            };

            // 클라우드에 저장
            await cloudManager.addConsultation(consultation);

            // Clear form
            document.getElementById('customerName').value = '';
            document.getElementById('customerJob').value = '';
            document.getElementById('customerPhone').value = '';
            document.getElementById('customerCarrier').value = '';
            document.getElementById('birthDate').value = '';

            alert('상담이 성공적으로 등록되었습니다.');
        }

        function handleFileUpload(event) {
            const file = event.target.files[0];
            if (!file) return;

            const reader = new FileReader();
            reader.onload = function (e) {
                try {
                    const data = new Uint8Array(e.target.result);
                    const workbook = XLSX.read(data, {type: 'array'});
                    const firstSheetName = workbook.SheetNames[0];
                    const worksheet = workbook.Sheets[firstSheetName];
                    const jsonData = XLSX.utils.sheet_to_json(worksheet, {header: 1});

                    processExcelData(jsonData);
                } catch (error) {
                    alert('파일을 읽는 중 오류가 발생했습니다: ' + error.message);
                }
            };
            reader.readAsArrayBuffer(file);
        }

        async function processExcelData(data) {
            if (data.length < 2) {
                alert('데이터가 충분하지 않습니다. 헤더와 최소 1개의 데이터 행이 필요합니다.');
                return;
            }

            const headers = data[0].map(header => {
                if (!header) return '';
                return header.toString().trim();
            });
            
            const nameKeywords = ['고객명', '이름', '성명', 'name', '고객이름', '성함', '신청자', '신청인'];
            const phoneKeywords = ['연락처', '전화번호', '휴대폰', '전화', 'phone', 'mobile', 'tel', '핸드폰'];
            const jobKeywords = ['직업', 'job', 'occupation', '업무', '직무'];
            const carrierKeywords = ['통신사', 'carrier', '통신', '이동통신사'];
            const birthKeywords = ['생년월일', '생일', 'birth', 'birthday', '년월일'];

            function findColumnIndex(keywords) {
                for (let i = 0; i < headers.length; i++) {
                    const header = headers[i].toLowerCase().replace(/[\s\-_\.]/g, '');
                    for (let keyword of keywords) {
                        const cleanKeyword = keyword.toLowerCase().replace(/[\s\-_\.]/g, '');
                        if (header === cleanKeyword || header.includes(cleanKeyword)) {
                            return i;
                        }
                    }
                }
                return -1;
            }

            let nameIndex = findColumnIndex(nameKeywords);
            let phoneIndex = findColumnIndex(phoneKeywords);
            let jobIndex = findColumnIndex(jobKeywords);
            let carrierIndex = findColumnIndex(carrierKeywords);
            let birthIndex = findColumnIndex(birthKeywords);

            if (nameIndex === -1 || phoneIndex === -1) {
                alert('필수 컬럼(고객명, 연락처)을 찾을 수 없습니다.');
                return;
            }

            function normalizePhoneNumber(phone) {
                if (!phone) return '';
                const numbersOnly = phone.toString().replace(/[^0-9]/g, '');
                if (numbersOnly.length === 11 && numbersOnly.startsWith('010')) {
                    return numbersOnly.replace(/(\d{3})(\d{4})(\d{4})/, '$1-$2-$3');
                }
                return numbersOnly;
            }

            let successCount = 0;
            let errorCount = 0;
            const today = new Date().toLocaleDateString('ko-KR');
            const maxDbNumber = consultations.length > 0 ? Math.max(...consultations.map(c => c.dbNumber || 0)) : 0;
            const newConsultations = [];

            for (let i = 1; i < data.length; i++) {
                const row = data[i];
                if (!row || row.length === 0) continue;

                const name = row[nameIndex]?.toString().trim();
                const job = jobIndex >= 0 ? (row[jobIndex]?.toString().trim() || '') : '';
                let phone = row[phoneIndex]?.toString().trim();
                const carrier = carrierIndex >= 0 ? (row[carrierIndex]?.toString().trim() || '') : '';
                const birthDate = birthIndex >= 0 ? (row[birthIndex]?.toString().trim() || '') : '';

                phone = normalizePhoneNumber(phone);

                if (name && phone) {
                    const isDuplicate = consultations.some(c =>
                        c.name === name && c.phone === phone
                    );

                    if (!isDuplicate) {
                        const consultation = {
                            id: Date.now() + i + Math.random() * 1000,
                            dbNumber: maxDbNumber + successCount + 1,
                            name: name,
                            job: job,
                            phone: phone,
                            carrier: carrier,
                            birthDate: birthDate,
                            date: today,
                            status: '상담대기',
                            memo: '',
                            manager: ''
                        };
                        newConsultations.push(consultation);
                        successCount++;
                    }
                } else {
                    errorCount++;
                }
            }

            // 대량 데이터 클라우드 업로드
            if (newConsultations.length > 0) {
                await cloudManager.uploadBulkData(newConsultations);
            }

            let message = `엑셀 업로드가 완료되었습니다!\n\n성공: ${successCount}건 등록`;
            if (errorCount > 0) {
                message += `\n실패/중복: ${errorCount}건`;
            }
            alert(message);

            event.target.value = '';
            closeRegistration();
        }

        function downloadBackup() {
            if (consultations.length === 0) {
                alert('백업할 데이터가 없습니다.');
                return;
            }

            // DB번호 순으로 정렬
            const sortedConsultations = [...consultations].sort((a, b) => (a.dbNumber || 0) - (b.dbNumber || 0));

            const excelData = sortedConsultations.map(consultation => ({
                'DB번호': consultation.dbNumber || '',
                '고객명': consultation.name || '',
                '생년월일': consultation.birthDate || '',
                '직업': consultation.job || '',
                '연락처': consultation.phone || '',
                '통신사': consultation.carrier || '',
                '메모': consultation.memo || '',
                '상담상태': consultation.status || '',
                '담당자': consultation.manager || '',
                '등록일': consultation.date || ''
            }));

            const wb = XLSX.utils.book_new();
            const ws = XLSX.utils.json_to_sheet(excelData);
            
            const colWidths = [
                {wch: 8}, {wch: 12}, {wch: 12}, {wch: 10}, {wch: 15}, 
                {wch: 10}, {wch: 20}, {wch: 12}, {wch: 10}, {wch: 12}
            ];
            ws['!cols'] = colWidths;

            XLSX.utils.book_append_sheet(wb, ws, '상담데이터');
            
            const fileName = `베스트론_백업_${new Date().toISOString().split('T')[0].replace(/-/g, '')}.xlsx`;
            XLSX.writeFile(wb, fileName);
            
            alert('Excel 백업 파일이 다운로드되었습니다.');
        }

        function handleSearch(event) {
            searchTerm = event.target.value.toLowerCase().trim();
            paginationManager.currentPage = 1; // 검색 시 첫 페이지로
            updateConsultationList();
        }

        function clearSearch() {
            document.getElementById('searchInput').value = '';
            searchTerm = '';
            paginationManager.currentPage = 1; // 검색 초기화 시 첫 페이지로
            updateConsultationList();
        }

        function filterConsultations() {
            let filtered = consultations;

            if (currentCategory !== 'all') {
                filtered = filtered.filter(c => c.status === currentCategory);
            }

            if (searchTerm) {
                filtered = filtered.filter(c => {
                    const nameMatch = c.name.toLowerCase().includes(searchTerm);
                    const phoneMatch = c.phone.replace(/-/g, '').includes(searchTerm.replace(/-/g, ''));
                    return nameMatch || phoneMatch;
                });
            }

            return filtered;
        }

        function showCategory(category) {
            currentCategory = category;
            paginationManager.currentPage = 1; // 카테고리 변경 시 첫 페이지로

            document.querySelectorAll('.category-tab').forEach(tab => {
                tab.classList.remove('active');
            });
            document.querySelector(`[data-category="${category}"]`).classList.add('active');

            updateConsultationList();
            clearSelection();
        }

        function updateConsultationList() {
            const tbody = document.getElementById('consultationList');
            tbody.innerHTML = '';

            const filteredConsultations = filterConsultations();
            
            // DB번호 순으로 정렬
            filteredConsultations.sort((a, b) => (a.dbNumber || 0) - (b.dbNumber || 0));
            
            // 페이지네이션 설정
            paginationManager.setTotalItems(filteredConsultations.length);
            const currentPageData = paginationManager.getCurrentPageData(filteredConsultations);

            // 페이지네이션 UI 업데이트
            paginationManager.renderPagination();
            paginationManager.updateRangeDisplay();

            currentPageData.forEach((consultation) => {
                const globalIndex = consultations.findIndex(c => c.id === consultation.id);
                const row = document.createElement('tr');
                row.className = 'table-row';

                const memoDisplay = consultation.memo ?
                    `<span class="text-blue-600 font-medium">${consultation.memo.length > 8 ? consultation.memo.substring(0, 8) + '...' : consultation.memo}</span>` :
                    '<span class="text-gray-400">메모없음</span>';

                const jobDisplay = consultation.job ?
                    `<span class="text-gray-900">${consultation.job}</span>` :
                    '<span class="text-gray-400">미지정</span>';

                const carrierDisplay = consultation.carrier ?
                    `<span class="text-gray-900">${consultation.carrier}</span>` :
                    '<span class="text-gray-400">미지정</span>';

                const birthDisplay = consultation.birthDate ?
                    `<span class="text-gray-900">${consultation.birthDate}</span>` :
                    '<span class="text-gray-400">미입력</span>';

                row.innerHTML = `
            <td>
                <input type="checkbox" class="checkbox-custom" onchange="toggleSelection(${globalIndex})" ${selectedItems.has(globalIndex) ? 'checked' : ''}>
            </td>
            <td class="text-sm font-medium text-gray-900">
                ${consultation.dbNumber || '-'}
            </td>
            <td class="text-sm font-medium">
                <button onclick="openEditNameModal(${globalIndex})" class="editable-field text-gray-900 hover:text-blue-600 font-medium">
                    ${consultation.name}
                </button>
            </td>
            <td class="text-sm">
                <button onclick="openEditBirthModal(${globalIndex})" class="editable-field text-gray-700 hover:text-blue-600">
                    ${birthDisplay}
                </button>
            </td>
            <td class="text-sm">
                <button onclick="openEditJobModal(${globalIndex})" class="editable-field text-gray-700 hover:text-blue-600">
                    ${jobDisplay}
                </button>
            </td>
            <td class="text-sm">
                <button onclick="openEditPhoneModal(${globalIndex})" class="editable-field text-gray-700 hover:text-blue-600">
                    ${consultation.phone}
                </button>
            </td>
            <td class="text-sm">
                <button onclick="openEditCarrierModal(${globalIndex})" class="editable-field text-gray-700 hover:text-blue-600">
                    ${carrierDisplay}
                </button>
            </td>
            <td class="text-sm">
                <button onclick="openMemoModal(${globalIndex})" class="text-purple-600 hover:text-purple-800 transition-colors font-medium">
                    ${memoDisplay}
                </button>
            </td>
            <td>
                <select class="status-select px-1 py-0 rounded text-xs font-medium ${statusStyles[consultation.status]}" 
                        onchange="changeStatusDirect(${globalIndex}, this.value)">
                    <option value="상담대기" ${consultation.status === '상담대기' ? 'selected' : ''}>상담대기</option>
                    <option value="1차콜완료" ${consultation.status === '1차콜완료' ? 'selected' : ''}>1차콜완료</option>
                    <option value="진행중" ${consultation.status === '진행중' ? 'selected' : ''}>진행중</option>
                    <option value="❤️승인완료❤️" ${consultation.status === '❤️승인완료❤️' ? 'selected' : ''}>❤️승인완료❤️</option>
                    <option value="부재" ${consultation.status === '부재' ? 'selected' : ''}>부재</option>
                    <option value="부결" ${consultation.status === '부결' ? 'selected' : ''}>부결</option>
                    <option value="A/S" ${consultation.status === 'A/S' ? 'selected' : ''}>A/S</option>
                    <option value="재컨택" ${consultation.status === '재컨택' ? 'selected' : ''}>재컨택</option>
                </select>
            </td>
            <td>
                <select class="manager-select text-sm text-gray-700" 
                        onchange="changeManagerDirect(${globalIndex}, this.value)">
                    <option value="" ${!consultation.manager ? 'selected' : ''}>미지정</option>
                    <option value="상현" ${consultation.manager === '상현' ? 'selected' : ''}>상현</option>
                    <option value="민성" ${consultation.manager === '민성' ? 'selected' : ''}>민성</option>
                </select>
            </td>
            <td class="text-sm text-gray-700">${consultation.date}</td>
        `;
                tbody.appendChild(row);
            });
        }

        async function changeStatusDirect(index, newStatus) {
            const oldStatus = consultations[index].status;

            if (newStatus !== oldStatus) {
                await cloudManager.updateConsultation(index, { status: newStatus });
                updateConsultationList();
                updateStats();

                const selectElement = event.target;
                selectElement.className = `status-select px-1 py-0 rounded text-xs font-medium ${statusStyles[newStatus]}`;
            }
        }

        async function changeManagerDirect(index, newManager) {
            await cloudManager.updateConsultation(index, { manager: newManager });
        }

        function openEditJobModal(index) {
            currentEditJobIndex = index;
            const consultation = consultations[index];
            document.getElementById('editJobSelect').value = consultation.job || '';
            document.getElementById('editJobModal').classList.remove('hidden');
            document.getElementById('editJobModal').classList.add('flex');
        }

        function closeEditJobModal() {
            document.getElementById('editJobModal').classList.add('hidden');
            document.getElementById('editJobModal').classList.remove('flex');
            currentEditJobIndex = -1;
        }

        async function saveEditJob() {
            if (currentEditJobIndex === -1) return;

            const newJob = document.getElementById('editJobSelect').value;
            await cloudManager.updateConsultation(currentEditJobIndex, { job: newJob });
            updateConsultationList();
            closeEditJobModal();
            alert('직업이 수정되었습니다.');
        }

        function openEditCarrierModal(index) {
            currentEditCarrierIndex = index;
            const consultation = consultations[index];
            document.getElementById('editCarrierSelect').value = consultation.carrier || '';
            document.getElementById('editCarrierModal').classList.remove('hidden');
            document.getElementById('editCarrierModal').classList.add('flex');
        }

        function closeEditCarrierModal() {
            document.getElementById('editCarrierModal').classList.add('hidden');
            document.getElementById('editCarrierModal').classList.remove('flex');
            currentEditCarrierIndex = -1;
        }

        async function saveEditCarrier() {
            if (currentEditCarrierIndex === -1) return;

            const newCarrier = document.getElementById('editCarrierSelect').value;
            await cloudManager.updateConsultation(currentEditCarrierIndex, { carrier: newCarrier });
            updateConsultationList();
            closeEditCarrierModal();
            alert('통신사가 수정되었습니다.');
        }

        function openEditNameModal(index) {
            currentEditNameIndex = index;
            const consultation = consultations[index];
            document.getElementById('editNameInput').value = consultation.name;
            document.getElementById('editNameModal').classList.remove('hidden');
            document.getElementById('editNameModal').classList.add('flex');
        }

        function closeEditNameModal() {
            document.getElementById('editNameModal').classList.add('hidden');
            document.getElementById('editNameModal').classList.remove('flex');
            currentEditNameIndex = -1;
        }

        async function saveEditName() {
            if (currentEditNameIndex === -1) return;

            const newName = document.getElementById('editNameInput').value.trim();
            if (!newName) {
                alert('고객명을 입력해주세요.');
                return;
            }

            await cloudManager.updateConsultation(currentEditNameIndex, { name: newName });
            updateConsultationList();
            closeEditNameModal();
            alert('고객명이 수정되었습니다.');
        }

        function openEditPhoneModal(index) {
            currentEditPhoneIndex = index;
            const consultation = consultations[index];
            document.getElementById('editPhoneInput').value = consultation.phone;
            document.getElementById('editPhoneModal').classList.remove('hidden');
            document.getElementById('editPhoneModal').classList.add('flex');
        }

        function closeEditPhoneModal() {
            document.getElementById('editPhoneModal').classList.add('hidden');
            document.getElementById('editPhoneModal').classList.remove('flex');
            currentEditPhoneIndex = -1;
        }

        async function saveEditPhone() {
            if (currentEditPhoneIndex === -1) return;

            const newPhone = document.getElementById('editPhoneInput').value.trim();
            if (!newPhone) {
                alert('연락처를 입력해주세요.');
                return;
            }

            await cloudManager.updateConsultation(currentEditPhoneIndex, { phone: newPhone });
            updateConsultationList();
            closeEditPhoneModal();
            alert('연락처가 수정되었습니다.');
        }

        function openEditBirthModal(index) {
            currentEditBirthIndex = index;
            const consultation = consultations[index];
            document.getElementById('editBirthInput').value = consultation.birthDate || '';
            document.getElementById('editBirthModal').classList.remove('hidden');
            document.getElementById('editBirthModal').classList.add('flex');
        }

        function closeEditBirthModal() {
            document.getElementById('editBirthModal').classList.add('hidden');
            document.getElementById('editBirthModal').classList.remove('flex');
            currentEditBirthIndex = -1;
        }

        async function saveEditBirth() {
            if (currentEditBirthIndex === -1) return;

            const newBirth = document.getElementById('editBirthInput').value.trim();
            await cloudManager.updateConsultation(currentEditBirthIndex, { birthDate: newBirth });
            updateConsultationList();
            closeEditBirthModal();
            alert('생년월일이 수정되었습니다.');
        }

        function toggleSelection(index) {
            if (selectedItems.has(index)) {
                selectedItems.delete(index);
            } else {
                selectedItems.add(index);
            }
            updateSelectionUI();
        }

        function toggleSelectAll() {
            const selectAllCheckbox = document.getElementById('selectAll');

            if (selectAllCheckbox.checked) {
                const filteredConsultations = filterConsultations();
                filteredConsultations.forEach(consultation => {
                    const globalIndex = consultations.findIndex(c => c.id === consultation.id);
                    selectedItems.add(globalIndex);
                });

                const checkboxes = document.querySelectorAll('#consultationList input[type="checkbox"]');
                checkboxes.forEach(checkbox => checkbox.checked = true);
            } else {
                selectedItems.clear();
                const checkboxes = document.querySelectorAll('#consultationList input[type="checkbox"]');
                checkboxes.forEach(checkbox => checkbox.checked = false);
            }

            updateSelectionUI();
        }

        function clearSelection() {
            selectedItems.clear();
            document.getElementById('selectAll').checked = false;
            const checkboxes = document.querySelectorAll('#consultationList input[type="checkbox"]');
            checkboxes.forEach(checkbox => checkbox.checked = false);
            updateSelectionUI();
        }

        function updateSelectionUI() {
            const selectedCount = selectedItems.size;
            document.getElementById('selectedCount').textContent = selectedCount;

            const batchBtn = document.getElementById('batchStatusBtn');
            const deleteBtn = document.getElementById('batchDeleteBtn');
            const batchBtnMobile = document.getElementById('batchStatusBtnMobile');
            const deleteBtnMobile = document.getElementById('batchDeleteBtnMobile');

            const buttons = [batchBtn, deleteBtn, batchBtnMobile, deleteBtnMobile].filter(btn => btn);

            buttons.forEach(btn => {
                if (selectedCount > 0) {
                    btn.disabled = false;
                    btn.classList.remove('opacity-50', 'cursor-not-allowed');
                } else {
                    btn.disabled = true;
                    btn.classList.add('opacity-50', 'cursor-not-allowed');
                }
            });
        }

        function updateStats() {
            const total = consultations.length;
            const progress = consultations.filter(c => c.status === '진행중').length;
            const approved = consultations.filter(c => c.status === '❤️승인완료❤️').length;

            document.getElementById('totalCount').textContent = total;
            document.getElementById('progressCount').textContent = progress;
            document.getElementById('approvedCount').textContent = approved;
        }

        function openMemoModal(index) {
            currentMemoIndex = index;
            const consultation = consultations[index];
            document.getElementById('memoCustomerName').textContent = consultation.name;
            document.getElementById('memoText').value = consultation.memo || '';
            document.getElementById('memoModal').classList.remove('hidden');
            document.getElementById('memoModal').classList.add('flex');
        }

        function closeMemoModal() {
            document.getElementById('memoModal').classList.add('hidden');
            document.getElementById('memoModal').classList.remove('flex');
            currentMemoIndex = -1;
        }

        async function saveMemo() {
            if (currentMemoIndex === -1) return;

            const memoText = document.getElementById('memoText').value.trim();
            await cloudManager.updateConsultation(currentMemoIndex, { memo: memoText });
            updateConsultationList();
            closeMemoModal();
            alert('메모가 저장되었습니다.');
        }

        function openBatchStatusModal() {
            if (selectedItems.size === 0) return;

            document.getElementById('batchSelectedCount').textContent = `${selectedItems.size}개`;
            document.getElementById('batchStatusModal').classList.remove('hidden');
            document.getElementById('batchStatusModal').classList.add('flex');
        }

        function closeBatchModal() {
            document.getElementById('batchStatusModal').classList.add('hidden');
            document.getElementById('batchStatusModal').classList.remove('flex');
        }

        async function updateBatchStatus() {
            const newStatus = document.getElementById('batchNewStatus').value;
            let changeCount = 0;

            for (const index of selectedItems) {
                if (consultations[index].status !== newStatus) {
                    await cloudManager.updateConsultation(index, { status: newStatus });
                    changeCount++;
                }
            }

            updateConsultationList();
            updateStats();
            clearSelection();
            closeBatchModal();

            alert(`${changeCount}개 항목의 상태가 "${newStatus}"로 변경되었습니다.`);
        }

        function openBatchDeleteModal() {
            if (selectedItems.size === 0) return;

            document.getElementById('deleteSelectedCount').textContent = `${selectedItems.size}개`;
            document.getElementById('batchDeleteModal').classList.remove('hidden');
            document.getElementById('batchDeleteModal').classList.add('flex');
        }

        function closeBatchDeleteModal() {
            document.getElementById('batchDeleteModal').classList.add('hidden');
            document.getElementById('batchDeleteModal').classList.remove('flex');
        }

        async function deleteBatchItems() {
            const selectedIndices = Array.from(selectedItems);
            const deleteCount = selectedIndices.length;

            await cloudManager.deleteConsultations(selectedIndices);

            selectedItems.clear();
            updateConsultationList();
            updateStats();
            updateSelectionUI();
            closeBatchDeleteModal();

            alert(`${deleteCount}개 항목이 성공적으로 삭제되었습니다.`);
        }

        // 자동 세션 갱신 (5분마다)
        setInterval(() => {
            if (loginManager.getLoginState()) {
                loginManager.refreshSession();
            }
        }, 5 * 60 * 1000); // 5분

        // 모달 외부 클릭시 닫기
        document.addEventListener('click', function(e) {
            if (e.target.classList.contains('modal-overlay')) {
                // 모든 모달 닫기
                const modals = [
                    'batchStatusModal', 'batchDeleteModal', 
                    'registrationModal', 'memoModal',
                    'editNameModal', 'editPhoneModal', 'editJobModal', 
                    'editCarrierModal', 'editBirthModal'
                ];
                
                modals.forEach(modalId => {
                    const modal = document.getElementById(modalId);
                    if (modal && !modal.classList.contains('hidden')) {
                        modal.classList.add('hidden');
                        modal.classList.remove('flex');
                    }
                });
                
                // 현재 편집 인덱스들 초기화
                currentEditIndex = -1;
                currentMemoIndex = -1;
                currentEditNameIndex = -1;
                currentEditPhoneIndex = -1;
                currentEditJobIndex = -1;
                currentEditCarrierIndex = -1;
                currentEditBirthIndex = -1;
            }
        });

        // 페이지 언로드 시 클라우드 연결 해제
        window.addEventListener('beforeunload', () => {
            if (cloudManager) {
                cloudManager.disconnect();
            }
        });

        // 초기화
        updateSelectionUI();
    </script>
</body>

</html>
