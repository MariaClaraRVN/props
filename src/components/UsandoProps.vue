<template>
    <div>
        <h1>Meu nome é {{ nome }}</h1>
        <InfoUser email="mariaclararezendeviannaa@gmail.com" :malito="emaill" :estaTrabalhando=true :estaLogado="true" />      
        <!-- Chamando a props de email dentro do componente de infoUser --> 
        <!-- Usando o binding com a props, atraves da variavel malito -->                               
    </div>
</template>

<script>
import InfoUser from './Info.User.vue';
    export default{
        name: 'UsandoProps',
        components:{
            InfoUser
        },
        data(){
            return{
                nome: 'Maria Clara',
                emaill: 'gameseplays1617@gmail.com'     /* dados que estão sendo passados na props */
            }
        }
    }
</script>

<style scoped> 
</style>