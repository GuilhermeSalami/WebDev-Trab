<template>
  <v-app id="inicio">
    <NavBar />
    <v-container fluid>
      <div class="box">
        <v-row>
            <v-col cols="5">
              <div style="position: relative" class="mt-16">
                <h1 class="text-white">Kiryu Kazuma</h1>
                <span class="text-white">Guarda Costas</span><br/>
                <v-btn title dark class="text-white mt-8" variant="outlined">Me Contate</v-btn>
              </div>
            </v-col>
          <v-col cols="7">
            <div style="position: absolute; bottom: 0; z-index:9999;" class="mt-16">
              <v-img src="Kiryu_terno.png" contain max-height="350"></v-img>
            </div>
          </v-col>
        </v-row>
      </div>
      <v-col cols="12" class="mt-16" id="sobre">
        <div>
          <v-row>
            <v-col cols="12" sm="6">
              <div class="like_a_dragon">
                <v-img src="y7_logo_tm.png" contain max-height="400"></v-img>
              </div>
            </v-col>
            <v-col cols="12" sm="6">
              <h1 class="mt-16">Sobre mim</h1>
              <div style="width: 120px"><br/>
              </div>
              <h4 class="mt-n4">Melhor Guarda Costas de Kamurocho</h4>
              <h4 class="">Ex-Yakuza</h4>
              <p class="text-black">
                  Entrei na família Kazama aos 20 anos de idade. Shintaro Kazama, meu chefe e também minha figura paterna,
                reconheceu meu valor. Após o incidente do Lote Vazio, fui promovido para a família Dojima. Contudo, as coisas
                desandaram quando tive que assumir o assassinato de Dojima Sohei, chefe do Clã Dojima, para salvar a vida de meu irmão, Akira Nishikiyama.
                Passei 10 anos na prisão e após isso, tudo mudou.
              </p>
              <br/>
              <p class="text-black">
                Ao longo de 30 anos de carreira na Yakuza, enfrentei muitas adversidades e inimigos, ao ponto de lutar contra 100 adversãrios e vencer. Atualmente,
                sou um mero guarda costas.
              </p>
              <v-btn tile dark color="#d50000" class="mt-4">
                Baixe o resumo
              </v-btn>
            </v-col>
          </v-row>
        </div>
      </v-col>
      
      <div class="text-center mt-4">
        <h1>O que eu faço</h1>
        <div style="width: 120px; margin: 0 auto">
        </div>
      </div>
      <v-col cols="12" class="padd" id="portfolio">
        <div class="first" id="project">
          <v-row>
            <v-col cols="12">
              <div class="child">
                <v-btn
                  icon="fas fa-hand-fist"
                  color="#d50000"
                  class="text-white"
                ></v-btn>
                <h3 class="ml-3 mt-4">Combate</h3>
                <p class="text-black ml-3 mt-4 text-caption">
                  Extremamente forte <br/>Bom de briga
                  <br/>Vários estilos de luta
                </p>
              </div>
              <div class="child">
                <v-btn
                  icon="fas fa-shield"
                  color="#d50000"
                  class="text-white"
                ></v-btn>
                <h3 class="ml-3 mt-4">Perseverança</h3>
                <p class="text-black ml-3 mt-4 text-caption">
                  Super resistente <br/> Inabalável
                  <br/>Levanta sempre
                </p>
              </div>
              <div class="child">
                <v-btn
                  icon="fas fa-heart"
                  color="#d50000"
                  class="text-white"
                ></v-btn>
                <h3 class="ml-3 mt-4">Índole</h3>
                <p class="text-black ml-3 mt-4 text-caption">
                  Dono de orfanato <br/>Pai
                  <br/>Faz tudo pelos amigos
                </p>
              </div>
            </v-col>
          </v-row>
          <v-divider></v-divider>
        </div>
      </v-col>
      <v-col cols="12" sm="12" id="serviços">
        <div class="d-flex justify-center mb-6">
          <v-btn color="#d50000" class="mr-2">Tudo</v-btn>
          <v-btn class="mr-2" variant="tonal">Combate</v-btn>
          <v-btn class="mr-2" variant="tonal">Perseverança</v-btn>
          <v-btn class="mr-2" variant="tonal"> Índole</v-btn>
          <v-btn variant="tonal"> Carreira</v-btn>
        </div>
      </v-col>
      <v-col cols="12" class="imgHover">
        <v-row class="fill-height" align="center" justify="center">
          <template v-for="(item, i) in items" :key="i">
            <v-col cols="12" md="4">
              <v-hover v-slot="{ isHovering, props }">
                <v-card
                  :elevation="isHovering ? 12 : 2"
                  :class="{ 'on-hover': isHovering }"
                  v-bind="props"
                >
                  <v-img :src="item.img" height="200px" cover> </v-img>
                </v-card>
              </v-hover>
            </v-col>
          </template>
        </v-row>
      </v-col>
      <v-col cols="12" sm="12">
        <div class="d-flex justify-center mb-6">
          <v-btn color="#d50000" class="mt-4">Carregar mais</v-btn>
        </div>
      </v-col>
      <v-col cols="12" id="extra">
        <div class="pre">
          <v-row>
            <v-col cols="12" sm="4">
              <v-card class="mx-auto" max-width="344" height="">
                <v-img src="erased.png" height="200px" cover></v-img>

                <v-card-title> Serviços para todos </v-card-title>

                <v-card-subtitle>
                  Joryu | 8 Nov 2023
                </v-card-subtitle>
                <v-card-text>
                  Para aqueles que não têm para quem recorrer.
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card class="mx-auto" max-width="344" height="">
                <v-img src="daigo.jpg" height="200px" cover></v-img>

                <v-card-title> Clientes aprovam </v-card-title>

                <v-card-subtitle>
                  Daigo Dojima | 22 Dec 2019
                </v-card-subtitle>
                <v-card-text>
                  Ex Chefe do Clã Tojo.
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card class="mx-auto" max-width="344" height="">
                <v-img src="watase.jpg" height="200px" cover></v-img>

                <v-card-title> Até estranjeiros aceitam </v-card-title>

                <v-card-subtitle>
                  Masaru Watase | 22 Dec 2019
                </v-card-subtitle>
                <v-card-text>
                  Ex Chefe da Aliança Omi.
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <v-col cols="12" sm="12" class="px-16" id="contato">
        <v-row>
          <v-col cols="12" sm="4">
            <div class="child">
              <h1>Informações de Contato</h1>
              <v-btn
                icon="fas fa-location-dot"
                color=""
                class="mt-10"
                variant="outlined"
              ></v-btn
              ><br/>
              <span class="text-caption">Kamurocho, Distrito de Tokyo </span
              ><br/>
              <v-btn
                icon="fas fa-phone"
                color=""
                class="mt-10"
                variant="outlined"
              ></v-btn
              ><br/>
              <span class="text-caption">(81)9999-9999 </span> <br/>
              <span class="text-caption">(81)96666-6666 </span> <br/>
              <v-btn
                icon="fas fa-envelope"
                color=""
                class="mt-10"
                variant="outlined"
              ></v-btn
              ><br/>
              <span class="text-caption">kiryukazuma@gmail.com </span> <br/>
              <span class="text-caption">dragonofdojima@gmail.com </span> <br/>
              <span class="text-caption">joryu@gmail.com </span> <br/>
            </div>
          </v-col>
          <v-col cols="12" sm="8">
            <h1 class="mt-8">Envie seu pedido</h1>
            <v-divider></v-divider>
            <span class="text-caption"
              >Descreva o motivo ao qual você precisa da minha ajuda</span
            >
            <v-row class="mt-10">
              <v-col cols="12" sm="6">
                <v-text-field
                  label="Nome"
                  persistent-hint
                  variant="outlined"
                ></v-text-field>
              </v-col>
              <v-col cols="12" sm="6">
                <v-text-field
                  label="Telefone"
                  persistent-hint
                  variant="outlined"
                ></v-text-field>
              </v-col>
            </v-row>
            <v-textarea
              label="Mensagem"
              persistent-hint
              variant="outlined"
            ></v-textarea>
            <v-btn color="#d50000" class="mt-2">Enviar</v-btn>
          </v-col>
        </v-row>
      </v-col>

    </v-container>
    <FooterView />
  </v-app>
