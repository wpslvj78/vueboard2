<template>
  <div role="tablist">
    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-1 variant="danger">1</b-button>
      </b-card-header>
      <b-collapse id="accordion-1" visible accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text></b-card-text>
          <b-card-text>
            <img src='../static/p1.jpg' alt='pic1'/> 
          <!-- <b-img :src="require('../static/pic1.jpg')" alt='pic1'></b-img> -->
          {{ text }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-2 variant="danger">2</b-button>
      </b-card-header>
      <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>
           <img src='../static/p2.jpg' alt='pic2'/>
          {{ text2 }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-3 variant="danger">3</b-button>
      </b-card-header>
      <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>
          <img src='../static/p4.jpg' alt='pic3'/>
          {{ text3 }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
    
  </div>
  
</template>

<script>
  export default {
    data() {
      return {
        text: `
         비에고입니다~
        `,
        text2: `
         판테온입니다~
        `,
        text3: `
         세나입니다~
        `
      }
    }
  }
</script>