<template>
  <div class="hello">
     <button @click="addModal" class="btn btn-primary">Open modal</button>
  </div>
</template>

<script>
import ModalService from '../modules/modals/services/modal.service';
import TestModal from '../components/TestModal.vue';
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
    methods: {
    addModal() {
      ModalService.open(TestModal);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
