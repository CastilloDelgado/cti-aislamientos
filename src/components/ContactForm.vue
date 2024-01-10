
<script setup>
import PrimaryButton from './PrimaryButton.vue';
</script>

<template>
    <div class="bg-storm-gray-100" id="contacto">
        <div class="max-w-7xl px-6 mx-auto py-12 grid grid-cols-1 gap-6 md:grid-cols-2 place-content-center ">
            <div class="mb-8 md:mb-0">
                <p class="text-center text-2xl text-minsk-800 font-semibold mb-6">Información de contacto</p>
                <div class="max-w-lg mx-auto flex flex-col gap-1">
                    <div class="flex justify-between gap-2">
                        <p class="font-semibold">Nombre de Contacto:</p>
                        <p>Ing. Carlos Ide Ornelas</p>
                    </div>
                    <div class="flex justify-between gap-2">
                        <p class="font-semibold">Dirección:</p>
                        <a href="https://maps.app.goo.gl/pRcoWUMNJBg3dgn48" target="_blank">
                            <p class="text-right">
                                Isla Trinidad No. 2458 Col. Jardines de la Cruz Guadalajara, Jal. C.P. 44920
                            </p>
                        </a>
                    </div>
                    <div class="flex justify-between gap-2">
                        <p class="font-semibold">Teléfono:</p>
                        <a href="tel:+52-33-3811-3359">
                            <p>+52 33-3811-3359</p>
                        </a>
                    </div>
                    <div class="flex justify-between gap-2 mb-4">
                        <p class="font-semibold">Correo electrónico:</p>
                        <a href="mailto:contacto@cti-aislamientos.com">
                            <p>contacto@cti-aislamientos.com</p>
                        </a>
                    </div>
                    <div class="h-72 border-4 border-white">
                        <iframe
                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3733.5302334690523!2d-103.37908062473456!3d20.64799630074758!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8428adeed33ae66b%3A0xbd639ca291abddb4!2sIsla%20Trinidad%202458%2C%20Col%C3%B3n%2C%2044920%20Guadalajara%2C%20Jal.!5e0!3m2!1ses-419!2smx!4v1704927808138!5m2!1ses-419!2smx"
                            width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"
                            referrerpolicy="no-referrer-when-downgrade"></iframe>
                    </div>
                </div>
            </div>
            <div class="">
                <div class="flex justify-center">
                    <form class="w-full sm:2/3" action="https://formsubmit.co/contacto@cti-aislamientos.com" method="POST">
                        <p class="text-center text-2xl text-minsk-900 font-bold mb-2">Contacto</p>
                        <p class="text-center text-lg  px-6 lg:px-24 mb-6 text-storm-gray-800">
                            Completa el formulario, da click enviar y te contactaremos a la brevedad.
                        </p>
                        <div class="lg:px-16">
                            <div class="mb-2 flex flex-col">
                                <label class="text-lg mb-1" for="">Nombre Completo</label>
                                <input
                                    class="border-2 border-storm-gray-200 rounded-sm bg-dark-400 px-2 py-1 text-storm-gray-800 placeholder:text-storm-gray-400"
                                    type="text" name="name" placeholder="Nombre Completo" required />
                            </div>
                            <div class="mb-2 flex flex-col">
                                <label class="text-lg mb-1" for="">Correo Electrónico</label>
                                <input
                                    class="border-2 border-storm-gray-200 rounded-sm bg-dark-400 px-2 py-1 text-storm-gray-800 placeholder:text-storm-gray-400"
                                    placeholder="Correo electrónico" type="email" name="email" required />
                            </div>

                            <div class="flex flex-col mb-6">
                                <label class="text-lg mb-1" for="">Escribe aquí tus dudas</label>
                                <textarea rows="6"
                                    class="border-2 border-storm-gray-200 rounded-sm bg-dark-400 px-2 py-1 text-storm-gray-800 placeholder:text-storm-gray-400"
                                    placeholder="..." name="message" required />
                            </div>
                            <div class="flex justify-center">
                                <a href="#contacto">
                                    <PrimaryButton type="submit">Enviar</PrimaryButton>
                                </a>
                            </div>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>