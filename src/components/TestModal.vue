<template>
  <Modal>
    <ModalHeader>
      <h3>Test Modal #1</h3>
    </ModalHeader>
    <ModalBody>
      <p>Body of modal #1</p>
    </ModalBody>
    <ModalFooter>
      <button @click="close('Modal closed')" class="btn btn-primary">Close Modal</button>
      <button @click="dismiss('Modal dismissed')" class="btn btn-primary">Dismiss Modal</button>
    </ModalFooter>
  </Modal>
</template>

<script>
import Modal from '../modules/modals/components/Modal.vue';
import ModalHeader from '../modules/modals/components/ModalHeader.vue';
import ModalFooter from '../modules/modals/components/ModalFooter.vue';
import ModalBody from '../modules/modals/components/ModalBody.vue';
import ModalMixin from '../modules/modals/mixins/ModalMixin';
export default {
  components: { Modal, ModalHeader, ModalBody, ModalFooter },
  mixins: [ModalMixin],
}
</script>