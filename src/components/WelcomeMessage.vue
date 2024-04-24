<script setup>
import logo from "../assets/images/logo-vertical.png"
import image1 from "../assets/images/13.jpeg"
import PrimaryButton from "./PrimaryButton.vue";


</script>

<template>
    <div class="w-full bg-storm-gray-200 background-image min-h-[90vh]">
        <div class="grid pt-12 md:pt-22 grid-cols-1 md:grid-cols-2 w-full min-h-[90vh] ">
            <div
                class="grid md:place-content-center pt-4 lg:pb-16 bg-gradient-to-r from-minsk-950 from-20% to-minsk-100/0 to-100%">
                <div class="w-full flex justify-center md:justify-end lg:pt-24">
                    <div
                        class="relative grid grid-cols-1 place-content-center px-6 w-full bg-storm-gray-100 md:w-3/4 py-12 md:py-8 lg:py-12 md:rounded-md shadow-md">
                        <div
                            class="absolute -bottom-10 -left-32 h-32 w-40 bg-transparent bg-[radial-gradient(#A8A8A8_2px,transparent_1px)] [background-size:16px_16px]">
                        </div>
                        <div
                            class="absolute -top-10 -left-24 h-60 w-32 bg-transparent bg-[radial-gradient(#000000_2px,transparent_1px)] [background-size:16px_16px]">
                        </div>
                        <div
                            class="hidden md:block absolute top-20 -right-24 h-60 w-32 bg-transparent bg-[radial-gradient(#000000_2px,transparent_1px)] [background-size:16px_16px]">
                        </div>

                        <div class="flex justify-center mb-4">
                            <!-- <img :src="logo" class="h-40 md:h-28 lg:h-32 2xl:h-52 w-auto" /> -->
                            <img :src="logo" class="h-52" />
                        </div>
                        <div class="lg:px-10 max-w-lg md:max-w-2xl mx-auto">
                            <p class="text-2xl font-semibold text-minsk-900 text-center mb-2">
                                Más de 20 años siendo expertos en el Aislamiento Térmico
                            </p>
                            <p class="text-storm-gray-700 text-center mb-6 ">
                                Somos expertos en la distribución de materiales para aislamiento térmico, así como en el
                                diseño, implementación y mantenimiento de diversos tipos de sistemas de aislamiento
                                térmico.
                            </p>
                            <div class="w-full flex justify-center">
                                <a href="#contacto">
                                    <PrimaryButton>¡Contactanos!</PrimaryButton>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
                <img :src="image1"
                    class="w-full flex justify-center md:justify-end md:hidden h-[80vh] md:h-[80vh] object-cover" />
                <div>
                </div>

            </div>
        </div>
    </div>
</template>+

<style scoped>
.background-image {
    background-image: url("../assets/images/13.jpeg");
    background-size: cover;
    height: 100%;
}
</style>