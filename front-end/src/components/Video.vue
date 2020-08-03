<template>
  <div id="Video">
    <section class="hero ">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">
             <img src="../assets/icon.png">
          </h1>
          <h2 class="subtitle">
          Conteúdos em video de uma forma fácil e simples
          </h2>
      <div class="input-group">
          <input type="search" class="input is-primary"  v-model="busca" placeholder="Buscar">
          <button class="button is-info is-rounded">Buscar</button>
      </div>
    </div>
  </div>
</section>
    <div class="row"> 
        <!-- <button type="button" class="btn btn-danger" @click="getData">Get Data</button> -->
        <br>
        <br>
    </div>   
    <div style="margin-left:100px; background-color:#7C56F6; whidth:900px; height=900; float:left">
      <div class="col-11 border-left" v-for="v1 in buscaV1" :key="v1.title">
        <iframe
            width="560"
            height="315"
            src="https://www.youtube.com/embed/XDdaaIziT2Y"
            frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
      </div>
    </div>

      <br>

      <div style="margin-rigth:100px; background-color:#7C56F6; whidth:900px; height=900; float:right">
        <div class="col-11 border-left" v-for="v2 in buscaV2" :key="v2.title">
          <iframe
              width="560"
              height="315"
              src="https://www.youtube.com/embed/sn_VZDrz3m0"
              frameborder="0"
              allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
              allowfullscreen
            ></iframe>
        </div>
      </div>
      
      <br>

      <div style="margin-left:100px; background-color:#7C56F6; whidth:900px; height=900; float:left">
        <div class="col-11 border-left" v-for="v3 in buscaV3" :key="v3.title">
          <iframe
              width="560"
              height="315"
              src="https://www.youtube.com/embed/gqSms6LqSso"
              frameborder="0"
              allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
              allowfullscreen
            ></iframe>
        </div>
      </div>

      <br>

      <div style="margin-rigth:100px; background-color:#7C56F6; whidth:900px; height=900; float:right">
        <div class="col-11 border-left" v-for="v4 in buscaV4" :key="v4.title">
            <iframe
            width="560"
            height="315"
            src="https://www.youtube.com/embed/lKTDiT_jeWc"
            frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
      </div>

      <br>

       <div style="margin-left:100px; background-color:#7C56F6; whidth:900px; height=900; float:left">
        <div class="col-11 border-left" v-for="v5 in buscaV5" :key="v5.title">
          <iframe
            width="560"
            height="315"
            src="https://www.youtube.com/embed/Wzm9Evh9lJ8"
            frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
       </div>

       <br>

       <div style="margin-right:100px; background-color:#7C56F6; whidth:900px; height=900; float:right">
        <div class="col-11 border-left" v-for="v6 in buscaV6" :key="v6.title">
            <iframe
            width="560"
            height="315"
            src="https://www.youtube.com/embed/B9mO-XXHASA"
            frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
       </div>

       <br>

       <div style="margin-left:100px; background-color:#7C56F6; whidth:900px; height=900; float:left">
        <div class="col-11 border-left" v-for="v7 in buscaV7" :key="v7.title">
            <iframe
            width="560"
            height="315"
            src="https://www.youtube.com/embed/KW2P5i7hSEk"
            frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
       </div>

       <br>

       <div style="margin-right:100px; background-color:#7C56F6; whidth:900px; height=900; float:right">
        <div class="col-11 border-left" v-for="v8 in buscaV8" :key="v8.title">
            <iframe
            width="560"
            height="315"
            src="https://www.youtube.com/embed/A5e1ellYSz8"
            frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
       </div>
  </div>  
</template>

<script>
export default {
  name: "Video",
  data() {
    return {
      busca: "",
      v1: [
        {
          title: "Anatomia cardiovascular: Pericárdio"
        }
      ],

      v2: [
        {
          title: "Anatomia do sistema digestório: Estômago"
        }
      ],

       v3: [
        {
          title: "Semio Neurológica: sensibilidade profunda"
        }
      ],

       v4: [
        {
          title: "Semiologia Cardiovascular - Manobra Vagal"
        }
      ],
        v5: [
        {
          title: "Anatomia cardiovascular: Valvas Arteriais"
        }
      ],

      v6: [
        {
          title: "Neuroanatomia - embriologia vestindo o jaleko"
        }
      ],

      v7: [
        {
          title: "Introdução à anatomia cardíaca"
        }
      ],

      v8: [
        {
          title: "Anatomia cardíaca - Anatomia externa"
        }
      ]
  
    };
  },
  computed: {

    buscaV1() {
      return this.busca
        ? this.v1.filter(v1 => {
            return v1.title.includes(this.busca);
          })
        : this.v1;
    },

    buscaV2() {
      return this.busca
        ? this.v2.filter(v2 => {
            return v2.title.includes(this.busca);
          })
        : this.v2;
    },

    buscaV3() {
      return this.busca
        ? this.v3.filter(v3 => {
            return v3.title.includes(this.busca);
          })
        : this.v3;
    },

     buscaV4() {
      return this.busca
        ? this.v4.filter(v4 => {
            return v4.title.includes(this.busca);
          })
        : this.v4;
    },

     buscaV5() {
      return this.busca
        ? this.v5.filter(v5 => {
            return v5.title.includes(this.busca);
          })
        : this.v5;
    },

     buscaV6() {
      return this.busca
        ? this.v6.filter(v6 => {
            return v6.title.includes(this.busca);
          })
        : this.v6;
    },

     buscaV7() {
      return this.busca
        ? this.v7.filter(v7 => {
            return v7.title.includes(this.busca);
          })
        : this.v7;
    },

     buscaV8() {
      return this.busca
        ? this.v8.filter(v8 => {
            return v8.title.includes(this.busca);
          })
        : this.v8;
    }

  },


  methods: {
    getData() {}
  }
};
</script>

<style scoped>
  
 

</style>>



