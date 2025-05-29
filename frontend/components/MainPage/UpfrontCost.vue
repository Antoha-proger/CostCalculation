<script setup>
import { questions } from '~/helper/helps'
import { ref } from 'vue';

let counter = ref(1);
let sum = ref(0)

function counterInc() {
    // console.log(rr.value);
    costsCum.value.push(rr.value)
    if (counter.value < 5) {
        counter.value++
    }

    if (costsCum.value.length <= 4) {
        costsCum.value.forEach(elem => {
            sum.value += elem
        })
    }
    console.log(sum);
    
}

function counterDec() {
    if (counter.value > 1) {
        counter.value--
    }
}

let costsCum = ref([])
let rr = ref("")

</script>

<template>
    <div class="h-[615px] flex items-center flex-col justify-between pt-[108px]">
        <div class="flex items-center h-[400px] w-[100%]">
            <div class="w-[50%] bg-[#150981] h-[400px] grid place-content-center">
                <h3 class="text-center text-white text-[32px] font-semibold">Узнайте предварительную<br>стоимость проекта</h3>
            </div>
            <div class="w-[50%] h-[400px] flex flex-col justify-between items-center pt-[10px]">
                <p class="text-xl text-[#2E1AEB] mb-[30px]">{{ counter }}/5</p>
                <p class="text-2xl mb-[30px]">{{ questions[counter-1].question }}</p>
                <div class="mb-[70px]" v-if="counter < 5">
                    <MainPageRadioButtons v-for="question in questions[counter-1].answers" v-model="rr" :question="question" :key="question"/>
                </div>
                <div v-else class="mb-[70px]">
                    <p class="text-3xl text-[#150981] text-center mb-[30px]">Предварительная стоимость<br>вашего проекта составляет {{ sum }}</p>
                    <p class="text-sm text-center ">Отправь заявку сейчас и получи скидку 10%</p>
                </div>
                <div class="w-[85%] flex justify-between">
                    <button class="w-[126px] h-[35px] text-white bg-[#150981]" @click="counterDec" v-show="counter > 1">Назад</button>
                    <button class="w-[126px] h-[35px] text-white bg-[#150981]" @click="counterInc" v-if="counter < 5">Вперед</button>
                    <button class="w-[126px] h-[35px] text-white bg-[#150981]" v-else>Отправить</button>
                </div>
            </div>
        </div>
        <div class="w-[50px] h-[3px] bg-[#150981]"></div>
    </div>
</template>