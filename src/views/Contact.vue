<template>
  <div class="home">
    <h1>Contact Me</h1>
    <form action="handleSubmit">
      <input type="text" placeholder="Enter your name" />
      <input type="text" placeholder="Your email address" />
      <input type="text" placeholder="Your message" />
    </form>
  </div>
</template>

<script>
import Axios from "axios";

export default {
  name: "ContactView",
  data() {
    return {
      name: null,
      email: null,
      message: null
    };
  },
  methods: {
    handleSubmit() {
      event.preventDefault();

      const data = {
        email: this.email,
        message: this.message,
        name: this.name
      };

      Axios.post(
        `https://us-central1-${process.env.VUE_APP_FIREBASE_PROJECT_ID}.cloudfunctions.net/submit`,
        data
      )
        .then(res => {
          console.log("res", res);
          // here will be code
        })
        .catch(error => {
          console.log(error);
        });
    }
  }
};
</script>
