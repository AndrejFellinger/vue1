<template>
    <h1>I really made it !</h1>
    <button @click="count ++">{{ count }}</button>


    <ol>
        <li v-for="kokos in list">{{ kokos }}</li>
    </ol>

    <input type="text" v-model="test" />
    <input type="submit" value="add" @click="storeTest">

    <p>{{ test }}</p>


</template>

<script>

export default {
    data() {
        return {
            count: 1,
            list: ['hey', 'gey', "let's gooo", 'finally', 'made ITTTTTTT'],
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

<style lang="">
    
</style>