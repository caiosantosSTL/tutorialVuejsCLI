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
    <!-- uso de v-bind -->
    <p>Para ir ao meu portfolio <a v-bind:href="linko" target="_blank">Aqui</a> </p>
    <pictures/>
  </div>
</template>

<script>
import Pictures from './Pictures.vue';
export default {
  components: { Pictures },
  name: "Infos",
  data(){
      return{
          laboras: true,
          show_email: true,
          codes: ['JS', 'PHP', 'Python', 'Java', 'Typescript'],
          email: 'email@ex.com',
          linko: 'https://google.com'
      }
  }
};
</script>