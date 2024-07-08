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
          {{ item.stat }}
        </dd>
      </div>
    </dl>
  </div>
</template>

<script setup>
const stats = [
  { name: "Total Subscribers", stat: "71,897" },
  { name: "Avg. Open Rate", stat: "58.16%" },
  { name: "Avg. Click Rate", stat: "24.57%" },
  { name: "Avg. Click Rate", stat: "24.57%" },
];
</script>
