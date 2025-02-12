<template>          <!-- Componente que vai ser chamado no outro componente -->
    <div>
        <p v-if="estaTrabalhando">Atualmente trabalho na area de programação como {{ profissao }}</p>
        <p v-else>No momento estou em busca de novas oportunidades</p>
        <p>Meu email é: {{ email }} <br> {{ emailSecond }} <br> {{ malito }}</p>

        <ul>
            <li v-if="estaLogado"> <a href="#">meu perfil do github: </a></li>
            <li v-else> <a href="#">meu perfil do Linkedin: </a></li>
        </ul>
    </div>
</template>

<script>
export default{
    name: 'infoUser',
    data(){
        return{
            profissao: 'estagiaria' ,
            emailSecond: 'mariaclararezendevianna@outlook.com', /* dados que estão sendo passados na props */
                                  
        }
    },
    props:{                             /* propriedade para receber dados (props) */
        email: String,                  /* Tipando a variavel que vai ser chamada no componente */
        malito: String,                 /* Tipando a variavel que vai ser chamada no componente */
        estaTrabalhando: Boolean,        /* Tipando a variavel que vai ser chamada no componente */
        estaLogado: Boolean
    }
}
</script>

