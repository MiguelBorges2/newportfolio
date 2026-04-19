<script setup>
import Navbar from '@/component/Navbar.vue';
import { ref, onMounted, onUnmounted } from 'vue'
const larguraTela = ref(window.innerWidth)

function atualizalarg(){
    larguraTela.value = window.innerWidth
}

onMounted(() => {
    window.addEventListener('resize', atualizalarg)
})
onUnmounted(() => {
  window.removeEventListener('resize', atualizalarg)
})
</script>
   
<template>
    <div class="d-flex justify-conten=hao2t-center big w-100">
        <div v-if="larguraTela>1024"class="d-flex  sic2 flex-column justify-content-around">
             <img class="ornamento" src="../assets/dots.svg">
             <img class="ornamento" src="../assets/rectangle.svg">
        </div>
        <div class="d-flex size2  main flex-column justify-content-start align-items-center"> 
            <Navbar ></Navbar>
            <div v-if="larguraTela>1024" class="d-flex w-100 justify-content-center push align-items-center">
                
                <div class="d-flex   size align-items-start flex-column">
                <p class="text-light push4 hero">Miguel Borges de Rezende Costa</p>
                <p class=" color push4 hero">Desenvolvedor full-stack</p>
                <span class="sub3 push4">
                    Criando aplicações Web versáteis e aplicativos mobiles...
                </span>
                <button class="but push4 text-light">
                    Entre em Contato!
                </button>
             </div>
                <div class="d-flex   img justfy-content-center">
                    <img class="log " src="../assets/Logo.svg">
                    <img class="pic " src="../assets/pic2.png">
                    <img class="log4 " src="../assets/dots.svg">
                </div>
            </div>
            <div v-if="larguraTela<=1024" class="d-flex w-100 flex-column justify-content-center tamp  align-items-center">
               <div class="ornamento10  teto2 d-flex justify-content-center">
                    <svg viewBox="0 0 600 80" fill="none" xmlns="http://www.w3.org/2000/svg" class="ornamento-svg ">
  <g stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">

    <!-- Linhas laterais -->
    <path d="M40 40 H240" opacity="0.6"/>
    <path d="M360 40 H560" opacity="0.6"/>

    <!-- Pontos sutis -->
    <circle cx="240" cy="40" r="2.5" fill="currentColor" stroke="none" opacity="0.6"/>
    <circle cx="360" cy="40" r="2.5" fill="currentColor" stroke="none" opacity="0.6"/>

    <!-- Código central -->
    <path d="M280 26 L260 40 L280 54" />
    <path d="M320 26 L340 40 L320 54" />
    <path d="M305 24 L295 56" />

  </g>
</svg>
                </div> 
                
                <div class="d-flex size teto floor align-items-center flex-column">
                    <p v-if="larguraTela>=500"class="text-light chao4 hero">Miguel Borges</p>
                    <p v-if="larguraTela<500"class="text-light  chao4 hero">Miguel Borges</p>
                    <p  class=" color push12 push4 chao4 hero2">Desenvolvedor full-stack</p>
                    <span class="sub3 push4">
                        Criando aplicações Web versáteis e aplicativos mobiles...
                    </span>
                
                </div>
    <div class="ornamento10 chao d-flex justify-content-center">
                    <svg  viewBox="0 0 600 80" fill="none" xmlns="http://www.w3.org/2000/svg" class="ornamento-svg">
  <g stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">

    <!-- Linhas laterais -->
    <path d="M40 40 H240" opacity="0.6"/>
    <path d="M360 40 H560" opacity="0.6"/>

    <!-- Pontos sutis -->
    <circle cx="240" cy="40" r="2.5" fill="currentColor" stroke="none" opacity="0.6"/>
    <circle cx="360" cy="40" r="2.5" fill="currentColor" stroke="none" opacity="0.6"/>

    <!-- Código central -->
    <path d="M280 26 L260 40 L280 54" />
    <path d="M320 26 L340 40 L320 54" />
    <path d="M305 24 L295 56" />

  </g>
