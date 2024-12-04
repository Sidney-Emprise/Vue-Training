<!--
Modal component with customizable slots and CSS transitions.
-->

<script>
import Modal from './Modal.vue'

export default {
  components: {
    Modal
  },
  data() {
    return {
      showModal: false
    }
  }
}
</script>

<template>
  <button id="show-modal" @click="showModal = true">Show Modal</button>

  <Teleport to="body">
    <!-- use the modal component, pass in the prop -->
    <modal :show="showModal" @close="showModal = false">
      <template #header>
        <h3>Submit your Question</h3>
      </template>
      <template #body>
        <p>This is a preview of your email, if you are satisfied with your submission hit OK.</p>
      </template>
    </modal>
  </Teleport>
</template>