<template>
  <h1>ユーザID: {{ user.name }}</h1>
</template>

<script>
export default {
  data () {
    return {
      id: this.$route.params.id,
      users: [
        { id: 1, name: 'john Doe' },
        { id: 2, name: 'kevin Smith' },
        { id: 3, name: 'Harry Bosch' },
      ]
    }

  },
  computed: {
    user () {
      return this.users.find(user => user.id == this.id)
    }
  }
}
</script>
