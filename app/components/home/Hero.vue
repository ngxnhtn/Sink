<script setup>
import { AreaChart } from 'lucide-vue-next'
import heroImg from '@/assets/images/hero.svg?raw'
</script>

<template>
  <main
    class="
      grid place-items-center pt-8 pb-8
      md:py-12
      lg:grid-cols-2
    "
  >
    <div>
      <h1
        class="text-6xl font-bold"
      >
        Rút gọn Link - Eddie
      </h1>
      <div
        class="
          mt-6 flex flex-col gap-3
          sm:flex-row
        "
      >
        <HomeLink
          href="/dashboard"
          type="outline"
          title="Dashboard"
          class="flex items-center justify-center gap-1"
          rel="noopener"
        >
          <AreaChart
            class="h-5 w-5"
          />
          Quản trị
        </HomeLink>
      </div>
    </div>
    <div
      class="
        hidden py-6
        md:block
      "
    >
      <div
        class="w-lg"
        v-html="heroImg"
      />
    </div>
  </main>
</template>
