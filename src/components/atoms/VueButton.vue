<template>
  <button v-if="options" class="text-3xl font-bold underline"
    :style="`         
        border: ${options.depressed ? `2px solid ${options.color}` : 'none'};
        background-color:  ${options.depressed ? 'white' : options.color};
        color: ${options.depressed ? options.color : 'white'};
    `"
  >
    {{ options.msg }}
  </button>
</template>

<script>
export default {
  props: {
    options: {
    type: Object,
    required: true,
  }, 
  } 
};
</script>

<style>
button {
  padding: 1rem;
  border-radius: 0.5rem;
  cursor: pointer;
}
</style>




