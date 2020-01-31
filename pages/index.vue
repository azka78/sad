<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
    xs12
    sm8
    md6
    >

    </v-flex>
    <login
    xs6
    sm8
    md6
    v-model="login"
    fixed
    />
    <button type="button" name="button" @click.stop="login = !login"></button>

  </v-layout>
</template>

<script>
  import login from '~/components/login.vue'
  export default {
    components: {
      login
    },
    data () {
      return {
        login: false
      }
    }
  }


  </script>
