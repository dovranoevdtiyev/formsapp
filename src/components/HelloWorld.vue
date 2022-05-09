<template>
  <form>
    <label>Email:</label>
    <input type="email" required v-model="email" />
    <label>Password:</label>
    <input type="password" required v-model="password" />
    <label for="">Role:</label>
    <select name="" id="">
      <option value="developer">Web designer</option>
      <option value="programmer">Web programmer</option>
    </select>
    <div id="terms">
      <input type="checkbox" required />
      <label>ACCEPT ALL TERMS AND CONDITIONS</label>
    </div>
    <div class="submit">
      <button>Create accaount</button>
    </div>
  </form>
  <p>Email:{{ email }}</p>
  <p>password:{{ password }}</p>
</template>

<script>
export default {
  data() {
    return {
      email: "",
      password: "",
    };
  },
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
form {
  max-width: 420px;
  margin: 30px auto;
  background: #dddd;
  text-align: left;
  padding: 40px;
  border-radius: 10px;
}
label {
  color: #aaaa;
  display: inline-block;
  margin: 25px 0 15px;
  font-size: 0.6cm;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: bold;
}
input,
select {
  display: block;
  padding: 10px 6px;
  width: 100%;
  box-sizing: border-box;
  border: none;
  border-bottom: 1px solid #ddd;
  color: #555;
}
input[type="checkbox"] {
  display: inline-block;
  width: 10px;
  margin: 0 10px 0 0;
  position: relative;
  top: 2px;
}
button {
  background: rgb(16, 77, 245);
  border: 0;
  padding: 10px 20px;
  margin-top: 20px;
  color: white;
  border-radius: 20px;
}
.submit {
  text-align: center;
}
</style>
