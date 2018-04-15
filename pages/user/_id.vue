<template>
  <div class="f2 ">
{{user.id}} | {{user.created | timeSince}}
<div>
  {{ user.submitted.length}} user submitions:
  <span v-for="item in user.submitted" :key="item">
    <nuxt-link :to="'/item/'+item">{{item}} </nuxt-link>
  </span>
</div>
  </div>
</template>

<script>
  import axios from "~/plugins/axios"
  import ItemsUser from "~/components/ItemsUser"

  export default {
    async asyncData({route:{params}}){
      const response = await axios.get(`/user/${params.id}.json`)
      return { user: response.data}
    }
  }
</script>
