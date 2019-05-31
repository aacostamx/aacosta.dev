<template>
  <section id="home-languages" class="py-3 bg-medium">
    <div class="container">
      <h2 class="section-title">I have experience</h2>
      <div class="bottom-line"></div>
      <p class="lead">Working with</p>

      <div class="home-languages">
        <div v-for="logo in technologies" :key="logo">
          <img :src="logo" style="max-width: 5.7rem;">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import aws from "../assets/icons/amazonwebservices/amazonwebservices-original-wordmark.svg";
import angularjs from "../assets/icons/angularjs/angularjs-plain.svg";
import bitbucket from "../assets/icons/bitbucket/bitbucket-original-wordmark.svg";
import bootstrap from "../assets/icons/bootstrap/bootstrap-plain-wordmark.svg";
import chrome from "../assets/icons/chrome/chrome-plain.svg";
import csharp from "../assets/icons/csharp/csharp-plain.svg";
import css from "../assets/icons/css3/css3-plain-wordmark.svg";
import docker from "../assets/icons/docker/docker-plain.svg";
import dotnet from "../assets/icons/dot-net/dot-net-plain-wordmark.svg";
import facebook from "../assets/icons/facebook/facebook-plain.svg";
import firefox from "../assets/icons/firefox/firefox-plain.svg";
import git from "../assets/icons/git/git-plain.svg";
import google from "../assets/icons/google/google-original.svg";
import html from "../assets/icons/html5/html5-plain-wordmark.svg";
import jquery from "../assets/icons/jquery/jquery-plain-wordmark.svg";
import less from "../assets/icons/less/less-plain-wordmark.svg";
import mysql from "../assets/icons/mysql/mysql-original-wordmark.svg";
import npm from "../assets/icons/npm/npm-original-wordmark.svg";
import postgress from "../assets/icons/postgresql/postgresql-plain-wordmark.svg";
import react from "../assets/icons/react/react-original.svg";
import redis from "../assets/icons/redis/redis-plain.svg";
import sass from "../assets/icons/sass/sass-original.svg";
import slack from "../assets/icons/slack/slack-original.svg";
import sourcetree from "../assets/icons/sourcetree/sourcetree-original-wordmark.svg";
import typescript from "../assets/icons/typescript/typescript-plain.svg";
import trello from "../assets/icons/trello/trello-plain-wordmark.svg";
import ubuntu from "../assets/icons/ubuntu/ubuntu-plain-wordmark.svg";
import visualstudio from "../assets/icons/visualstudio/visualstudio-plain.svg";
import vuejs from "../assets/icons/vuejs/vuejs-original-wordmark.svg";
import webpack from "../assets/icons/webpack/webpack-plain.svg";
import win from "../assets/icons/windows8/windows8-original.svg";
import wordpress from "../assets/icons/wordpress/wordpress-plain.svg";
// import oracle from "../assets/icons/oracle/oracle-original.svg";
// import photoshop from "../assets/icons/photoshop/photoshop-line.svg";
// import android from "../assets/icons/android/android-plain.svg";
// import github from "../assets/icons/github/github-original-wordmark.svg";
// import js from "../assets/icons/javascript/javascript-original.svg";
// import linux from "../assets/icons/linux/linux-plain.svg"
// import apple from "../assets/icons/apple/apple-original.svg";
// import babel from "../assets/icons/babel/babel-original.svg";

export default {
  data() {
    return {
      logos: [
        aws,
        angularjs,
        bitbucket,
        bootstrap,
        chrome,
        csharp,
        css,
        docker,
        dotnet,
        facebook,
        firefox,
        git,
        google,
        html,
        jquery,
        less,
        mysql,
        npm,
        postgress,
        react,
        redis,
        sass,
        slack,
        sourcetree,
        typescript,
        trello,
        ubuntu,
        visualstudio,
        vuejs,
        webpack,
        win,
        wordpress
        // android,
        // oracle,
        // photoshop,
        // babel,
        // apple,
        // js,
        // github,
        // linux,
      ]
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