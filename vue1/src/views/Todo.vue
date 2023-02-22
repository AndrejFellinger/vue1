<template>
    <h1>I really made it !</h1>
    <button @click="count ++">{{ count }}</button>


    <ol>
        <li v-for="kokos in list">{{ kokos }}</li>
    </ol>

    <input type="text" v-model="test" />
    <p>{{ test + ' ahoj' + count }}</p>


</template>

<script>

export default {
    data() {
        return {
            count: 1,
            list: ['hey', 'gey', "let's gooo", 'finally', 'made ITTTTTTT'],
            test: 'wd'
        }
    },
}
</script>

<style lang="">
    
</style>