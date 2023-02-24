<template>

    <div class="container">
        <h1>Todo List</h1>

        <ol>
            <li v-for="kokos in list">{{ kokos }}</li>
        </ol>

        <input type="text" v-model="test" placeholder="start typing..." />
        <input class="submit" type="submit" value="ADD" name="add" @click="storeTest">
    </div>



</template>

<script>

export default {
    data() {
        return {
            list: [],
            test: ''
        }

    },

    methods: {
        storeTest(){
            this.list.push(this.test)
        }
    },
}
</script>

<style scoped>

    .container{
        background: white;
        display: grid;
        grid-template-columns: auto;
        color: rgb(27, 27, 27);
        padding: 20px;
        border-radius: 5px;
        justify-content: center;
        align-items: center;
        box-shadow: 0 0 15px rgba(255, 255, 255, 0.24);
        max-height: 800px;
        overflow: scroll;
    }

    h1{
        text-align: center;
        border-bottom: 1px solid rgb(212, 212, 212);
    }

    ol{
        font-size: 18px;
        text-align: left;
        
    }

    input{
        padding: 5px;
        outline: none;
        border: none;
        background: rgb(212, 212, 212);
        margin: 3px;
        border-radius: 3px;
    }

    .submit{
        color: green;
        background: greenyellow;
    }

</style>