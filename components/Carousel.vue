<template>
  <div class="max-w-7xl mx-auto md:hidden block px-2">
    <div class="splide" ref="splide">
      <div class="splide__track">
        <ul class="splide__list">
          <li class="splide__slide" v-for="(image, index) in data" :key="index">
            <div class="col-span-1 rounded-md p-2 bg-[#F5F5F5]">
              <NuxtImg
                src="https://images.olx.com.pk/thumbnails/462714568-800x600.webp"
                class="w-full h-auto"
                alt=""
              />
              <Heading
                text="FURGONI"
                class="text-[22px] text-[#343B3C] font-bold"
              />
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
    perPage: 1,
    perMove: 1,
    gap: "1rem",
    arrows: false,
  }).mount();
});
const next = () => {
  splide.value.go(">"); // Move to the next slide
};

const prev = () => {
  splide.value.go("<"); // Move to the previous slide
};
</script>

<style>
@import "@splidejs/splide/dist/css/splide.min.css";

.splide__arrows {
  background: red !important;
  display: flex;
  align-items: center;
  justify-content: center;
}
.splide__arrow {
  align-items: center;
  background: #ccc;
  border: 0;

  cursor: pointer;
  display: flex;
  height: 30px;
  justify-content: center;
  opacity: 0.7;
  padding: 0;
  position: absolute;
  top: -18%;

  width: 30px;
  z-index: 1;
}
.custom-arrow svg {
  width: 24px;
  height: 24px;
  color: #000; /* Change color as needed */
}
.splide__arrow--next {
  right: 0em;
  background: transparent;
}
.splide__arrow--prev {
  left: 96%;

  background: transparent;
}
</style>
