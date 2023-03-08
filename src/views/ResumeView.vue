<template>
  <div id="resume">

    <EducationVue :details="resume[0]"/>

    <SkillsVue :details="resume[1]"/>

  </div>
</template>

<script>
// @ is an alias to /src
import EducationVue from '@/components/EducationVue.vue'
import SkillsVue from '@/components/SkillsVue.vue'

export default {
  name: 'HomeView',
  components: {
    EducationVue,
    SkillsVue,
  },
  data() {
    return {
      resume: [
        {
          //Education
          secondarySchool: 'Wynberg Boys High School',
          qualification: 'National Senior Certificate',
          year: '2021',
          additionalAchievements: 'Chess Team',
          courses: [
            'Bergvliet High - Continuing Edecation',
            '- MS Excel Intermediate Course',
            '- MS Excel Advanced Course',
            'Life Choices Academy',
            '- 12 Month Coding Course'
          ],
        },
        {
          //Skills
          html: '90',
          css: '90',
          js: '80',
          bootstrap: '85',
          nodejs: '90',
          mysql: '85',
          vuejs: '90',
          excel: '65',
          softSkills: '85',
        }
      ]
    }
  },
}
</script>

<style scoped>
  h1, h2, h3, h4, h5, h6, p{
    word-wrap: break-word;
  }
  #resume {
    background-image: url(https://i.postimg.cc/Dz84Q2Dg/georgie-cobbs-unsplash-white-wall-desk.jpg);
  }
  .cv-btns {
    grid-column: 1/-1;
  }
</style>