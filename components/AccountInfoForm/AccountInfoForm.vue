<template>
  <section>
    <b-field label="Name">
      <b-input
        placeholder="John Smith"
        type="text"
        v-model="name">
      </b-input>
    </b-field>

    <b-field label="Age">
      <b-input
        min="0"
        placeholder="36"
        type="number"
        v-model="age">
      </b-input>
    </b-field>

    <b-field label="Email">
      <b-input
        placeholder="johnsmith@website.com"
        type="email"
        v-model="email">
      </b-input>
    </b-field>

    <button class="button is-info" @click="submit">Submit</button>
  </section>
</template>

<script>
  export default {
    data: () => ({
      age: null,
      email: null,
      name: null
    }),
    methods: {
      submit() {
      }
    }
  };
</script>
