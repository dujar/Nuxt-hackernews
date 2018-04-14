<template>
  <div class="f2 ">
{{user.id}} | {{user.created | timeSince}}
  </div>
</template>

<script>
  import axios from "~/plugins/axios"

  export default {
    async asyncData({route:{params}}){
      const response = await axios.get(`/user/${params.id}.json`)
      return { user: response.data}
    }
  }
</script>