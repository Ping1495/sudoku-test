<template>
  <div>
    <div
      class="flex flex-col justify-center items-center gap-4 border h-screen border-red-500"
    >
      <!-- topic -->
      <!-- <h1 class="text-3xl font-bold underline">Sudoku Master Z</h1> -->

      <!-- sudoku test -->
      <div class="flex flex-col gap-2">
        <!-- 3x3 -->
        <!-- <div class="text-xl">3x3</div> -->
        <div class="grid grid-cols-2 gap-10 text-8xl font-medium">
          <!-- sudoku grid -->
          <div
            class="grid grid-cols-3 border-2 border-black w-[450px] h-[450px]"
          >
            <div :class="gridSudoku"></div>
            <div :class="gridSudoku"></div>
            <div :class="gridSudoku"></div>
            <div :class="gridSudoku"></div>
            <div :class="gridSudoku"></div>
            <div :class="gridSudoku"></div>
            <div :class="gridSudoku"></div>
            <div :class="gridSudoku"></div>
            <div :class="gridSudoku"></div>
          </div>
          <!-- number botton -->
          <div class="grid grid-cols-3 gap-1 border-black w-[450px] h-[450px]">
            <div :class="numberButton">1</div>
            <div :class="numberButton">2</div>
            <div :class="numberButton">3</div>
            <div :class="numberButton">4</div>
            <div :class="numberButton">5</div>
            <div :class="numberButton">6</div>
            <div :class="numberButton">7</div>
            <div :class="numberButton">8</div>
            <div :class="numberButton">9</div>

            <div :class="helpButton" class="bg-green-600">back</div>
            <div :class="helpButton" class="bg-red-600">delete</div>
            <div :class="helpButton" class="bg-orange-400">reset</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const gridSudoku =
  "border-2 border-black hover:border-red-500 flex justify-center items-center rounde";

const numberButton =
  "border-2 border-black  flex justify-center items-center rounded-xl";

const helpButton =
  "  text-white  text-5xl flex justify-center items-center py-4 rounded-xl";

const box1 = ref();
const box2 = ref();
const box3 = ref();
const box4 = ref();
const box5 = ref();
const box6 = ref();
const box7 = ref();
const box8 = ref();
const box9 = ref();
</script>

<style></style>
