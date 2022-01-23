<template>
    <NovoComponente/>
    <life-cycle/>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue'
import NovoComponente from './components/NovoComponente.vue'
export default {
  components: { NovoComponente, LifeCycle },
  name: 'App'
}
</script>