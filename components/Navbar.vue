<template>
    <nav class="flex items-center justify-between flex-wrap  bg-teal-500 p-6">
        <div class="flex items-center flex-shrink-0 text-white mr-10">
            <svg class="fill-current h-8 w-8 mr-2" width="54" height="54" viewBox="0 0 54 54"
                xmlns="http://www.w3.org/2000/svg">></svg>
            <span class="font-semibold text-xl tracking-tight mr-10">SMKN 1 Cibadak</span>
                </div>        
                <div class="bg-bg-cyan-600">
                </div>
                <div class="block lg:hidden">
                    <button
                class="flex items-center px-3 py-2 border rounded text-teal-200 border-teal-400 hover:text-white hover:border-white">
            </button>
        </div>
        <div class="w-full block flex-grow lg:flex lg:items lg:w-auto">
            <div class="text-sm lg:flex-grow">
                <a v-for="(item, index) in navigations" :key="index" href="item.link"
                    class="block mt-20 lg:inline-block lg:mt-0 text-teal-200 hover:text-white mr-10">
                    {{ item.label }}
                </a>
            </div>

        </div>
    </nav>
</template>

<script>
export default {
    data() {
        return {
            navigations: [
                {
                    "label": "Home",
                    "link": "/Home"
                },
                {
                    "label": "Program Studi",
                    "link": "/Program Studi"
                },
                {
                    "label": "Data Siswa",
                    "link": "/Data Siswa"
                },
                {
                    "label": "Organisasi",
                    "link": "/Organisasi"
                },
                {
                    "label": "Info",
                    "link": "/Info"
                },
                {
                    "label": "Berita",
                    "link": "/Berita"
                },
                {
                    "label": "Tentang",
                    "link": "/Tentang"
                },
                {
                    "label": "Kontak",
                    "link": "/Kontak"
                }
            ]
        }
    },
}
</script>
