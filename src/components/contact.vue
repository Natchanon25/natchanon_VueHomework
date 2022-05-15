<template>
  <div>
    <h1>Contact</h1>
    <ul v-for="c in contact" :key="c.id">
      <li>Email : {{ c.email }} <br /></li>
      <li>Line Id : {{ c.lineID }} <br /></li>
    </ul>
  </div>
</template>

<script>
export default {
  data: () => ({
    contact: [
      {
        email: "natchanon.ni25@gmail.com",
        lineID: "25171205",
      },
    ],
  }),
};
</script>

<style>
h1 {
  text-align: center;
}
li {
  padding: 7px;
}
</style>