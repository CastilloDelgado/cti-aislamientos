<script setup>
import { ref } from "vue"
import kockLogo from "../assets/images/koch-logo.png"
import nestleLogo from "../assets/images/nestle-logo.jpg"
import tequilaLogo from "../assets/images/tequila-logo.png"
import sauzaLogo from "../assets/images/sauza-logo.jpg"
import oleosLogo from "../assets/images/oleos-logo.jpg"
import CustomerBadge from "./CustomerBadge.vue"
import PrimaryButton from "./PrimaryButton.vue"


const customers = ref([
    {
        alt: "Kock Company",
        title: "Koch Company",
        url: "https://kochllc.com/our-brands/koch-mexico/",
        image: kockLogo
    },
    {
        alt: "Nestlé México",
        title: "Nestlé México",
        url: "https://www.nestle.com.mx/",
        image: nestleLogo
    },
    {
        alt: "Tequilas Finos de México SA. de CV.",
        title: "Tequilas Finos de México SA. de CV.",
        url: "https://www.mexbest.com/empresa-fabrica-de-tequilas-finos-937.html",
        image: tequilaLogo
    },
    {
        alt: "Tequila Sauza",
        title: "Tequila Sauza",
        url: "https://www.casasauza.com/",
        image: sauzaLogo
    },
    {
        alt: "Oleos Finos",
        title: "Oleos Finos",
        url: "https://oleofinos.com.mx/",
        image: oleosLogo
    },
    // {
    //     alt: "Benotto",
    //     title: "Benotto",
    //     url: "https://tienda.benotto.com/?view=Home",
    //     image: benottoLogo
    // },
    // {
    //     alt: "Fresenius Kabi",
    //     title: "Fresenius Kabi",
    //     url: "https://www.fresenius-kabi.com/mx/",
    //     image: freseniusLogo
    // },
    // {
    //     alt: "Grupo Morsa",
    //     title: "Grupo Morsa",
    //     url: "https://www.morsa.com.mx/",
    //     image: morsaLogo
    // },
    // {
    //     alt: "Cactus Feliz",
    //     title: "Cactus Feliz",
    //     url: "https://cactusfeliz.com/",
    //     image: cactusLogo
    // },
])

</script>

<template>
    <div class="bg-white">
        <div class="max-w-7xl mx-auto py-12 px-6 md:px-8">
            <div class="max-w-xl mx-auto text-center mb-8">
                <p class="text-4xl font-bold text-minsk-900 mb-6">Nuestros clientes</p>
                <p class="text-storm-gray-700  text-xl">
                    Con una destacada trayectoria en el mercado, hemos
                    adquirido una amplia experiencia brindando soluciones a
                    diversos proyectos.
                </p>
            </div>
            <div class="flex justify-center flex-wrap gap-x-6 gap-y-2 lg:gap-x-12  lg:gap-y-6 max-w-4xl mx-auto px-6">
                <CustomerBadge v-for="customer in customers" :customer="customer" />
            </div>
            <div class="max-w-xl mx-auto text-storm-gray-700 ">
                <p class="text-xl text-center mt-12 mb-8">
                    Ponte en contacto con nosotros para saber más de nuestros proyectos.
                </p>
                <div class="w-full flex justify-center">
                    <a href="#contacto">
                        <PrimaryButton>¡Contactanos!</PrimaryButton>
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>