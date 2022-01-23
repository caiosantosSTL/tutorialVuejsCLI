<template>
    <NovoComponente/>
    <life-cycle/>
    <persono/>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue'
import NovoComponente from './components/NovoComponente.vue'
import Persono from './components/Persono.vue'
export default {
  components: { NovoComponente, LifeCycle, Persono },
  name: 'App'
}
</script>