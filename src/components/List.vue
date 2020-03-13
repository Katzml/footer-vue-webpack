<template>
  <div class="box">
    <ul v-for="element in itemElements" :key="element.title">
      <Item :itemName="element.title" :itemLink="element.link" type="item-title"/>
      <div :class="element.line"></div>
      <Item v-for="item in element.items" :key="item.name" :itemName="item.name" :itemLink="item.itemLink" type="item"/>
    </ul>
  </div>
</template>

<script>
import Item from "./Item";
import elements from "../elements.json";
export default {
  name: "List",
  components: {
    Item
  },
  data() {
    return {
      itemElements: elements
    };
  }
};
</script>

<style scoped>
   .line-orange {
  padding-top: 0.1rem;
  width: 1.5em;
  margin-top: 0.4rem;
  height: 0.1em;
  background-color: #ff842c;
}

.line-blue {
  padding-top: 0.1rem;
  width: 1.5em;
  margin-top: 0.4rem;
  height: 0.1em;
  background-color: #4376b0;
}
.box {
margin-left: 1.2rem;
display: inline-grid;
}
.box ul {
  list-style: none;
  align-self: start;
}


</style>
