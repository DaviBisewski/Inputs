<script setup>
import { ref } from 'vue'
const nome = ref('');
const email = ref('');
const senha = ref('');
const confirmasenha = ref('');
const idade = ref('');
const endereco = ref('');
const cidade = ref('');


</script>

<template>
  <div id="forms">
    <input type="text" v-model="nome" placeholder="Nome:" />
    <input type="email" v-model="email" placeholder="Email:" />
    <input type="password" v-model="senha" placeholder="Senha:" />
    <input type="password" v-model="confirmasenha" placeholder="Confirmar senha:" />
    <input type="date" v-model="idade" placeholder="Data de nascimento:" />
    <input type="text" v-model="endereco" placeholder="Endereço:" />
    <input type="text" v-model="cidade" placeholder="Cidade:" />
    <select v-model="estado">
      <option value="AC">ACRE</option>
      <option value="AL">ALAGOAS</option>
      <option value="AP">AMAPÁ</option>
      <option value="AM">AMAZONAS</option>
      <option value="BA">BAHIA</option>
      <option value="CE">CEARÁ</option>
      <option value="DF">DISTRITO FEDERAL</option>
      <option value="ES">ESPÍRITO SANTO</option>
      <option value="GO">GOIÁS</option>
      <option value="MA">MARANHÃO</option>
      <option value="MT">MATO GROSSO</option>
      <option value="MS">MATO GROSSO DO SUL</option>
      <option value="MG">MINAS GERAIS</option>
      <option value="PA">PÁRA</option>
      <option value="PB">PARAÍBA</option>
      <option value="PR">PARANÁ</option>
      <option value="PB">PERNAMBUCO</option>
      <option value="PI">PIAUÍ</option>
      <option value="RJ">RIO DE JANEIRO</option>
      <option value="RN">RIO GRANDE DO NORTE</option>
      <option value="RS">RIO GRANDE DO SUS</option>
      <option value="RO">RONDÔNIA</option>
      <option value="RR">RORAIMA</option>
      <option value="SC">SANTA CATARINA</option>
      <option value="SP">SÃO PAULO</option>
      <option value="SE">SERGIPE</option>
      <option value="TO">TOCANTINS</option>
    </select>
    <p>Linguagem de Programação</p>

    <div class="checkbox">
      <input type="checkbox" v-model="cmaismais" id="" />
      <p>C++</p>
    </div>
    <div class="checkbox">
      <input type="checkbox" v-model="python" id="" />
      <p>Python</p>
    </div>
    <div class="checkbox">
      <input type="checkbox" v-model="javascript" id="" />
      <p>JavaScript</p>
    </div>
    <div class="checkbox">
      <input type="checkbox" v-model="java" id="" />
      <p>Java</p>
    </div>

    <p>Hobbies favoritos</p>

    <div class="checkbox">
      <input type="checkbox" v-model="musica" id="" />
      <p>Musica</p>
    </div>
    <div class="checkbox">
      <input type="checkbox" v-model="esportes" id="" />
      <p>Esportes</p>
    </div>
    <div class="checkbox">
      <input type="checkbox" v-model="viagem" id="" />
      <p>Viagem</p>
    </div>
    <div class="checkbox">
      <input type="checkbox" v-model="cozinhar" id="" />
      <p>Cozinhar</p>
    </div>

    <input type="text" v-model="biografia" id="" placeholder="Biografia:" />
  </div>
  <button v-if>

  </button>
  <div id="submit" v-model="submit">
    {{ nome }}
    {{ endereco }}
    {{ confirmasenha }}
    {{ idade }}
    {{ endereco }}
    {{ cidade }}
  </div>
</template>

<style scoped>
*{
  margin: 0;
  padding: 0;
  border: 0;
  box-sizing: border-box;
  user-select: none;
}
#forms {
  display: flex;
  flex-direction: column;
}

.checkbox {
  display: flex;
}

#submit{
  display: flex;
  flex-direction: column;
}
</style>
