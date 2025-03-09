---
title: "Dashboard"
date: 2025-03-09
draft: false
---
    <script src="https://cdn.tailwindcss.com"></script>
    <div class="max-w-6xl mx-auto">
        <h1 class="text-3xl font-bold mb-6">Dashboard</h1>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
            <div class="bg-white p-4 rounded-lg shadow">
                <h2 class="text-lg font-semibold">Utenti </h2>
                <iframe src="/utenti.html" class="w-full h-32"></iframe>
            </div>
            <div class="bg-white p-4 rounded-lg shadow">
                <h2 class="text-lg font-semibold">Libri Prestati</h2>
                <iframe src="/prestiti.html" class="w-full h-32"></iframe>
            </div>
            <div class="bg-white p-4 rounded-lg shadow">
                <h2 class="text-lg font-semibold">Libri Disponibili</h2>
                <iframe src="/disponibili.html" class="w-full h-32"></iframe>
            </div>
            <div class="bg-white p-4 rounded-lg shadow">
                <h2 class="text-lg font-semibold">Eventi Programmati</h2>
                <iframe src="/eventi.html" class="w-full h-32"></iframe>
            </div>
        </div>
    </div>
    
    <script>
        if (!document.cookie.includes("nf_jwt")) {
            window.location.href = "/.netlify/identity/login";
        }
    </script>
