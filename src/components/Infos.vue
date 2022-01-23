<template>
  <div>
      <!-- condicionais -->
    <p v-if="laboras">Estou laborando</p>
    <p v-else>Em busca de laboro</p>

    <p>Uso tecnoloogias:</p>
    <ul>
      <li :key="code" v-for="code in codes">{{code}}</li>
    </ul>

    <button @click="showEmail()">{{textoBotao}}</button>

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
          show_email: false,
          codes: ['JS', 'PHP', 'Python', 'Java', 'Typescript'],
          email: 'email@ex.com',
          linko: 'https://google.com',
          textoBotao: 'Show Email'
      }
  },
  methods: {
      showEmail(){
          this.show_email = !this.show_email
          if(this.show_email){
              this.textoBotao = "Ocultar Email"
          }else{
              this.textoBotao = "Mostrar Email"
          }
          
      }
  }
};
</script>