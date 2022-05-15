<template>
  <div>
    <h1>Profile</h1>
    <h1><img src="../assets/profile.png" width="250px" /></h1>
    <ul v-for="p in profile" :key="p.id">
      <li>Name : {{ p.name }} {{ p.lastName }}</li>
      <li>NickName : {{ p.nickName }}</li>
      <li>Age : {{ p.age }}</li>
      <li>Sduty at : {{ p.studyAt }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data: () => ({
    profile: [
      {
        name: "Natchanon",
        lastName: "Nilsuwan",
        nickName: "Mix",
        age: "21",
        studyAt: "KUSRC",
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