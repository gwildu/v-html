<template>
  <div>
    <ul v-if="dummies && dummies.length > 0">
      <li v-for="dummy in dummies">{{dummy}}</li>
    </ul>
    <table v-if="dummies && dummies.length > 0">
      <tr v-for="dummy in dummies">
        <td>{{dummy}}</td>
      </tr>
    </table>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        dummies: ['something', 'something else']
      }
    }
//    props: {
//      dummies: {
//        type: Array,
//        required: true,
//        default: []
//      }
//    }
  }
</script>

<style></style>
