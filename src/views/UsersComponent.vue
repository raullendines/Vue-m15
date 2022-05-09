<template>
  <div class="home">
    <UsersComponent/>
  </div>
</template>

<script>
// @ is an alias to /src
import UsersComponent from '@/components/UsersComponent.vue'

export default {
  name: 'HomeView',
  components: {
    UsersComponent
  }
}
</script>