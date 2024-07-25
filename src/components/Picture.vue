<template>
  <img :src="avatar" :alt="descricao" />
  <MudarImagem @mudar-imagem="TrocarImagem" />
</template>
<script>
import MudarImagem from "./MudarImagem.vue";

export default {
  name: "Picture",
  components: {
    MudarImagem,
  },
  data() {
    return {
      avatar: "/img/avatar.png",
      descricao: "Patricia Adania",
    };
  },
  methods: {
    TrocarImagem() {
      this.avatar = "/img/avatar2.png";
    },
  },
};
</script>
