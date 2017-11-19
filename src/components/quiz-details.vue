<<template>
    <section>
            <h2 class="hero is-primary" v-if="quiz">
                <h2  class="title">{{ quiz.name }}</h2>
                <div class="subtitle">{{quiz.categoryName}}</div>
            </h2>
            <img :src="quiz.promo" alt=""/>
            <question-list :questions="quiz.questions"></question-list>
    </section>
</template>
<script>
    import QuestionList from './question-list.vue';
    export default {
        name: 'QuizDetails',
        components: {
            QuestionList
        },
        props: {
            quiz: Object
        }
    }
</script>