</svg>
                </div> 
                <div  class=" metade d-flex flex-column justify-content-center align-items-center">
                    
                    <div class="quote-box">
                        <p class="text-light no">A tecnologia por si só não muda o mundo. São as pessoas que a constroem, com propósito, que fazem isso.</p>
                    </div>
                    <div class="quote-box2">
                        <p class="text-light no">-Satya Nadella</p>
                    </div>
             </div>
         
            </div>
             <div v-if="larguraTela>1024"  class="w-100 d-flex push2  justify-content-end">
                    <span class="trab d-flex bg-dark justify-content-between">
                        <div class="square"></div>
                        <p class="text-light tips">Procurando emprego!</p>
                    </span>
              </div>
            <div v-if="larguraTela>1024" class="metade d-flex flex-column justify-content-center align-items-center">
                <div class="quote-box">
                    <p class="text-light no">A tecnologia por si só não muda o mundo. São as pessoas que a constroem, com propósito, que fazem isso.</p>
                </div>
                <div class="quote-box2">
                    <p class="text-light no">-Satya Nadella</p>
                </div>
            </div>
            <div class="w-100 push3 d-flex flex-column">
                <div class="w-100 d-flex align-items-center justify-content-start">
                    <p class="text-light no2"><span class="hash">#</span>projetos</p>
                    <div class="linha"></div>   
                </div>
                <div v-if="larguraTela > 1024" class="w-100 d-flex push2 justify-content-around align-items-center"> 
                    <a class="prog" href="https://reformacasa.facom.ufu.br/">
                        <div class="projeto d-flex flex-column ">
                        <img class="projpic" src="../assets/ct.png">
                        <div class="stack d-flex justify-content-center">
                            <p class="sub no3">HTML CSS Vue.js Node.js</p>
                        </div>
                         <div class="stack2 d-flex justify-content-center flex-column align-items-center">
                            <p class="text-light no3 sic ">Reforma Na palma da mão</p>
                            <p class=" sub2">Plataforma Web informativa sobre reformas. Desenvolvido em parceria com a FAU da UFU</p>
                            <div class="chama d-flex text-light justify-content-center">Ativo</div>
                        </div>  
                    </div>
                    </a>
                    <a class="prog" href="https://casadaeternapaz.onrender.com/">
                         <div class="projeto d-flex flex-column ">
                        <img class="projpic" src="../assets/casa.png">
                        <div class="stack d-flex justify-content-center">
                            <p class="sub no3">HTML CSS Vue.js Node.js</p>
                        </div>
                         <div class="stack2 d-flex justify-content-center flex-column align-items-center">
                            <p class="text-light no3 sic ">Site Imersivo (RPG de Mesa)</p>
                            <p class="sub2 ">Aplicação web imersiva, simulando recrutamento para um culto fictício.</p>
                            <div class="chama d-flex text-light justify-content-center">Ativo</div>
                        </div>  
                    </div>
                    </a>
                </div>
                  <div v-if="larguraTela <= 1024" class="w-100 d-flex push2  flex-column justify-content-around align-items-center"> 
                    <a class="prog" href="https://reformacasa.facom.ufu.br/">
                        <div class="projeto d-flex flex-column ">
                        <img class="projpic" src="../assets/ct.png">
                        <div class="stack d-flex justify-content-center">
                            <p class="sub no3">HTML CSS Vue.js Node.js</p>
                        </div>
                         <div class="stack2 d-flex justify-content-center flex-column align-items-center">
                            <p class="text-light no3 sic ">Reforma Na palma da mão</p>
                            <p class=" sub2">Plataforma Web informativa sobre reformas. Desenvolvido em parceria com a FAU da UFU</p>
                            <div class="chama d-flex text-light justify-content-center">Ativo</div>
                        </div>  
                    </div>
                    </a>
                    <a class="prog" href="https://casadaeternapaz.onrender.com/">
                         <div class="projeto d-flex flex-column ">
                        <img class="projpic" src="../assets/casa.png">
                        <div class="stack d-flex justify-content-center">
                            <p class="sub no3">HTML CSS Vue.js Node.js</p>
                        </div>
                         <div class="stack2 d-flex justify-content-center flex-column align-items-center">
                            <p class="text-light no3 sic ">Site Imersivo (RPG de Mesa)</p>
                            <p class="sub2 ">Aplicação web imersiva, simulando recrutamento para um culto fictício.</p>
                            <div class="chama d-flex text-light justify-content-center">Ativo</div>
                        </div>  
                    </div>
                    </a>
                </div>
                 <div  class="w-100 d-flex push2 align-items-center justify-content-start">
                    <p class="text-light no2"><span class="hash">#</span>skills</p>
                    <div class="linha"></div>   
                </div>
                <div v-if="larguraTela > 1024"  class="w-100 d-flex justify-content-around ">
                    <img class="detail" src="../assets/group36.svg">
                    <div class="w-50 d-flex align-items-around justify-content-between flex-wrap">
                        <div class="skill ">
                            <span class="text-light w-100 bott d-flex justify-content-center">
                                Linguagens
                            </span>
                            <div class="d-flex flex-column align-items-start">
                                <p class="color2">-JavaScript</p>
                                <p class="color2">-Java</p>
                                <p class="color2">-Python</p>
                                <p class="color2">-C</p>
                                <p class="color2">-C++</p>
                                <p class="color2">-TypeScript</p>
                            </div>
                        </div>
                        <div class="skill ">
                            <span class="text-light w-100 bott d-flex justify-content-center">
                                Database
                            </span>
                            <div class="d-flex flex-column align-items-start justify-content-center">
                                <p class="color2">-MySQL</p>
                                <p class="color2">-PostgreSQL</p>
                                <p class="color2">-Mongo</p>
                                <p class="color2">-SQLite</p>
                            </div>
                        </div>
                        <div class="skill ">
                            <span class="text-light w-100 bott d-flex justify-content-center">
                                Outros
                            </span>
                            <div class="d-flex flex-column align-items-start">
                                <p class="color2">-Node.js</p>
                                <p class="color2">-HTML</p>
                                <p class="color2">-CSS</p>
                                <p class="color2">-BootStrap</p>
                                <p class="color2">-Tailwind</p>
                            </div>
                        </div>
                         <div class="skill ">
                            <span class="text-light w-100 bott  d-flex justify-content-center">
                                Frameworks
                            </span>
                            <div class="d-flex flex-column align-items-start">
                                <p class="color2">-Vue.js</p>
                                <p class="color2">-Express</p>
                                <p class="color2">-SpringBoot</p>
                                <p class="color2">-REACT</p>
                                <p class="color2">-C++</p>
                                <p class="color2">-TypeScript</p>
                            </div>
                        </div>
                        
                    </div>
                </div>
                 <div v-if="larguraTela <= 1024"  class="w-100 d-flex justify-content-around flex-column rela">
                    <div class="w-100 d-flex push31 align-items-around justify-content-around flex-wrap">
                        <div class="skill ">
                            <span class="text-light w-100 bott d-flex justify-content-center">
                                Linguagens
                            </span>
                            <div class="d-flex flex-column align-items-start">
                                <p class="color2">-JavaScript</p>
                                <p class="color2">-Java</p>
                                <p class="color2">-Python</p>
                                <p class="color2">-C</p>
                                <p class="color2">-C++</p>
                                <p class="color2">-TypeScript</p>
                            </div>
                        </div>
                        <div class="skill ">
                            <span class="text-light w-100 bott d-flex justify-content-center">
                                Database
                            </span>
                            <div class="d-flex flex-column align-items-start justify-content-center">
                                <p class="color2">-MySQL</p>
                                <p class="color2">-PostgreSQL</p>
                                <p class="color2">-Mongo</p>
                                <p class="color2">-SQLite</p>
                            </div>
                        </div>
                        
                        
                    </div>
                    <div class="w-100 d-flex push31 align-items-around justify-content-around flex-wrap">
                        
                        <div class="skill ">
                            <span class="text-light w-100 bott d-flex justify-content-center">
                                Outros
                            </span>
                            <div class="d-flex flex-column align-items-start">
                                <p class="color2">-Node.js</p>
                                <p class="color2">-HTML</p>
                                <p class="color2">-CSS</p>
                                <p class="color2">-BootStrap</p>
                                <p class="color2">-Tailwind</p>
                            </div>
                        </div>
                         <div class="skill ">
                            <span class="text-light w-100 bott  d-flex justify-content-center">
                                Frameworks
                            </span>
                            <div class="d-flex flex-column align-items-start">
                                <p class="color2">-Vue.js</p>
                                <p class="color2">-Express</p>
                                <p class="color2">-SpringBoot</p>
                                <p class="color2">-REACT</p>
                                <p class="color2">-C++</p>
                                <p class="color2">-TypeScript</p>
                            </div>
                        </div>
                        
                    </div>
                </div>
                <div class="w-100 d-flex push2 align-items-center justify-content-start">
                    <p class="text-light no2"><span class="hash">#</span>Sobre mim</p>
                    <div class="linha"></div>   
                </div>
                <div v-if="larguraTela > 1024" class="w-100 d-flex">
                    <div class="meia push30">
                        <p class="color2">Ola, eu sou o Miguel!</p>
                        <p class="color2">Sou desenvolvedor full-stack formado em Ciência da Computação pela UFU, com experiência prática no desenvolvimento de aplicações web e APIs RESTful.</p>
                        <p class="color2">Atuei como estagiário na Algar Telecom e como desenvolvedor full-stack júnior na Telek Sistemas, trabalhando com sistemas reais, integrações e comunicação entre serviços.</p>
                        <p class="color2 push3">Trabalho principalmente com Vue.js no frontend e Node.js no backend, desenvolvendo soluções completas, modernas e focadas em performance e usabilidade.</p>
                        <p class="color2 push3">Tenho experiência em projetos reais, incluindo uma plataforma desenvolvida em parceria com a UFU, além de aplicações web interativas.</p>
                        <p class="color2 push3">Busco sempre entregar soluções bem estruturadas, eficientes e fáceis de manter.</p>
                    </div>
                    <div class="meia bisnaga">
                        <img class="pic2 " src="../assets/tuts2.png">
                        <img class="log2 " src="../assets/dots.svg">
                        <img class="log3 " src="../assets/frame.svg">
                    </div>
                </div>
                <div v-if="larguraTela <= 1024" class="w-100 d-flex flex-column">
                    <div class="w-100  chao3 push30">
                        <p class="color2">Ola, eu sou o Miguel!</p>
                        <p class="color2">Sou desenvolvedor full-stack formado em Ciência da Computação pela UFU, com experiência prática no desenvolvimento de aplicações web e APIs RESTful.</p>
                        <p class="color2">Atuei como estagiário na Algar Telecom e como desenvolvedor full-stack júnior na Telek Sistemas, trabalhando com sistemas reais, integrações e comunicação entre serviços.</p>
                        <p class="color2 push3">Trabalho principalmente com Vue.js no frontend e Node.js no backend, desenvolvendo soluções completas, modernas e focadas em performance e usabilidade.</p>
                        <p class="color2 push3">Tenho experiência em projetos reais, incluindo uma plataforma desenvolvida em parceria com a UFU, além de aplicações web interativas.</p>
                        <p class="color2 push3">Busco sempre entregar soluções bem estruturadas, eficientes e fáceis de manter.</p>
                    </div>
                    <div class="w-100 bisnaga">
                        <img class="pic2 " src="../assets/tuts2.png">
                        <img class="log2 " src="../assets/dots.svg">
                        <img class="log3 " src="../assets/frame.svg">
                    </div>
                </div>
                <div class="w-100 d-flex push2 align-items-center justify-content-start">
                    <p class="text-light no2"><span class="hash">#</span>contato</p>
                    <div class="linha"></div>   
                </div>
                <div v-if="larguraTela>1024" class="w-100 d-flex justify-content-between">
                    <p class="color2 push3  self meia">Não exite em entrar em contato pelas redes sociais listadas ou dar uma olhada no meu GitHub!  </p>
                    <div class="size7 boxe push10 d-flex flex-column  align-items-center">
                        <div class="w-100  align-items-center d-flex">
                            <img class="icone" src="../assets/email.svg">
                            <p class="text-light m-0">miguel.costa@ufu.br</p>
                        </div>
                        <div class="w-100   align-items-center d-flex">
                            <img class="icone" src="../assets/zapzap.svg">
                            <p class="text-light m-0">(34) 98442-3034</p> 
                        </div>
                        <div class="w-100  align-items-center d-flex">
                            <img class="icone" src="../assets/git.svg">
                            <p class="text-light m-0">(34) 98442-3034</p>
                        </div>
                    </div>
                </div>
                <div v-if="larguraTela <= 1024" class="w-100 d-flex justify-content-center flex-column align-items-center">
                    <p class="color2 push3  self w-100">Não exite em entrar em contato pelas redes sociais listadas ou dar uma olhada no meu GitHub!  </p>
                    <div class="size7 boxe push10 d-flex flex-column  align-items-center">
                        <div class="w-100  align-items-center d-flex">
                            <img class="icone" src="../assets/email.svg">
                            <p class="text-light sic3 m-0">miguel.costa@ufu.br</p>
                        </div>
                        <div class="w-100   align-items-center d-flex">
                            <img class="icone" src="../assets/zapzap.svg">
                            <p class="text-light sic3  m-0">(34) 98442-3034</p> 
                        </div>
                        <div class="w-100  align-items-center d-flex">
                            <img class="icone" src="../assets/git.svg">
                            <p class="text-light sic3 m-0">(34) 98442-3034</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div  v-if="larguraTela > 1024" class="d-flex sic2 flex-column justify-content-around">
            <img class="ornamento" src="../assets/rectangle.svg">
             <img class="ornamento2" src="../assets/dots.svg">
             <img class="ornamento" src="../assets/dots.svg">
        </div>  
    </div>
  
