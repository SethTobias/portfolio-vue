<template>
  <div v-if="isVisible" class="modal cert" @click="handleOverlayClick">
    <div class="modal-content cert" @click.stop>
      <button class="modal-close cert" @click="close">×</button>
      <h2>{{ title }}</h2>
      <p>{{ msg }}</p>
      <p>
        <a :href="{ github }">HitHub</a> | 
        <a :href="{ link }">Hosted Link</a>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CertModal',
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
    },
    github: {
      type: String,
      default: ''
    },
    link: {
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
.modal.cert {
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
.modal-content.cert {
  background: white;
  padding: 20px;
  border-radius: 5px;
  position: relative;
}
.modalCert-close.cert {
  position: absolute;
  top: 10px;
  right: 10px;
  background: none;
  border: none;
  font-size: 1.5em;
  cursor: pointer;
}
</style>