<template>
  <div>
    <h1>Titulo</h1>

    <header>
      <slot name="header"></slot>
    </header>
    <main>
      <slot>{{ msg }}</slot>
    </main>
    <footer>
      <slot name="footer"></slot>
    </footer>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: {
      type: String,
      default: "Texto por default...",
      desc: "Evita que el botón pueda ser pulsado dos veces seguidas",
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  margin: 10px 0 0;
}
</style>