</template>
<style>
.size7 {
    width: 20%;
}
.push11 {
    margin-top: 5%;;
}
.push12 {
    margin-top: 0;
}
.self {
    align-self: center;
}
.boxe {
    border: 2px solid rgba(171, 178, 191, 1);
}
.icone {
    width: 15%;
    margin-bottom: 0;
    margin-top: 0;
}
.bisnaga {
    position: relative;
    width: 100%
}
.meia {
    width: 50%;
}
.push4 {
    margin-left: 5%;
}
.style {
    list-style: none;
}
.push10 {
    margin: 2%;
}
.color2 {
    color: rgba(171, 178, 191, 1);
    margin:0;
    text-align: justify;
}
.bott {
    border-bottom: 2px solid rgba(171, 178, 191, 1);
}
.skill {
    width: 30%;
    border: 2px solid rgba(171, 178, 191, 1);
    margin-bottom: 2%;
         transition: all 0.3s ease;
}
.skill:hover {
    transform: scale(1.1);
    box-shadow: 
  0 1px 2px rgba(199, 120, 221, 1),
  0 4px 10px rgba(199, 120, 221, 1);
}
.detail {
    width: 22%;
}
.chama {
    width: 40%;
    background-color:  rgba(199, 120, 221, 1);
    border-radius: 60px;
    box-shadow: 0 0 10px rgba(199, 120, 221, 1);
    margin: 1%;
    padding: 1%;
}

