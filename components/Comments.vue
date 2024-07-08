<template>
  <div class="w-full mt-4">
    <div class="splide" ref="splide">
      <div class="splide__track">
        <ul class="splide__list">
          <li class="splide__slide" v-for="(image, index) in data" :key="index">
            <div
              class="cursor-pointer rounded-lg border-2 border-[#F3F3F3] bg-white px-5 py-5 hover:bg-[#3677EF] hover:bg-opacity-5"
            >
              <div class="flex items-center justify-between gap-4">
                <div class="flex items-center gap-2">
                  <img
                    src="https://tailwindui.com/img/avatar-2.jpg"
                    alt=""
                    class="h-10 w-10 rounded-full"
                  />
                  <h1
                    class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] text-[17px] font-semibold"
                  >
                    Kashif
                  </h1>
                </div>
                <div class="flex items-center gap-1">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="h-5 w-5 text-[#E2B704]"
                    width="1em"
                    height="1em"
                    viewBox="0 0 24 24"
                  >
                    <path
                      fill="currentColor"
                      d="m12 17.27l4.15 2.51c.76.46 1.69-.22 1.49-1.08l-1.1-4.72l3.67-3.18c.67-.58.31-1.68-.57-1.75l-4.83-.41l-1.89-4.46c-.34-.81-1.5-.81-1.84 0L9.19 8.63l-4.83.41c-.88.07-1.24 1.17-.57 1.75l3.67 3.18l-1.1 4.72c-.2.86.73 1.54 1.49 1.08z"
                    />
                  </svg>

                  <h1
                    class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] text-xl font-semibold"
                  >
                    4.8
                  </h1>
                </div>
              </div>
              <h3
                class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] pt-2"
              >
                Stay cool and casual with our product, Lorem ipsum dolor sit
                amet consectetur, adipisicing elit. Facere, aliquam.
              </h3>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script setup>
import { onMounted, ref, defineProps } from "vue";
import Splide from "@splidejs/splide";

const images = [1, 2, 3, 4, 5, 6, 7, 8];

defineProps({
  data: {
    type: Object,
    default: [1, 2, 3, 4, 5],
  },
});

const splide = ref(null);

onMounted(() => {
  new Splide(splide.value, {
    type: "loop",
    perPage: 2,
    perMove: 1,
    gap: "1rem",
    pagination: false,
    arrows: false,
    autoplay: true,
  }).mount();
});
const next = () => {
  splide.value.go(">"); // Move to the next slide
};

const prev = () => {
  splide.value.go("<"); // Move to the previous slide
};
</script>
