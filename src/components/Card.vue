

<template>
    <Grid>
        <img :src="url" :alt="nombre">
        <h2>{{nombre}}</h2>
        <a :href="url"
        target="_blank"
        >Descargar</a>
    </Grid>
</template>
<script>
import Grid from './Grid.vue';

export default {
    props: {
        url: {
            String
        },
        nombre: {
            String
        }
    },
    components: { Grid }
}
</script>
<style scoped>
img{
    width: 8rem;
    height: 8rem;
    padding: 0.5rem;
    background: red;
}
a{
    text-decoration: none;
    color: snow;
    background: #301665;
    padding: 0.3rem;
    border-radius: 5px;
    border: 1px solid #f2f2f2;
}
</style>