</template>

<script>
import { defineComponent } from 'vue';

// Components
import NavBar from '../components/NavBar.vue';
import FooterView from "../components/FooterView.vue";

export default defineComponent({
  name: 'HomeView',
  setup() {
    return {
      slider2: 50,
      items: [
        {
          img: "y6.png",
        },
        {
          img: "y1k.png",
        },
        {
          img: "y2k.png",
        },
        {
          img: "y3.png",
        },
        {
          img: "y4.png",
        },
        {
          img: "y5.png",
        },
      ],
    };
  },

  components: {
    NavBar,
    FooterView
  },
});

</script>
<style scoped>
.v-container{
  padding: 16px 0;
}

.box{
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 540px;
  width: 100%;
  color: white;
  
}
.box:before {
  content: " ";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 50%;
  background: rgb(255,255,255);
  background: linear-gradient(0deg, rgba(255,255,255,1) 0%, rgba(213,0,0,1) 31%, rgba(0,0,0,1) 79%);        
}

.box:after {
  content: " ";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50%;
  background: rgb(255,255,255);
  background: linear-gradient(0deg, rgba(255,255,255,1) 0%, rgba(213,0,0,1) 31%, rgba(0,0,0,1) 79%);
}

.first {
  width: 100%;
  height: 280px;
  text-align: center;
  padding: 2rem 2rem;
}
.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  margin-right: 8px;
}
.imgHover {
  padding: 0 200px;
}
.pre {
  width: 100%;
  height: 380px;
  text-align: center;
  padding: 0 200px;
  background-color: #f5f5f5;
}
.hire {
  width: 100%;
  height: 200px;
  padding: 0 200px;
  background-color: #e9e9e9;
  margin-top: -24px;
}

</style>
