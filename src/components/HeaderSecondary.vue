<template>
  <div class="header-content">
    <h1>
      I AM
      <span class="txt-type" ref="writer"></span>
    </h1>
    <p class="lead">{{ lead }}</p>
    <a v-if="showViewMyWork" href="/" class="btn-light">View My Work</a>
  </div>
</template>

<script>
import TypeWriter from "../utils/typewriter";
export default {
  data() {
    return {
      words: [
        "SOFTWARE ARCHITECT",
        "ANGULAR SPECIALIST",
        "VUE MASTER",
        "FULL STACK DEVELOPER",
        "REACT EXPERT",
        "SOFTWARE DEVELOPER",
        "SOFTWARE ENGINEER"
      ],
      wait: 3000,
      lead: `I'm an expert in web applications with javascript frameworks like Angular, Vue and React`,
      showViewMyWork: false
    };
  },
  mounted() {
    new TypeWriter(this.$refs.writer, this.words, this.wait);
  }
};
</script>

