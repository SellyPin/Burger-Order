<template>
    <div id="nav">
        <router-link to="/" id="logo-url">
            <img :src="logo" :alt="alt" id="logo">
        </router-link>
     <router-link to="/">Home</router-link> 
     <router-link to="/pedidos">Pedidos</router-link>
    </div>
</template>

<script>
export default {
    name: "Navbar",
    props: ["logo", "alt"]
}

</script>

<style scoped>
    #nav {
        background-color: #222;
        border-bottom: 4px solid #111;
        padding: 15px 50px;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }
    /* medidas da barra em que ficam a logo e os textos */
    #nav #logo-url {
        margin: auto;
        margin-left: 0;
    }
    /* usou o nav para garantir que logo ficasse no lugar desejado */
    #logo {
        width: 40px;
        height: 40px;
    }
    /* medidas da logo */
    #nav a {
        color: #FCBA03;
        text-decoration: none;
        margin: 12px;
        transition: .5s;
    }
    /* medidas do texto na barra */
    #nav a:hover {
        color: #FFF;
    }
    /* cor da transição quando passa o mouse */
</style>>

