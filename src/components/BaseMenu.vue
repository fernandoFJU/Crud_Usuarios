<template>
  <header>
    <a href="#" class="voltar" @click.prevent="$router.go(-1)">
      <img src="@/assets/arrow.svg" alt="Voltar" />
    </a>

    <div>
      <a
        href="#"
        class="usuario"
        title="Clique para deslogar"
        @click.prevent="deslogar"
      >
        Lucas ✌️
      </a>
    </div>
  </header>
</template>

<script>
export default {
  name: "BaseMenu",
  methods: {
    deslogar() {
      console.log("deslogar");
    },
  },
};
</script>

<style scoped>
header {
  padding: 15px 20px;
  min-height: 75px;
  border-bottom: 1px solid #ececec;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.voltar {
  background: #f7f7f7;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 45px;
  height: 45px;
  border-radius: 50%;
}
.voltar img {
  width: 20px;
}
.usuario {
  background: rgba(58, 85, 221, 0.2);
  border-radius: 5px;
  padding: 15px 20px;
  font-size: 14px;
  color: #3a55dd;
}
ul {
  display: flex;
  align-items: center;
  gap: 40px;
}
</style>