.sic {
    font-size: 1.2vw;
}
.push5 {
    margin-left: 2%;
}
.stack {
    width: 100%;
    border-top: 2px solid rgba(171, 178, 191, 1);
    border-bottom: 2px solid rgba(171, 178, 191, 1);
    
}
.stack2 {
    width: 100%;
    
}
.prog {
     width: 25%;
     text-decoration: none;
}
.projeto {
    width: 100%;
    border: 2px solid rgba(171, 178, 191, 1);
     transition: all 0.3s ease;
    
}
.projeto:hover {
    transform: scale(1.1);
    box-shadow: 
  0 1px 2px rgba(199, 120, 221, 1),
  0 4px 10px rgba(199, 120, 221, 1);
}
.projpic {
    width: 100%;
    height: 10vw;
    margin: 0 !important;
    padding: 0;
}
.linha {
    padding: 0.1%;
    background-color: rgba(199, 120, 221, 1);
    border-radius: 60px;
    width: 30%;
}
.no {
    margin: 0;
}
.no2 {
    padding: 0;
    margin-right: 1%;
    margin-bottom: 0;
    font-size: 1.3vw;
}
.no3 {
    padding: 0;
    margin: 3%;
    
}
.quote-box {
  margin-top: 8%;
  position: relative;
  border: 1px solid rgba(171, 178, 191, 1);
  padding: 2%;
  font-size: 1vw;
  border-radius: 2px;
  color: #fff;
  text-align: center;
}
.quote-box2 {
  align-self: end;
  border: 1px solid rgba(171, 178, 191, 1);
  padding: 1%;
  font-size: 1vw;
  border-radius: 2px;
  color: #fff;
}
.quote-box::before {
  content: "“";
  position: absolute;
  top: -18px;
  left: 20px;

  font-size: 40px;
  color: #c9a44c;

 /* mesma cor do fundo */
  
}
.metade {
    width:50%;
}
.quote-box::after {
  content: "“";
  position: absolute;
  bottom: -40px;
  right: 20px;

  font-size: 40px;
  color: #c9a44c;

 /* mesma cor do fundo */
  padding: 0 8px;
}
.chao4 {
    margin-bottom: 3%;
}
.chao {
    margin-bottom: 7%;
}
.chups {
    margin-bottom: 45%;
}
.tips {
    margin: 0;
}
 .push2 {
    margin-top: 2%;
 }
 .push3 {
    margin-top: 2%;
 }
 .push30 {
    margin-top: 3%;
 }
 .push31 {
    margin-top: 3%;
 }
    .trab {
        width: 20%;
        margin-right: 14%;
        padding: 0.5%;
        border: 1px solid rgba(171, 178, 191, 1)
    }
    .square {
        background-color: rgba(199, 120, 221, 1);
        width: 10%;
         padding: 0%;

    }
    .img {
        position: relative;
        width: 50%;

    }
    .big {
        height: 100%;
        padding:0;
        margin: 0 !important;
        padding: 0;
    }
    .main {
        background-color: rgba(40, 44, 51, 1);
        
       
    }
    .but {
        background-color: rgba(40, 44, 51, 1);
        border: 1px solid rgba(199, 120, 221, 1);
        margin-top: 5%;
        padding: 1.5%;
        width: 30%;
    }
    .sub {
        color: rgba(171, 178, 191, 1);
        font-size:1.4vw;
    }
    .sub3 {
        color: rgba(171, 178, 191, 1);
        font-size:1.4vw;
    }
    .sic2 {
        width: 7.5%;
    }
    .sub2 {
        color: rgba(171, 178, 191, 1);
        font-size: 1vw;
        margin-top: 0;
        margin-bottom: 2%;
        text-align:start;
        margin-left: 1%;
        margin-right: 1%;
        
    }
    .hero {
        font-size: 2vw;
    }
    .hero2 {
        font-size: 2vw;
    }
    .push {
        margin-top: 15%;
    }
    .sic2{
        width: 7.5%;
        margin: 0 !important;
        padding:0;
    }
    .ornamento10 {
        width: 100%;
        color: rgba(199, 120, 221, 1);
    }
    .teto {
        margin-top: 5%;
    }
    .floor {
        margin-bottom: 5%;
    }
    .ornamento-svg {
  width: 55%;
  display: flex;
  height: auto;
  display: block;
}
    .ornamento {
        width: 50%;
        margin: 0;
    }
    .ornamento2 {
        width: 65%;
        margin: 0;
    }
    .size2 {
        width: 85%;
        height: 100%;
        margin: 0 !important;
    }
    .chao2 {
        margin-top: 23%;
    }
    .charps {
       
    }
    .color {
        color: rgba(199, 120, 221, 1);
    }
    .size {
        width: 50%;
    }
    .log {
        width: 27%;
        height:auto;
         position: absolute;
        margin: 0;
        top: 50%;
        left: 18%;
        transform: translate(-1%, -60%);
    }

    .pic {
        margin: 0;
        width: 30%;
        height: auto;
        position: absolute;
        z-index: 10;
        top: 50%;
        left: 40%;
        transform: translate(-10%, -65%);
     
    }
    .chao3 {
        margin-bottom: 70%;
    }
    .log2 {
        margin: 0;
        width: 12%;
        height:auto;
         position: absolute;
        top: 30%;
        left: 38%;
        z-index: 9;
        transform: translate(-50%, -50%);
    }
    
    .log3 {
        margin: 0;
        width: 15%;
        height:auto;
         position: absolute;
        top: 70%;
        z-index: 11;
        left: 70%;
        transform: translate(-50%, -50%);
    }
    .log4 {
        margin: 0;
        width: 15%;
        height:auto;
         position: absolute;
        top: 90%;
        z-index: 11;
        left: 72%;
        transform: translate(-50%, -10%);
    }
    .pic2 {
        margin: 0;
        width: 43%;
        height: auto;
        position: absolute;
        z-index: 10;
        top: 52%;
        left: 50%;
        transform: translate(-50%, -48%);
     
    }
    @media(max-width: 1024px){
        .sic3 {
            font-size: 2.2vw;
        }
        .skill {
    width: 32%;
    border: 2px solid rgba(171, 178, 191, 1);
    margin-bottom: 2%;
}
    .img{
        width:100%;
    }
        .icone {
          width: 10%;
        }
        .pic2 {
        margin: 0;
        width: 32%;
        height: auto;
        position: absolute;
        z-index: 10;
        top: 2%;
        left: 50%;
        transform: translate(-50%, -100%);
     
    }
    .log2 {
        margin: 0;
        width: 14%;
        height:auto;
         position: absolute;
        top: 2%;
        left: 38%;
        z-index: 9;
        transform: translate(-50%, -450%);
    }
    .push4 {
        margin-left: 1%;
    }
    .log3 {
        margin: 0;
        width: 17%;
        height:auto;
         position: absolute;
        top: 90%;
        z-index: 11;
        left: 70%;
        transform: translate(-80%, -200%);
    }
    .color2 {
        font-size: 2vw;
    }
    .bott {
        font-size: 2.6vw;
    }
        .linha {
    padding: 0.1%;
    background-color: rgba(199, 120, 221, 1);
    border-radius: 60px;
   
}
    .no2 {
        font-size: 2.2vw;
    }
        .projpic {
    width: 100%;
    height: 28vw;
    margin: 0 !important;
    padding: 0;
}
.detail {
    width: 60%;
    position: absolute;
    top: 50%;
    z-index: 1;
        left: 50%;
        transform: translate(-50%, -50%);
}
.sub2 {
        color: rgba(171, 178, 191, 1);
        font-size: 2vw;
        margin-top: 0;
        margin-bottom: 2%;
        text-align:start;
        margin-left: 1%;
        margin-right: 1%;
        
    }

.rela {
    position: relative;
}
.log {
        width: 20%;
        height:auto;
         position: absolute;
        margin: 0;
        top: 40%;
        left: 30%;
        transform: translate(-20%, -65%);
    }
        .size2{
            width: 100% !important;
        }
         .prog {
            width: 55%;
            margin-bottom: 4%;
         }
        
        .metade {
            width: 70%;
        }
        .pic {
        margin: 0;
        width: 30%;
        height: auto;
        position: absolute;
        z-index: 10;
        top: 100%;
        left: 50%;
        transform: translate(-50%, -60%);
     
    }
    .hero {
        font-size: 8.5vw;
    }
    .hero2 {
        font-size: 6vw;
    }
    .size {
        width: 100%;
    }
    .sub3 {
        font-size: 3vw;
        text-align:center;
        
    }
    .sub {
        font-size: 2.5vw;
    }
    .trab {
        margin-left: 14%;
        width: 35%;
    }
    .tips {
        font-size: 2vw;
        margin-right: 2%;
    }
    .size7 {
    width: 30%;
}
    .push30 {
        margin-bottom: 63%;
    }
.metade {
            width:80%;
        }
    .quote-box {
  margin-top: 2%;
  position: relative;
  border: 1px solid rgba(171, 178, 191, 1);
  padding: 1%;
  font-size: 2.7vw;
  border-radius: 2px;
  color: #fff;
  text-align: center;
}
.quote-box2 {
  align-self: end;
  border: 1px solid rgba(171, 178, 191, 1);
  padding: 1%;
  font-size: 2.6vw;
  border-radius: 2px;
  color: #fff;
}
 .log4 {
        margin: 0;

        height:auto;
         position: absolute;
        top: 98%;
        z-index: 12;
        left: 72%;
        width: 12%;
        transform: translate(-90%, 50%);
    }
    .tamp {
        height: 100dvh !important;
    }
  .sic {
    font-size: 2.5vw !important;
}
    }
   
    @media(max-width: 500px){
    .push30 {
        margin-bottom: 75%;
    }
     .pic2 {
        margin: 0;
        width: 42%;
        height: auto;
        position: absolute;
        z-index: 10;
        top: 2%;
        left: 50%;
        transform: translate(-50%, -100%);
     
    }
        .skill {
    width: 40%;
    border: 2px solid rgba(171, 178, 191, 1);
    margin-bottom: 2%;
}
         .prog {
            width: 65%;
            margin-bottom: 4%;
         }
        .tips {
        font-size: 3.5vw;
        margin-right: 2%;
    }
    .teto {
        margin-top: 10%;
    }
    .floor {
        margin-bottom: 10%;
    }
        .log {
        width: 25%;
        height:auto;
         position: absolute;
        margin: 0;
        top: 10%;
        left: 30%;
        transform: translate(-40%, -105%);
    }
        .log4 {
        margin: 0;

        height:auto;
         position: absolute;
        top: 5%;
        z-index:11;
        left: 72%;
        width: 18%;
        transform: translate(-40%, -10%);
    }
        .pic {
        margin: 0;
        width: 45%;
        height: auto;
        position: absolute;
        z-index: 10;
        top: 100%;
        left: 50%;
        transform: translate(-50%, -75%);
     
    }
        .chao {
            margin-bottom: 20%;
        }
        .chups {
            margin-bottom: 52%;
        }
        .hero {
            font-size: 9vw;
        }
         .hero2 {
        font-size: 6.5vw;
    }
    .sub {
        font-size: 3.5vw;
    }
    .sub3 {
        font-size: 4vw;
        margin-top:1%;
        margin-bottom: 2%;
    
    }
         .size7 {
    width: 35%;
}
.sic3 {
            font-size: 2.5vw;
        }
    .sic {
    font-size: 3.5vw !important;
}   
    .sub2 {
        color: rgba(171, 178, 191, 1);
        font-size: 3.3vw;
        margin-top: 0;
        margin-bottom: 2%;
        text-align:start;
        margin-left: 1%;
        margin-right: 1%;
        
    }
    .color2 {
        font-size: 3.5vw;
    }
    .bott {
        font-size: 3.2vw;
    }
    .linha {
        padding: 0.1%;
        background-color: rgba(199, 120, 221, 1);
        border-radius: 60px;
    
    }
      .tamp {
        height: 85vh !important;
    }
    .no2 {
        font-size: 3vw;
    }
      .trab {
         margin-left: 15%;
         width: 55%;
        }  
        .size2{
            width: 100% !important;
        }
        .metade {
            width: 95%;
        }
        .quote-box2 {
  align-self: end;
  border: 1px solid rgba(171, 178, 191, 1);
  padding: 1%;
  font-size: 3.4vw;
  border-radius: 2px;
  color: #fff;
}
        .quote-box {

  position: relative;
  border: 1px solid rgba(171, 178, 191, 1);
  padding-top: 1%;
  font-size: 3.6vw;
  border-radius: 2px;
  color: #fff;
  text-align: center;
}
.chao2 {
      margin-top: 23%; 
    
    }
.ornamento-svg {
    width: 80%;
}
    }
