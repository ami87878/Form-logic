<template>
    <ul>
        <li><button type="button">Poor</button></li>
        <li><button type="button">Avrage</button></li>
        <li><button type="button">Great</button></li>
    </ul>
</template>

<script>

export default {
    name: 'FormLogicRatingControl',

    data() {
        return {
            
        };
    },

    mounted() {
        
    },

    methods: {
        
    },
};
</script>

<style lang="css" scoped>
    ul{

        list-style: none;
        margin: 0.5rem 0;
        padding: 0;
        display: flex;


    }

    li{

        padding: 1rem;
        display: flex;
        margin: 0 1rem;
        border: 1px solid  #ccc ;
        align-items: center;
        justify-content: center;

    }

    button{


        font: inherit;
        border: none;
        background-color: transparent;
        cursor: pointer;
        
    }
</style>