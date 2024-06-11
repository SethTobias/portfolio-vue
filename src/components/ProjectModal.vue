<template>
  <div v-if="isVisible" class="modal project" @click="handleOverlayClick">
    <div class="modal-content project" @click.stop>
      <button class="modal-close project" @click="close">×</button>
      <h2>{{ title }}</h2>
      <p>{{ msg }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProjectModal',
  props: {
    isVisible: {
      type: Boolean,
      required: true
    },
    title: {
      type: String,
      default: ''
    },
    msg: {
      type: String,
      default: ''
    }
  },
  methods: {
    close() {
      this.$emit('close');
    },
    handleOverlayClick() {
      this.close();
    },
    handleEscapeKey(event) {
      if (event.key === 'Escape') {
        this.close();
      }
    }
  },
  mounted() {
    document.addEventListener('keydown', this.handleEscapeKey);
  },
  beforeDestroy() {
    document.removeEventListener('keydown', this.handleEscapeKey);
  }
}
</script>

<style scoped>
.modal.project {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 5;
}
.modal-content.project {
  background: white;
  padding: 20px;
  border-radius: 5px;
  position: relative;
}
.modalCert-close.project {
  position: absolute;
  top: 10px;
  right: 10px;
  background: none;
  border: none;
  font-size: 1.5em;
  cursor: pointer;
}
</style>