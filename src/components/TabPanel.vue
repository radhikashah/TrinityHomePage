<script >

import { tabdata } from './../data/TabData.js';

export default {
  data() {
    return {
      currentTab: 0,
      tabdata,
      activeSection: 0,
    };
  },
    methods: {
        toggleSection(index) {
            this.activeSection = index;
            console.log('activesection => ', this.activeSection)
        },
    }
  }
  
</script>



<template>
<section class="overflow-hidden">

<div class="tabs__wrap">
            <div class="tabs__inner">
                <div class="tabs js-tabs is-initialized tabs-allowed" data-start-collapsed="true">
                    <div class="tabs__tab-list hidden lg:block">
                        <ul class="tabs__tab-list-items" role="tablist">
                                <li :class="['tabs__tab-list-trigger accent--seafoam', { active: currentTab === tb.id }]" v-for="tb in tabdata" :key="tb.id" @click="currentTab = tb.id" role="presentation">
                                    <a class="js-tabs-trigger"  role="tab">
                                        <span>{{tb.title}}</span>
                                    </a>
                                </li>
                        </ul>
                    </div>
                        <section v-if="tabdata[currentTab]" :class="['tabs__panel js-tabs-panel hidden lg:block', `${tabdata[currentTab].bgclass}`]" 
                            
                        >
                            <div class="tabs__accordion-trigger js-accordion-trigger">
                                <div class="tabs__accordion-trigger__title"><span>{{tabdata[currentTab].title}}</span></div>
                                <div class="tabs__accordion-trigger-icon">
                                    <span class="label--open">Open</span><span class="label--close">Close</span>
                                    <svg aria-hidden="true" focusable="false" viewBox="0 0 20 20">
                                        <rect class="vert" height="18" width="2" fill="currentColor" y="1" x="9"></rect>
                                        <rect height="2" width="18" fill="currentColor" y="9" x="1"></rect>
                                    </svg>
                                </div>
                            </div>
                            <div class="tabs__panel-content js-tabs-content">
                                <div class="tabs__panel-content-image"><img :src="`./src/assets/${tabdata[currentTab].image}`" width="1730" height="825" alt="" loading="lazy" style="--width: 600; --height: 400;"></div>
                                <div class="tabs__panel-content-body">
                                    <h2>{{tabdata[currentTab].title}}</h2>
                                    <p>{{tabdata[currentTab].desc}}</p>
                                    <a class="btn btn--secondary" href="/consulting/ehs" aria-label="Environmental Consulting">View Our Capabilities</a>
                                </div>
                            </div>
                        </section>

                        <section v-for="(tb, index) in tabdata" :key="index" :class="['block lg:hidden js-tabs-panel tabs__panel ', `${tb.bgclass}`]" 
                            
                        >
                            <div class="tabs__accordion-trigger js-accordion-trigger">
                                <div class="tabs__accordion-trigger__title" @click="toggleSection(index)"><span>{{tb.title}}</span></div>
                                <div class="tabs__accordion-trigger-icon">
                                    <span class="label--open">Open</span><span class="label--close">Close</span>
                                    <svg aria-hidden="true" focusable="false" viewBox="0 0 20 20">
                                        <rect class="vert" height="18" width="2" fill="currentColor" y="1" x="9"></rect>
                                        <rect height="2" width="18" fill="currentColor" y="9" x="1"></rect>
                                    </svg>
                                </div>
                            </div>
                            <div class="tabs__panel-content js-tabs-content" v-show="activeSection === index" >
                                <div class="tabs__panel-content-image"><img :src="`./src/assets/${tb.image}`" width="1730" height="825" alt="" loading="lazy" style="--width: 600; --height: 400;"></div>
                                <div class="tabs__panel-content-body">
                                    <h2>{{tb.title}}</h2>
                                    <p>{{tb.desc}}</p>
                                    <a class="btn btn--secondary" href="/consulting/ehs" aria-label="Environmental Consulting">View Our Capabilities</a>
                                </div>
                            </div>
                        </section>
</div>
</div>

</div>
</section>
</template>


