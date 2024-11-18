<template>
    <div class="content-list">
      <div v-for="(item, index) in contents" :key="index" class="content-item">
        <h3 v-if="item.title">{{ item.title }}</h3>
        <img v-if="item.image" :src="item.image" :alt="item.alt || 'Content Image'" />
        <p v-if="item.text1"><b>Project Overview:</b> {{ item.text1 }}</p>
        <p v-if="item.text2"><b>Services Provided:</b> {{ item.text2 }}</p>
        <p v-if="item.text3"><b>Outcome:</b> {{ item.text3 }}</p>
        
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "ContentList",
    props: {
      contents: {
        type: Array,
        required: true,
        default: () => [],
      },
    },
  };
  </script>
  
  <style scoped>
  .content-list {
    display: flex;
    flex-direction: column;
    gap: 16px;
  }
  
  .content-item {
    padding: 16px;
    border-radius: 8px;
  }
  
  .content-item h3 {
    margin: 0 0 8px;
    text-shadow: -2px -2px #0A100DA3;
    
  }
  
  .content-item p {
    margin: 10px 0 12px;
    text-align: left;
    text-shadow: 2px 2px #0A100DA3;
  }
  
  .content-item img {
    max-width: max-content;
    border-radius: 4px;
  border: solid #0A100DA3;
  }
  </style>
  