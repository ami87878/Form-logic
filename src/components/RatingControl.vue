<template>

    <ul>
        <li :class="{ active:activeable==='poor'}">

            <button    @click="actived('poor')"  type="button">Poor</button>
        </li>

        <li :class="{active:activeable==='avrage'}">

            <button  @click='actived("avrage")' type="button">Avrage</button>
        </li>

        <li :class="{ active:activeable==='great'}">

        <button    @click='actived("great")' type="button">Great</button>
    </li>
    </ul>

</template>

<script>

export default {


    name: 'RatingControl',

    data() {



        return {
            

            activeable:null,


        };
    },

    mounted() {
        
    },

    methods: {
        

        actived(option){

           this.activeable=option;  
             
            console.log('this is an option',this.activeable);

        }
    },
};
</script>

<style lang="css" scoped>


.active{

border-color: #920965;


}



.active button{


color: #920965;

}
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