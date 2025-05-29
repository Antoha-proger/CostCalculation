<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Navigation } from 'swiper/modules';
import 'swiper/css';
import 'swiper/css/navigation';
</script>

<template>
    <div class="container pt-[50px] h-[600px] flex flex-col items-center">
        <h4 class="text-[32px] font-semibold text-[#150981] text-center mb-[60px]">Наши кейсы</h4>

        <swiper class="h-[450px] w-[100%]" :modules="[Navigation]" :slides-per-view="1" :space-between="50" navigation>
            <swiper-slide class="bg-[url(../../assets/image/factory1.png)] rounded-[20px] pt-[50px] pl-[100px]">
                <h4 class="font-bold text-[32px] text-[#150981] mb-[50px]">Завод "НовоеПоколение"</h4>
                <ul class="list-disc ml-[15px] mb-[90px]">
                    <li class="text-[#150981] text-xl font-semibold">Тип сайта: корпоративный сайт</li>
                    <li class="text-[#150981] text-xl font-semibold">Количество страниц: 20 </li>
                    <li class="text-[#150981] text-xl font-semibold">Срок разработки: 6 месяцев</li>
                    <li class="text-[#150981] text-xl font-semibold">Стоимость проекта: 450 тыс. руб.</li>
                </ul>
                <nuxt-link class="pointer w-[200px] h-[35px] bg-[#150981] rounded-[10px] text-white grid place-items-center text-lg hover:bg-white hover:text-[#150981] duration-300 border border-[#150981]" to="/reg">Подробнее</nuxt-link>
            </swiper-slide>
            <swiper-slide class="bg-[url(../../assets/image/coffee.png)] rounded-[20px] pt-[50px] pl-[100px]">
                <h4 class="font-bold text-[32px] text-[#150981] mb-[50px]">Кофейня "КофеТайм"</h4>
                <ul class="list-disc ml-[15px] mb-[90px]">
                    <li class="text-[#150981] text-xl font-semibold">Тип сайта: многостраничный сайт</li>
                    <li class="text-[#150981] text-xl font-semibold">Количество страниц: 7</li>
                    <li class="text-[#150981] text-xl font-semibold">Срок разработки: 3 месяца</li>
                    <li class="text-[#150981] text-xl font-semibold">Стоимость проекта: 200.000 тыс. руб.</li>
                </ul>
                <nuxt-link class="pointer w-[200px] h-[35px] bg-[#150981] rounded-[10px] text-white grid place-items-center text-lg hover:bg-white hover:text-[#150981] duration-300 border border-[#150981]" to="/reg">Подробнее</nuxt-link>
            </swiper-slide>


            <swiper-slide class="bg-[url(../../assets/image/freelance.png)] rounded-[20px] pt-[50px] pl-[100px]">
                <h4 class="font-bold text-[32px] text-[#150981] mb-[50px]">Сайт-визитка дизайнера</h4>
                <ul class="list-disc ml-[15px] mb-[90px]">
                    <li class="text-[#150981] text-xl font-semibold">Тип сайта: сайт-визитка</li>
                    <li class="text-[#150981] text-xl font-semibold">Количество страниц: 3</li>
                    <li class="text-[#150981] text-xl font-semibold">Срок разработки: 3 недели</li>
                    <li class="text-[#150981] text-xl font-semibold">Стоимость проекта: 80.000 тыс. руб.</li>
                </ul>
                <nuxt-link class="pointer w-[200px] h-[35px] bg-[#150981] rounded-[10px] text-white grid place-items-center text-lg hover:bg-white hover:text-[#150981] duration-300 border border-[#150981]" to="/reg">Подробнее</nuxt-link>
            </swiper-slide>
            
        </swiper>
    </div>
</template>