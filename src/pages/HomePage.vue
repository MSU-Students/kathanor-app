<template>
  <div class="home">
    THis is my HOME {{101 + 2}}
    <button>Submit</button>
    <q-btn icon="phone" label="Call" stack glossy color="purple" />
    <q-select :options="['Male', 'Female']" label="Standard" />
    <ul>
      <li v-bind:key="item.id" v-for="item in records">{{item.name}}</li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      records : [{id:1, name: 'Ibrahim'}, {id:2, name: 'Nisa'}, {id:3, name: 'Me'}, {id:4, name: 'Me'}]
    }
  }
}
</script>
<style scoped>
  .home {
    color: blue;
  }
</style>
