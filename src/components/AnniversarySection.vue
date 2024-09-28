<script >
export default {
  data() {
    return {

      anniversaryContent: [
        {
            id: 1,
            title: "Trinity Celebrates 50 Year Anniversary",
            desc1: "Through years of growth and change, Trinity remains committed to providing client responsiveness, specialty expertise, and quality technical work.",
            desc2: "For more details, please watch the video.",
            video: "https://www.youtube.com/watch?v=C0DPdy98e4c"
        },
        {
            id: 2,
            title: "The Origin of Trinity's Name",
            desc1: "Explore the origins of Trinity Consultants' name and the history of the Texas river that inspired it. Discover how our namesake river has shaped our global consulting expertise over the decades.",
            desc2: "Watch the video to learn more.",
            video: "https://www.youtube.com/watch?v=C0DPdy98e4c"
        }
      ]
      
    };
  }
};
</script>

<template>
<section class="section-anniversary-video">

<div class="flex-row grid lg:flex grid-cols-1 lg:grid-cols-2" v-for="asc in anniversaryContent" :key="asc.id">
<div class="section-anniversary-video__content">
    <h2>{{asc.title}}</h2>
    <p>{{asc.desc1}}</p>
    <p>{{asc.desc2}}</p>
</div>

<div>
    <video height="443" controls>
        <source :src="`${asc.video}`" type="video/mp4">
        Your browser does not support the video tag.
    </video>                  
</div>
</div>

</section>
</template>