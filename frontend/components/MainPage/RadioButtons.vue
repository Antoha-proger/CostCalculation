<script setup>
defineProps(['question'])

const model = defineModel()
</script>

<template>
    <div class="mb-[10px] self-start w-[550px]">
        <input class="" type="radio" :id="question.answer" v-model="model" name="questions" :value="question.cost" >
        <label class="pl-[10px]" :for="question.answer">{{ question.answer }}</label>
    </div>
</template>

<!-- :v-model="modelValue" -->