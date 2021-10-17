<template>
  <form @submit.prevent="handleSubmit">
    <h3>SignUp Form</h3>
    <div class="form-group">
      <label>First Name</label>
      <input
        type="text"
        class="form-control"
        v_model="first_name"
        placeholder="First Name"
      />
    </div>
    <div class="form-group">
      <label>Last Name</label>
      <input
        type="text"
        class="form-control"
        v_model="last_name"
        placeholder="Last Name"
      />
    </div>
    <div class="form-group">
      <label>Email</label>
      <input
        type="email"
        class="form-control"
        v_model="email"
        placeholder="Email"
      />
    </div>
    <div class="form-group">
      <label>Password</label>
      <input
        type="password"
        class="form-control"
        v_model="password"
        placeholder="Password"
      />
    </div>
    <div class="form-group">
      <label>Confirm Password</label>
      <input
        type="password"
        class="form-control"
        v_model="confirm_password"
        placeholder="Confirm Password"
      />
    </div>
    <button class="btn btn-primary btn-block">Sign Up</button>
  </form>
</template>

<script>
export default {
  name: "register",
  data() {
    return {
      first_name: "",
      last_name: "",
      email: "",
      password: "",
      password_confirm: "",
    };
  },
  methods: {
    handleSubmit() {
      const data = {
        first_name: this.first_name,
        last_name: this.last_name,
        email: this.email,
        password: this.password,
        password_confirm: this.password_confirm,
      };
      console.log(data);
    },
  },
  props: {
    data: String,
  },
};
</script>