<template>
  <div>
    <header class="header">
      <div class="header__logo">
        <a href="index.html" class="logo">
          <img
            src="@/assets/img/logo.svg"
            alt="V!U!E! Pizza logo"
            width="90"
            height="40"
          />
        </a>
      </div>
      <div class="header__cart">
        <a href="cart.html">0 ₽</a>
      </div>
      <div class="header__user">
        <a href="#" class="header__login"><span>Войти</span></a>
      </div>
    </header>
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
