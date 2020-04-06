<template>
  <div id="app" class="container">
    <div class="mt-5"></div>
    <div class="row mb-5">
      <div class="col-md-6 m-auto">
        <Todos v-bind:todos="item" v-bind:key="item.id" v-for="item in groceryList"/>
      </div>
    </div>
  </div>
</template>

<script>
  import Todos from "./components/Todos";
  export default {
    components: {
      Todos
    },
    data() {
      return {
        groceryList: [
          { id: 0, text: 'Vegetables' },
          { id: 1, text: 'Cheese' },
          { id: 2, text: 'Whatever else humna are supposed to eat'}
        ]
      }
    }
  }
</script>


