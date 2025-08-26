<script setup>
function scrollToSection(id) {
    const el = document.getElementById(id)
    if (el) {
        el.scrollIntoView({ behavior: "smooth" })
    }
}
</script>

<template>
    <nav class="fixed top-0 w-full z-50 bg-black/30 backdrop-blur-lg">
        <div class="max-w-6xl mx-auto px-6 lg:px-8 py-6 flex justify-center md:justify-between items-center">
            <button @click="scrollToSection('inicio')" class="flex gap-2 cursor-pointer  justify-center items-center">
                <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" viewBox="0 0 24 24">
                    <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="1">
                        <path stroke-width="2" d="M8 12h.009m3.986 0h.01m3.986 0H16" />
                        <path stroke-width="1.5"
                            d="M18 21c1.232 0 2.231-1.151 2.231-2.571c0-2.248-.1-3.743 1.442-5.52c.436-.502.436-1.316 0-1.818c-1.542-1.777-1.442-3.272-1.442-5.52C20.231 4.151 19.232 3 18 3M6 21c-1.232 0-2.231-1.151-2.231-2.571c0-2.248.1-3.743-1.442-5.52c-.436-.502-.436-1.316 0-1.818C3.835 9.352 3.769 7.84 3.769 5.57C3.769 4.151 4.768 3 6 3" />
                    </g>
                </svg>
                <div
                    class=" text-3xl font-bold bg-gradient-to-r from-cyan-400 via-blue-400 to-purple-500 bg-clip-text text-transparent">
                    coodii
                </div>
            </button>

            <div class="hidden md:flex space-x-8">
                <button @click="scrollToSection('servicios')"
                    class="text-slate-300 hover:text-cyan-400 cursor-pointer  transition-all duration-300 font-medium hover:scale-105">
                    Servicios
                </button>
                <button @click="scrollToSection('nosotros')"
                    class="text-slate-300 hover:text-cyan-400 cursor-pointer  transition-all duration-300 font-medium hover:scale-105">
                    Nosotros
                </button>
                <button @click="scrollToSection('contacto')"
                    class="text-slate-300 hover:text-cyan-400 cursor-pointer  transition-all duration-300 font-medium hover:scale-105">
                    Contacto
                </button>
            </div>
        </div>
    </nav>
</template>
