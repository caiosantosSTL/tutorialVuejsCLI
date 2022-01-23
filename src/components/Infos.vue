<template>
  <div>
      <!-- condicionais -->
    <p v-if="laboras">Estou laborando</p>
    <p v-else>Em busca de laboro</p>

    <p>Uso tecnoloogias:</p>
    <ul>
      <li :key="code" v-for="code in codes">{{code}}</li>
    </ul>
    <p v-show="show_email">Mande um email para: {{email}}</p>
  </div>
</template>

<script>
export default {
  name: "Infos",
  data(){
      return{
          laboras: true,
          show_email: true,
          codes: ['JS', 'PHP', 'Python', 'Java', 'Typescript'],
          email: 'email@ex.com'
      }
  }
};
</script>