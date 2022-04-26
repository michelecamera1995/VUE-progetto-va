<template>
    <li><a href="">{{items.name}}</a></li>
</template>

<script>
export default {
    name: 'Listcomponent',

    props:{
        items: Object
    },

}
</script>

<style lang="scss" scoped>

    li{
        margin: 2%;
        display: flex;
        align-items: center;
        margin: 0px 15px;

        a{
            text-decoration: none;
        }
    
        a:hover {
        text-decoration: none;
        color: white;
        height: 25px;
        border-bottom: 1px solid white;
        }

        a:visited {
        text-decoration: none;
        color: white;
        }
    }

</style>