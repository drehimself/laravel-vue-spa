<template>
  <div>
    Fetching users...
  </div>
</template>

<script>
import axios from 'axios'

export default {
  mounted () {
    axios.get('/api/users')
      .then(response => console.log(response.data))
  }
}
</script>
