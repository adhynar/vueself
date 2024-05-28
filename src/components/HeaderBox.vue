<script setup>
    const handler = () => {
        const menuBox = document.querySelector('#menuBox')
        const toggleBtn = document.querySelector('#toggleBtn')
        menuBox.classList.toggle('hidden')
        toggleBtn.classList.toggle('bg-slate-700')
    }
</script>
<template>
    <header>
        <nav class="h-[125px] w-full bg-blue-950 flex items-center gap-4 justify-between">
            <div class="p-4 w-full lg:w-auto">
                <p class="text-3xl text-white translate-x-10 font-bold font-mono text-center lg:text-start lg:translate-x-0">Lorem Ipsum</p>
            </div>
            <div class="p-4 relative lg:hidden">
                <div id="toggleBtn" class="p-4 flex flex-col gap-2 rounded-lg hover:cursor-pointer" @click="handler">
                    <div class=" h-1 w-10 rounded-lg bg-white"></div>
                    <div class=" h-1 w-10 rounded-lg bg-white"></div>
                    <div class=" h-1 w-10 rounded-lg bg-white"></div>
                </div>
                <div id="menuBox" class="p-4 absolute bg-slate-700 -left-6 top-16 rounded-lg hidden">
                    <ul class="flex flex-col gap-4">
                    <li class="text-white semibold text-lg py-2 px-3 rounded-lg hover:bg-slate-50 hover:text-slate-700 hover:font-bold">Sit</li>
                    <li class="text-white semibold text-lg py-2 px-3 rounded-lg hover:bg-slate-50 hover:text-slate-700 hover:font-bold">Dolor</li>
                    <li class="text-white semibold text-lg py-2 px-3 rounded-lg hover:bg-slate-50 hover:text-slate-700 hover:font-bold">Epeum</li>
                </ul>
                </div>
            </div>
            <div class="p-4 hidden lg:block">
                <ul class="flex flex-row gap-4">
                    <li class="text-white semibold text-lg py-2 px-3 rounded-lg hover:bg-slate-50 hover:text-slate-700 hover:font-bold">Sit</li>
                    <li class="text-white semibold text-lg py-2 px-3 rounded-lg hover:bg-slate-50 hover:text-slate-700 hover:font-bold">Dolor</li>
                    <li class="text-white semibold text-lg py-2 px-3 rounded-lg hover:bg-slate-50 hover:text-slate-700 hover:font-bold">Epeum</li>
                </ul>
            </div>
        </nav>
        <div id="jumbotron" class="bg-slate-400 flex flex-row gap-4 flex-wrap justify-between p-10">
            <div class="w-full flex pl-6 flex-col gap-5 justify-center lg:w-1/3">
                <h1 class="text-5xl text-center font-bold lg:text-start">Lorem, ipsum dolor.</h1>
                <p class="text-lg text-center lg:text-start">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Provident, commodi.</p>
            </div>
            <div class="w-full flex flex-col items-center lg:w-1/2">
                <img class="w-full h-full rounded-full" src="../assets/image/evans.jpg" />
            </div>
        </div>
    </header>
</template>

<script>

</script>