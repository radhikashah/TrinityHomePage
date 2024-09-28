<script >
export default {
  data() {
    return {

      tcContent: [
        {
            id: 1,
            subtitle: "Upcoming Training",
            title: "Learn in-person, or online",
            desc1: "We provide a wide range of professional training on technical topics, taught by senior staff with extensive real-world experience.",
            btnLabel: "View Traiining",
            btnUrl: "https://www.trinityconsultants.com/",
            image: "training-carrer-image-1.png"
        },
        {
            id: 2,
            subtitle: "Career Opportunities",
            title: "Unlock your potential. Where will Trinity take you?",
            desc1: "With Trinity you can advance your career in the direction and at the pace you want. We will support you every step of the way with training, mentorship, and opportunities.",
            btnLabel: "Join Us",
            btnUrl: "https://www.youtube.com/watch?v=C0DPdy98e4c",
            image: "training-carrer-image-2.png"
        }
      ]
      
    };
  }
};
</script>

<template>
<section class="section-anniversary-video">

<div class="flex-row grid lg:flex grid-cols-1 lg:grid-cols-2" v-for="asc in tcContent" :key="asc.id">
<div class="section-anniversary-video__content">
    <h3>{{asc.subtitle}}</h3>
    <h2>{{asc.title}}</h2>
    <p>{{asc.desc1}}</p>
    <a class="btn btn-jasmine" href="`${asc.btnUrl}`">{{asc.btnLabel}}</a>
</div>

<div>
    <img :src="`./src/assets/${asc.image}`" alt="" />                
</div>
</div>

</section>
</template>