@media(max-height: 600px){
    .teto2 {
        margin-top: 10vh !important;
    }
    .tamp {
        height: 100% !important;
    }
     .teto {
        margin-top: 10vh;
    }
    .floor {
        margin-bottom: 10vh;
    }
    .ornamento-svg {
        width: 70vh;
    }
        
    .tips {
        font-size: 3.5vw;
        margin-right: 2%;
    }
        .log {
        width: 23%;
        height:auto;
         position: absolute;
        margin: 0;
        top: 10%;
        left: 33%;
        transform: translate(-40%, -105%);
    }
        .log4 {
        margin: 0;

        height:auto;
         position: absolute;
        top: 5%;
        z-index:11;
        left: 68%;
        width: 17%;
        transform: translate(-40%, -10%);
    }
        .pic {
        margin: 0;
        width: 39%;
        height: auto;
        position: absolute;
        z-index: 10;
        top: 100%;
        left: 50%;
        transform: translate(-50%, -75%);
     
    }
        .chao {
            margin-bottom: 1vh;
        }
        .chups {
            margin-bottom: 30%;
        }
        .hero {
            font-size: 6vh;
        }
         .hero2 {
        font-size: 3.5vh;
    }
    .sub3 {
        font-size: 2.3vh;
        margin-top:0;
        margin-bottom: 2%;
        
    }
         .size7 {
    width: 35%;
}
.sic3 {
            font-size: 2.5vw;
        }
    .sic {
    font-size: 4vw !important;
}   
    .sub2 {
        color: rgba(171, 178, 191, 1);
        font-size: 3.3vw;
        margin-top: 0;
        margin-bottom: 2%;
        text-align:start;
        margin-left: 1%;
        margin-right: 1%;
        
    }
    .color2 {
        font-size: 2.8vw;
    }
    .bott {
        font-size: 3.2vw;
    }
    .linha {
        padding: 0.1%;
        background-color: rgba(199, 120, 221, 1);
        border-radius: 60px;
    
    }
    .no2 {
        font-size: 3vw;
    }
      .trab {
         margin-right: 0;
         width: 55%;
        }  
        .size2{
            width: 100% !important;
        }
        .metade {
            width: 95%;
        }
        .quote-box2 {
  align-self: end;
  border: 1px solid rgba(171, 178, 191, 1);
  padding: 1%;
  font-size: 2vh;
  border-radius: 2px;
  color: #fff;
}
        .quote-box {

  position: relative;
  border: 1px solid rgba(171, 178, 191, 1);
  padding-top: 2%;
  font-size: 2vh;
  border-radius: 2px;
  color: #fff;
  text-align: center;
}
.chao2 {
      margin-top: 22%; 

    }
}

