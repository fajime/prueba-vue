<template>
  <div @click="onClick">Contenido de productos</div>
</template>
<script>
export default {
  name: "PepeLibre",
  props: {
    nombre: {
      type: String,
      default: "Marca desconocida...",
    },
  },
  mounted() {
    this.init();
  },
  methods: {
    /**
     *  init component
     */
    init() {
      console.log("Init ......");
    },
    /**
     * Capture the `click` event and emit the event itself.
     *
     * @param {event} event The native click event.
     */
    onClick(event) {
      console.log(event);
      // if (this.once) {
      //   if (this.onceInProcess) {
      //     clearTimeout(this.onceTimeoutId);
      //   } else {
      //     this.$emit("clicked", event);
      //     this.onceInProcess = true;
      //   }
      //   this.onceTimeoutId = setTimeout(
      //     () => (this.onceInProcess = false),
      //     Number(this.onceTime)
      //   );
      // } else {
      //   this.$emit("clicked", event);
      // }
    },
  },
};
</script>
