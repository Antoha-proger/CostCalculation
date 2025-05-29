<template>
    <div class="h-[600px] flex items-center flex-col justify-between pt-[108px]">
        <div class="flex items-center h-[400px] w-[100%]">
            <div class="w-[50%] bg-[#150981] h-[400px] grid place-content-center">
                <h3 class="text-center text-white text-[32px] font-semibold">Остались вопросы?<br>Напишите нам!</h3>
            </div>
            <div class="w-[50%] h-[100%]">
                <form action="" class="flex flex-col items-center w-[100%] h-[100%] pt-[40px]">
                    <input type="text" placeholder="ФИО" class="w-[300px] h-[40px] border border-[#150981] rounded-[20px] pl-[20px] outline-[#150981] mb-[25px]">
                    <input type="email" placeholder="Почта" class="w-[300px] h-[40px] border border-[#150981] rounded-[20px] pl-[20px] outline-[#150981] mb-[25px]">
                    <textarea placeholder="Сообщение" class="w-[300px] pt-[10px] h-[150px] border border-[#150981] rounded-[20px] pl-[20px] outline-[#150981] mb-[25px]"></textarea>
                    <button class="cursor-pointer w-[300px] h-[35px] bg-[#150981] rounded-[10px] text-white grid place-items-center text-lg hover:bg-white hover:text-[#150981] duration-300 border border-[#150981]">Отправить</button>
                </form>
            </div>
        </div>
        <div class="w-[50px] h-[3px] bg-[#150981]"></div>
    </div>
</template>