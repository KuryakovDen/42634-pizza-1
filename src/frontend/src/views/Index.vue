<template>
  <div>
    <p>{{ user.name }}</p>
    <p>{{ pizza.dough[0].name }}</p>
    <p>{{ misc[0].name }}</p>
  </div>
</template>
<script>
import user from "@/static/user.json";
import pizza from "@/static/pizza.json";
import misc from "@/static/misc.json";

export default {
  name: "Index",
  data() {
    return {
      user,
      pizza,
      misc,
    };
  },
};
</script>
<style></style>