@media(max-height: 480px){
    .teto2 {
        margin-top: 0;
    }
    .tamp {
        height: 92vh !important;
    }
    .tips {
        font-size: 3.5vw;
        margin-right: 2%;
    }
        .log {
        width: 23%;
        height:auto;
         position: absolute;
        margin: 0;
        top: 10%;
        left: 33%;
        transform: translate(-40%, -105%);
    }
        .log4 {
        margin: 0;

        height:auto;
         position: absolute;
        top: 5%;
        z-index:11;
        left: 68%;
        width: 17%;
        transform: translate(-40%, -10%);
    }
        .pic {
        margin: 0;
        width: 32%;
        height: auto;
        position: absolute;
        z-index: 10;
        top: 100%;
        left: 50%;
        transform: translate(-50%, -75%);
     
    }
        .chao {
            margin-bottom: 2%;
        }
        .chups {
            margin-bottom: 30%;
        }
        .hero {
            font-size: 7vw;
        }
         .hero2 {
        font-size: 6.5vw;
    }
    .sub3 {
        font-size: 4.2vw;
        margin-top:0;
        margin-bottom: 2%;
        
    }
         .size7 {
    width: 35%;
}
.sic3 {
            font-size: 2.5vw;
        }
    .sic {
    font-size: 4vw !important;
}   
    .sub2 {
        color: rgba(171, 178, 191, 1);
        font-size: 3.3vw;
        margin-top: 0;
        margin-bottom: 2%;
        text-align:start;
        margin-left: 1%;
        margin-right: 1%;
        
    }
    .color2 {
        font-size: 2.8vw;
    }
    .bott {
        font-size: 3.2vw;
    }
    .linha {
        padding: 0.1%;
        background-color: rgba(199, 120, 221, 1);
        border-radius: 60px;
    
    }
    .no2 {
        font-size: 3vw;
    }
      .trab {
         margin-left: 3%;
         width: 55%;
        }  
        .size2{
            width: 100% !important;
        }
        .metade {
            width: 95%;
        }
        .quote-box2 {
  align-self: end;
  border: 1px solid rgba(171, 178, 191, 1);
  padding: 1%;
  font-size: 3vw;
  border-radius: 2px;
  color: #fff;
}
        .quote-box {

  position: relative;
  border: 1px solid rgba(171, 178, 191, 1);
  padding-top: 2%;
  font-size: 3.3vw;
  border-radius: 2px;
  color: #fff;
  text-align: center;
}
.chao2 {
      margin-top:17%; 
      
    }
}

</style>