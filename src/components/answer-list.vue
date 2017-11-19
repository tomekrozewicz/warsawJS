<template>
    <section>
        <answer-list-element v-for="answer in answers" :key="answer.title" :answer="answer"></answer-list-element>
    </section>
</template>
<script>
    import AnswerListElement from './answer-list-element.vue';
    export default {
        name: 'AnswerList',
        components: {
            AnswerListElement
        },
        props: {
            answers: Array
        }
    }
</script>
<style scoped>

</style>