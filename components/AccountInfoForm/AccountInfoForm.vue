<template>
  <form-schema :schema="schema" v-model="model" @submit="submit">
    <button type="submit">Submit</button>
  </form-schema>
</template>

<script>
  import FormSchema from 'vue-json-schema';
  import schema from './schema.json';

  export default {
    data: () => ({
      schema,
      model: {}
    }),
    methods: {
      submit(e) {
        // this.model contains the valid data according your JSON Schema.
        // You can submit your model to the server here
      }
    },
    components: { FormSchema }
  };
</script>

<style>
  input {
    display: block;
  }
</style>
