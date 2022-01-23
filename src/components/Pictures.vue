<template>
  <!--alternativo v bind-->
  <div>
    <img :src="avatar" alt="" />
  </div>
</template>

<script>
export default {
  name: "Picture",
  data() {
    return {
      avatar: "/img/pixs.png",
      desc: "Fulano de tal",
    };
  },
};
</script>