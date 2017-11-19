<template>
    <section>
        <p class="questionTitle">{{ question.title }}</p>
        <answer-list :answers="question.answers"></answer-list>
    </section>
</template>
<script>
    import AnswerList from './answer-list.vue';
    export default {
        name: 'QuestionListElement',
        components: {
            AnswerList
        },
        props: {
            question: Object
        }
    }
</script>
<style scoped>
.questionTitle {
    font-size:30px;
}
</style>