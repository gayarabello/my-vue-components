<script setup>
import VueButtonCollection from "@/components/molecules/VueButtonCollection.vue";
</script>

<template>
  <div id="app" style="margin: 0 auto; text-align: center;">
    <VueButtonCollection :buttons="[
      {
        msg:'You did it!',
        color:'blue',
        depressed: true
      },
      {
        msg:'Yeah yeah!',
        color:'red',
        depressed: false
      },
      {
        msg:'Okay dokey!',
        color:'aquamarine',
        depressed: true
      }
    ]"/>
  </div>
</template>

