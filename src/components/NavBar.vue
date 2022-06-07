<template>
  <nav>
    <router-link to="/" id="logo_props">
      <img :src="logo" :alt="alt" id="logo" />
    </router-link>
    <router-link to="/">Home</router-link> |
    <router-link to="/pedidos">Pedidos</router-link>
  </nav>
</template>


<script>
export default {
  name: "NavBar",
  props: ["logo", "alt"],
};
</script>

<style scoped>
nav {
  display: flex;
  background-color: #222;
  border-bottom: 4px solid #111;
  padding: 15px 50px;
  justify-content: flex-end;
  align-content: center;
}
#logo_props{
  margin: auto;
  margin-left: 0;
}
#logo{
  width: 40px;
  height: 40px;

}
nav a{
  text-decoration: none;
  color: #FCBA03;
  margin: 12px;
  transition: .5s;
}

nav a:hover{
  color: #FFFF;
}
</style>