<script setup>
import IconArrow from './icons/IconArrow.vue'
import IconPdf from './icons/IconPdf.vue'
</script>
<script >

import { allprojects } from './../data/AllProjects.js';

export default {
  data() {
    return {
      allprojects // assign imported contacts to local data
    };
  }
};
</script>


<template>
<div class="py-12">
    <section>
    <div class="content-wrapper">
        <div class="cw-wrap">
            <div class="cw--title">
                <div class="cw--title__wrapper block md:flex items-end">
                    <div>
                        <h3 class="cw--title__subtitle uppercase">Featured Projects </h3>
                        <h2 class="cw--title__title">Solving Complex Problems</h2>
                    </div>
                    <div class="text-left md:text-right">
                        <a class="btn btn--link flex items-center" href="https://www.trinityconsultants.com/resources?ds%5B0%5D=ResourceType%7CCase%20Study&amp;sbt=&amp;rs%5Bmin%5D=978346622444&amp;rs%5Bmax%5D=1695677252497&amp;pg=1&amp;drp=DatePublished%20desc" target="_self" aria-label="VIEW ALL PROJECTS">
                            <span>VIEW ALL PROJECTS</span>
                            <IconArrow />
                        </a>
                    </div>
                </div>
            </div>
            <div class="feature-list flex justify-between h-screenflex flex-row gap-x-5 px-2 align-top grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4">
                    <div class="card"  v-for="allproject in allprojects" :key="allproject.id">
                        <figure>
                                    <img :src="`./src/assets/${allproject.image}`" alt="" class="object-cover" width="100%" height="150">
                        </figure>
                        <div class="card__body">
                            <h4>{{allproject.title}}</h4>
                            <p>{{allproject.desc}}</p>
                        </div>
                        <div class="card__footer">
                            <a class="flex items-center flex-end uppercase" href="https://tciglobalcdn.azureedge.net/tciwebsiteresources/docs/default-source/case-study/frazier-collaborates-with-trinity-consultants_cs_ec.pdf" aria-label="Read More" target="_blank">
                                <IconPdf />
                                <span>Read More</span>
                            </a>
                        </div>
                    </div>
                    
                                       
            </div>
        </div>
    </div>
</section>
</div>
</template>