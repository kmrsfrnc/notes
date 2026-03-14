<template>
  <div class="min-h-screen bg-neutral-50 dark:bg-neutral-950 text-neutral-900 dark:text-neutral-100 selection:bg-indigo-500/30 font-sans transition-colors duration-300">
    <VitePwaManifest />
    
    <!-- Background decorations -->
    <div class="fixed inset-0 overflow-hidden pointer-events-none z-0">
      <div class="absolute -top-40 -right-40 w-96 h-96 bg-indigo-500/10 dark:bg-indigo-500/5 rounded-full blur-3xl"></div>
      <div class="absolute top-[40%] -left-40 w-[30rem] h-[30rem] bg-rose-500/10 dark:bg-rose-500/5 rounded-full blur-3xl"></div>
    </div>

    <div class="relative z-10 flex flex-col items-center justify-center min-h-screen p-6 sm:p-12">
      
      <!-- Hero Section -->
      <div class="text-center max-w-2xl w-full space-y-8 animate-fade-in-up">
        
        <div class="inline-flex items-center justify-center w-24 h-24 mb-6 rounded-3xl bg-white dark:bg-neutral-900 shadow-xl shadow-indigo-500/10 ring-1 ring-neutral-200 dark:ring-neutral-800 backdrop-blur-sm">
          <svg class="w-12 h-12 text-indigo-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-4l-4 4m0 0l-4-4m4 4V4" />
          </svg>
        </div>
        
        <div class="space-y-4">
          <h1 class="text-4xl sm:text-5xl font-extrabold tracking-tight bg-clip-text text-transparent bg-gradient-to-br from-indigo-500 to-rose-500">
            Install this App
          </h1>
          <p class="text-lg text-neutral-600 dark:text-neutral-400">
            Experience our application in full screen by installing it directly to your home screen. Fast, responsive, and always ready.
          </p>
        </div>

        <!-- Installation Instructions Cards -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mt-12 text-left">
          
          <!-- iOS Card -->
          <div class="group relative bg-white/60 dark:bg-neutral-900/60 backdrop-blur-md rounded-3xl p-8 shadow-sm hover:shadow-xl hover:shadow-indigo-500/10 ring-1 ring-neutral-200/50 dark:ring-neutral-800/50 transition-all duration-300">
            <div class="absolute inset-0 bg-gradient-to-br from-indigo-500/5 to-transparent opacity-0 group-hover:opacity-100 rounded-3xl transition-opacity duration-300"></div>
            <div class="relative">
              <div class="flex items-center gap-4 mb-6">
                <div class="flex items-center justify-center w-12 h-12 rounded-2xl bg-neutral-100 dark:bg-neutral-800 text-neutral-900 dark:text-white">
                  <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M12 2C6.477 2 2 6.477 2 12c0 4.991 3.657 9.128 8.438 9.878v-6.987h-2.54V12h2.54V9.797c0-2.506 1.492-3.89 3.777-3.89 1.094 0 2.238.195 2.238.195v2.46h-1.26c-1.243 0-1.63.771-1.63 1.562V12h2.773l-.443 2.89h-2.33v6.988C18.343 21.128 22 16.991 22 12c0-5.523-4.477-10-10-10z" />
                  </svg>
                </div>
                <h2 class="text-2xl font-bold">iOS / Safari</h2>
              </div>
              <ul class="space-y-4 text-neutral-600 dark:text-neutral-400">
                <li class="flex items-start gap-3">
                  <span class="flex items-center justify-center w-6 h-6 rounded-full bg-indigo-100 dark:bg-indigo-900/50 text-indigo-600 dark:text-indigo-400 text-sm font-semibold shrink-0 mt-0.5">1</span>
                  <span>Tap the <strong class="text-neutral-900 dark:text-white">Share</strong> button at the bottom of the screen.</span>
                </li>
                <li class="flex items-start gap-3">
                  <span class="flex items-center justify-center w-6 h-6 rounded-full bg-indigo-100 dark:bg-indigo-900/50 text-indigo-600 dark:text-indigo-400 text-sm font-semibold shrink-0 mt-0.5">2</span>
                  <span>Scroll down and tap <strong class="text-neutral-900 dark:text-white">"Add to Home Screen"</strong>.</span>
                </li>
                <li class="flex items-start gap-3">
                  <span class="flex items-center justify-center w-6 h-6 rounded-full bg-indigo-100 dark:bg-indigo-900/50 text-indigo-600 dark:text-indigo-400 text-sm font-semibold shrink-0 mt-0.5">3</span>
                  <span>Tap <strong class="text-neutral-900 dark:text-white">Add</strong> in the top right corner.</span>
                </li>
              </ul>
            </div>
          </div>

          <!-- Android Card -->
          <div class="group relative bg-white/60 dark:bg-neutral-900/60 backdrop-blur-md rounded-3xl p-8 shadow-sm hover:shadow-xl hover:shadow-rose-500/10 ring-1 ring-neutral-200/50 dark:ring-neutral-800/50 transition-all duration-300">
            <div class="absolute inset-0 bg-gradient-to-br from-rose-500/5 to-transparent opacity-0 group-hover:opacity-100 rounded-3xl transition-opacity duration-300"></div>
            <div class="relative">
              <div class="flex items-center gap-4 mb-6">
                <div class="flex items-center justify-center w-12 h-12 rounded-2xl bg-neutral-100 dark:bg-neutral-800 text-neutral-900 dark:text-white">
                  <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M17.523 15.3414C17.523 15.3414 16.2731 15.3414 15.6481 15.3414C15.0232 15.3414 14.3982 14.7164 14.3982 14.0914..."/>
                    <path d="M17.523 15.341c0-1.25-.625-1.875-1.875-1.875h-7.5c-1.25 0-1.875.625-1.875 1.875v3.125h11.25v-3.125zM15.44 9.196L16.975 6.54c.15-.262.062-.596-.2-.746-.262-.15-.596-.062-.746.2l-1.583 2.74c-2.316-1.053-5.076-1.053-7.392 0L5.47 6.002c-.15-.262-.484-.35-.746-.2-.262.15-.35.484-.2.746l1.535 2.656C3.593 10.59 2.062 13.575 2 17h20c-.062-3.425-1.593-6.41-4.06-7.804zM7.25 14.25c-.69 0-1.25-.56-1.25-1.25s.56-1.25 1.25-1.25 1.25.56 1.25 1.25-.56 1.25-1.25 1.25zm9.5 0c-.69 0-1.25-.56-1.25-1.25s.56-1.25 1.25-1.25 1.25.56 1.25 1.25-.56 1.25-1.25 1.25z"/>
                  </svg>
                </div>
                <h2 class="text-2xl font-bold">Android / Chrome</h2>
              </div>
              <ul class="space-y-4 text-neutral-600 dark:text-neutral-400">
                <li class="flex items-start gap-3">
                  <span class="flex items-center justify-center w-6 h-6 rounded-full bg-rose-100 dark:bg-rose-900/50 text-rose-600 dark:text-rose-400 text-sm font-semibold shrink-0 mt-0.5">1</span>
                  <span>Tap the <strong class="text-neutral-900 dark:text-white">Menu</strong> icon (3 dots) in the top right.</span>
                </li>
                <li class="flex items-start gap-3">
                  <span class="flex items-center justify-center w-6 h-6 rounded-full bg-rose-100 dark:bg-rose-900/50 text-rose-600 dark:text-rose-400 text-sm font-semibold shrink-0 mt-0.5">2</span>
                  <span>Tap <strong class="text-neutral-900 dark:text-white">"Install app"</strong> or <strong class="text-neutral-900 dark:text-white">"Add to Home screen"</strong>.</span>
                </li>
                <li class="flex items-start gap-3">
                  <span class="flex items-center justify-center w-6 h-6 rounded-full bg-rose-100 dark:bg-rose-900/50 text-rose-600 dark:text-rose-400 text-sm font-semibold shrink-0 mt-0.5">3</span>
                  <span>Follow the on-screen prompt to <strong class="text-neutral-900 dark:text-white">Install</strong>.</span>
                </li>
              </ul>
            </div>
          </div>

        </div>

      </div>
    </div>
  </div>
</template>

<script setup>
// Use the Vite PWA manifest to ensure standard manifest mounting
useHead({
  title: 'Install PWA App',
  meta: [
    { name: 'description', content: 'Instructions for installing our application on your device.' }
  ]
})
</script>

<style>
@keyframes fade-in-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}
.animate-fade-in-up {
  animation: fade-in-up 0.8s cubic-bezier(0.16, 1, 0.3, 1) forwards;
}
</style>
