<template>
<section class="foo-fragment">
    <List/>
</section>

</template>

<script>
import List from './List'
export default {
    name:"Layout",
    components:{
        List
    }

}
</script>

<style scoped>

.foo-fragment {
  font-family: Helvetica;
  display: grid;
  grid-template-columns: repeat(4,1fr);

}

</style>