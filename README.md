Hi, this is our first program or initial concept developed using Vue.js tools.

>link : Documentation on vue: 
https://vuejs.org/guide/quick-start.html#try-vue-online


## Instalation

link:: https://cli.vuejs.org/#getting-started

 Instalação do cliente Vue
```
~npm install -g @vue/cli
```

## Criação do projeto
```
vue create nome_do_diretorio
```
or 

Abrir interface de criação de projeto na página web
```
~vue ui 
```

...Ao fim da criação do projeto, você deve entrar no diretório criado e iniciar o servidor local.

```
cd nome_diretorio

npm run sreve 

ou 

yarn serve
```


## Utilitários
Site para icons
https://icones.js.org/


## Concept of SFC

SFC (Single-File Component) é um formato de arquivo do Vue que encapsula a lógica, estilização e marcação de um componente em um único arquivo. É uma funcionalidade que define o Vue como framework. 

Estrutura padrão

- Arquivo de component "Componente.vue"
```
<template> 
    <header>
        <div>
            <p>Conteúdo escrito!</p>
        </div>
    </header>
</template>

<script>
    export default{

    }
</script>

<style>
header{
    background-color: #000;
}
</style>

```

- Arquivo prinicipal "App.vue"

```
<template>
  <TheHeader/>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import Componente from './components/Componente.vue'

export default {
  name: 'App',
  components: {
    Componente    
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
```


## Diretivas
As diretivas são instruções dadas ao elemento html para resolução de problema.

Ex: v-show="", v-if="", v-else=if="", v-else=""
```
<template>
  <TheHeader
    v-show="showHeader"
  />
</template>

<script>
  export default {
    name: 'App'
    components: {
      TheHeader
    }
  },
  data() {
    return{
      showHeader: false
    }
  }
</script>
```



## Uso do FOR (Introdução a Loops(diretiva v-for))

//menção de fake API para consultar dados e testar o TODO. 
Link: https://jsonplaceholder.typicode.com/
Ex: Nesse exemplo é usado uma diretiva v-for para fazer um loop.
<template>
  <div v-for="obj in todos" 
    v-bind:key="obj.id"
  >

    {{ obj.title}}

</div>
</template>


## v-bind - da uma instrução para que o atributo seja dinâmico
Ex Não dinâmico: 
```
<img
  src="http://..." 
  alt="Idetificação da imagem"
>
<img
  v-bind:src="variavel-declarada-no-script-com-o-url-da-imagem" 
  v-bind:alt="variavel-declarada-no-script"
>

<script>
  export default {
    name: 'App',
    data() {
      return {
        variavel-declarada-no-script-com-o-url-do-src: 'html://..',
        variavel-declarada-no-script-com-a-definicao-do-alt: 'Eu sou o alt da imagem',
      }
    }
  }
</script>

```

## Data Biding (v-bind)