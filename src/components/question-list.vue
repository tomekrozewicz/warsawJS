<template>
    <section>
        <question-list-element v-for="question in questions" :key="question.title" :question="question"></question-list-element>
    </section>
</template>
<script>
import QuestionListElement from './question-list-element.vue';
    export default {
        name: 'QuestionList',
        components: {
            QuestionListElement
        },
        props: {
            questions: Array
        }
    }
</script>
<style scoped>
</style>