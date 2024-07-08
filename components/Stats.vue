<template>
  <div>
    <dl class="mt-8 grid grid-cols-1 gap-5 sm:grid-cols-4">
      <div
        v-for="item in stats"
        :key="item.name"
        class="overflow-hidden rounded-lg bg-white px-4 py-5 border border-gray-200 sm:p-6"
      >
        <dt class="truncate text-sm font-medium text-gray-500">
          {{ item.name }}
        </dt>
        <dd class="mt-1 text-3xl font-semibold tracking-tight text-gray-900">
          <span class="flex items-center gap-1"
            ><count-up :end-val="item.stat"></count-up>%</span
          >
        </dd>
      </div>
    </dl>
  </div>
</template>

<script setup>
import CountUp from "vue-countup-v3";
const stats = [
  { name: "Total Subscribers", stat: 40 },
  { name: "Avg. Open Rate", stat: 40 },
  { name: "Avg. Click Rate", stat: 50 },
  { name: "Avg. Click Rate", stat: 90 },
];
</script>
