<template>
  <section id="about-tech" class="bg-dark py-3">
    <div class="container">
      <h2 class="section-title">Technical Skills</h2>
      <div class="bottom-line"></div>
      <div class="areas">
        <div v-for="(skill, index) in skills" :key="index">
          <h4>{{skill.title}}:</h4>
          <div class="progress">
            <div :style="`width: ${skill.percentage}%`"></div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        {
          title: ".NET",
          percentage: 90
        },
        {
          title: "SQL Database",
          percentage: 90
        },
        {
          title: "HTML & CSS",
          percentage: 90
        },
        {
          title: "Javascript",
          percentage: 80
        },
        {
          title: "Angular",
          percentage: 80
        },
        {
          title: "React",
          percentage: 80
        },
        {
          title: "Vue",
          percentage: 80
        },
        {
          title: "Azure DevOps",
          percentage: 90
        },
        {
          title: "Microsoft Azure",
          percentage: 90
        },
        {
          title: "AWS Cloud",
          percentage: 80
        },
        {
          title: "Google Cloud Platform",
          percentage: 70
        },
        {
          title: "UX Design",
          percentage: 60
        },
        {
          title: "Scrum",
          percentage: 90
        },
        {
          title: "Automation Testing",
          percentage: 70
        },
        {
          title: "Unit Testing",
          percentage: 90
        }
      ]
    };
  }
};
</script>
