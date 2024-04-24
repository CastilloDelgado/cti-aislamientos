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
                        <p>Ing. Rodolfo Ide Pinto</p>
                    </div>
                    <div class="flex justify-between gap-2">
                        <p class="font-semibold">Dirección:</p>
                        <a href="https://maps.app.goo.gl/pRcoWUMNJBg3dgn48" target="_blank">
                            <p class="text-right">
                                Mezquite 1427, Del Fresno, 44900 Guadalajara, Jal. </p>
                        </a>
                    </div>
                    <div class="flex justify-between gap-2">
                        <p class="font-semibold">Teléfono:</p>
                        <a href="tel:+52-33-1615-0122">
                            <p>+52 33-1615-0122</p>
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
                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d983.1387586512367!2d-103.36766664602231!3d20.655747784292128!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8428adfbab7ac57b%3A0x47bc8659178498ce!2sMezquite%201427%2C%20Del%20Fresno%2C%2044900%20Guadalajara%2C%20Jal.!5e0!3m2!1sen!2smx!4v1713998144705!5m2!1sen!2smx"
                            width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"
                            referrerpolicy="no-referrer-when-downgrade"></iframe>
                    </div>
                </div>
            </div>
            <div class="">
                <div class="flex justify-center">
                    <form class="w-full sm:2/3" action="https://formsubmit.co/contacto@cti-aislamientos.com"
                        method="POST">
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