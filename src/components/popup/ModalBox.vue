<template>
  <div class="dizme_tm_modalbox opened">
    <div class="box_inner">
      <div class="close">
        <div class="close" @click.prevent="close">
          <a href="#"><i class="icon-cancel"></i></a>
        </div>
      </div>
      <div class="description_wrap"><slot></slot></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ModalBox",
  props: {
    close: { type: Function },
  },
  methods: {
    escListener(event) {
      if (event.key === 'Escape') {
        this.close();
      }
    }
  },
  mounted() {
    document.addEventListener('keydown', this.escListener);
  },
  beforeUnmount() {
    document.removeEventListener('keydown', this.escListener);
  },
};
</script>
