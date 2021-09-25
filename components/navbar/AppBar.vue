<template>
  <div class='flex w-full h-14 bg-white shadow z-10 items-center px-4'>
    <button @click="onSideMenuToggle" class='hover:bg-blue-100 h-10 w-10 inline-flex items-center justify-center rounded-full'>
      <span class='material-icons-outlined text-gray-600'>menu</span>
    </button>
    <button class='text-xl font-medium ml-2'>Online DMS</button>
    <div class='flex-1'></div>

    <button class='hover:bg-blue-100 h-10 w-10 inline-flex items-center justify-center rounded-full'>
      <span class='material-icons-outlined text-gray-600'>account_circle</span>
    </button>

  </div>

</template>

<script>
export default {
  name: 'AppBar',
  methods: {
    onSideMenuToggle() {
      this.$emit('side-menu-toggle')
    }
  }
}
</script>
