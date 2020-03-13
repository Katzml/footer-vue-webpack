<template>
<li :class="type"><a :href="itemLink" v-text="itemName"></a></li>
</template>

<script>
export default {
    name:"Item",
    props:{
        itemName:String,
        itemLink:String,
        type:String,
    }

}
</script>
<style scoped>
.item {
  font-size: 0.8em;
  margin-top: 0.9rem;
  margin-bottom: 0.9rem;
}

.item-title {
  font-weight: bold;
  font-size: 0.876em;
}
li a:link,
a:visited {
  text-decoration: none;
  color: black;
}

li a:hover {
  font-weight: bold;
}

</style>