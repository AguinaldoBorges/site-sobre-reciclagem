<template>
    <div class="container-fluid">
      <!-- center -->
      <div class="row">
          <div class="col-12">
            <h1 id="text-template" :style="`color:${color}`">{{text}}<span :style="`color:${destakColor}`">{{destakText}}</span><span>{{text2}}</span></h1>
          </div>
      </div>
    </div>
  </template>

  <script>
  export default {
    props:{
        text:{},
        destakText:{},
        text2:{},
        color:{},
        destakColor:{}
    }

  }
  </script>

  <style>
  #text-template{
    font-weight: 100;
    font-size: 26px;
  }

  </style>