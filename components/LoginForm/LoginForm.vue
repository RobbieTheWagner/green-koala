<template>
  <section>
    <b-field label="Username">
      <b-input
        placeholder="johnsmith10"
        type="text"
        v-model="username">
      </b-input>
    </b-field>

    <b-field label="Password">
      <b-input type="password"
               v-model="password"
               password-reveal>
      </b-input>
    </b-field>

    <button class="button is-info" @click="submit">Submit</button>
  </section>
</template>

<script>
  export default {
    data: () => ({
      username: null,
      password: null
    }),
    methods: {
      submit() {
      }
    }
  };
</script>
