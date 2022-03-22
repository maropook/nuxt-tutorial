<template>
  <div>
    <h1>About Page</h1>
    <h2>{{ subtitle }}</h2>
  </div>
</template>

<script>
export default {
  head () {
    return {
      title: 'Aboutページ',
      meta: [
        { hid: 'description', name: 'description', content: 'これはAboutページ' }
      ]
    }
  },
  data () {
    return {
      id: this.$route.params.id,
      users: [
        {
          id: 1, name: 'John Doe'
        }
      ],
      subtitle: 'この文書'
    }
  },
  computed: {
    user () {
      return this.users.find(user => user.id == this.id)
    }
  }
};
</script>
