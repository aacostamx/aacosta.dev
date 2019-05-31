<template>
  <section id="home-specialize" class="py-3 bg-light">
    <div class="container">
      <h2 class="section-title">I'm an expert in</h2>
      <div class="bottom-line"></div>
      <p class="lead">Web Applications with Javascript frameworks like Angular, React, Vue and .NET Core</p>
      <div class="home-languages" style="text-align: center;">
        <div v-for="logo in technologies" :key="logo">
          <img :src="logo" style="max-width: 15rem;">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import net from "../assets/icons/dot-net/dot-net-original-wordmark.svg";
import angular from "../assets/icons/angularjs/angularjs-original.svg";
import css from "../assets/icons/css3/css3-original.svg";
import html from "../assets/icons/html5/html5-original.svg";
import react from "../assets/icons/react/react-original.svg";
import vue from "../assets/icons/vuejs/vuejs-original.svg";

export default {
  data() {
    return {
      logos: [angular, css, html, react, vue, net]
    };
  },
  computed: {
    technologies() {
      const technologies = this.logos.slice(0);
      technologies.sort(function() {
        return 0.5 - Math.random();
      });

      return technologies;
    }
  }
};
</script>
