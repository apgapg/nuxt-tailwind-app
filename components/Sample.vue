<template>
  <div class='bg-white relative'>
    <SideBar ref='sidebar' class='w-1/6 bg-blue-500 min-h-full z-10 absolute transform -translate-x-full duration-200' />

    <AppBar class='absolute' @side-menu-toggle='onSideMenuToggle' />

    <div class='relative'>
      <div class='flex items-center justify-center min-h-screen'>
        <div>
          <div class='text-4xl'>Welcome to Online DMS</div>
        </div>
      </div>
    </div>
  </div>

</template>

<script>
import AppBar from '@/components/navbar/AppBar'

export default {
  name: 'Sample',
  components: { AppBar },

  methods: {
    onSideMenuToggle() {
      this.$refs.sidebar.classList.toggle('-translate-x-full')
    }
  }
}
</script>
