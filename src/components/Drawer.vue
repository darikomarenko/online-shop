<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-70"></div>
  <div class="bg-white w-96 h-full fixed right-0 top-0 z-20 p-8">

    <DrawerHead/>
    <CartItemList/>

    <div class="flex flex-col gap-4 my-6">
      <div class="flex gap-2">
        <span>Total:</span>
        <div class="flex-1 border-bottom border-dashed"></div>
        <b>12900$</b>
      </div>

      <div>
      <div class="flex gap-2">
        <span>Tax 5%:</span>
        <div class="flex-1 border-bottom border-dashed"></div>
        <b>900$</b>
      </div>
    </div>

    </div>

    <button class="bg-lime-500 w-full rounded-xl py-3 text-white disabled:bg-slate-300 transition hover:bg-lime-700">
      Order
    </button>
  </div>
</template>

<script setup>
import DrawerHead from './DrawerHead.vue'
import CartItemList from './CartItemList.vue'
</script>
