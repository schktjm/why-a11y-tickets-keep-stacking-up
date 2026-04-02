<script setup lang="ts">
import { useNav } from '@slidev/client'

const { currentPage, prev, next } = useNav()
</script>

<template>
  <button class="absolute left-0 inset-y-0 w-16 cursor-pointer" @click="prev()">
    <span class="sr-only">
      前のスライドへ
    </span>
  </button>
  <button class="absolute right-0 inset-y-0 w-16 cursor-pointer" @click="next()">
    <span class="sr-only">
      次のスライドへ
    </span>
  </button>
  <div class="absolute bottom-12 right-4 text-sm opacity-70">
    {{ currentPage }}
  </div>
</template>
