<template>
  <div class="parent-component">
    <ChildComponent  @sent-text="displayText" />
    <br>
    <p>Texto recibido: {{ receivedText }}</p>
  </div>
</template>

<script>
import ChildComponent from "./ChildComponent.vue";

export default {
  components: {
    ChildComponent,
  },
  data() {
    return {
      receivedText: "",
    };
  },
  methods: {
    displayText(message) {
      this.receivedText = message;
    },
  },
};
</script>

<style scoped>

.parent-component{ 
  padding-top: 2%;
  padding-bottom: 2%;
}
</style>
