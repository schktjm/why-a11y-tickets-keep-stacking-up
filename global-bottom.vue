<template>
  <div
    class="absolute left-0 inset-y-0 w-16 cursor-pointer"
    style="z-index: 100"
    @click="$slidev.nav.prev()"
  />
  <div
    class="absolute right-0 inset-y-0 w-16 cursor-pointer"
    style="z-index: 100"
    @click="$slidev.nav.next()"
  />
  <div class="absolute bottom-12 right-4 text-sm opacity-70" style="z-index: 100">
    {{ $slidev.nav.currentPage }}
  </div>
</template>
