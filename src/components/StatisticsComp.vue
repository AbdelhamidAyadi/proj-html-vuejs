<template>
    <div class="statistics_container">
        <img src="../assets/img/background-pattern-grid-line-06.png" alt="">
        <div class="single_statistic">
            <div>1.926</div>
            <div>FINISHED SESSIONS</div>
        </div>
        <img src="../assets/img/background-pattern-grid-line-06.png" alt="">
        <div class="single_statistic">
            <div>100%</div>
            <div>SATISFACTION RATE</div>
        </div>
        <img src="../assets/img/background-pattern-grid-line-06.png" alt="">
        <div class="single_statistic">
            <div>3092+</div>
            <div>ENROLLED LEARNERS</div>
        </div>
        <img src="../assets/img/background-pattern-grid-line-06.png" alt="">
        <div class="single_statistic">
            <div>200</div>
            <div>ONLINE INSTRUCTORS</div>
        </div>
        <img src="../assets/img/background-pattern-grid-line-06.png" alt="">


    </div>
</template>

<script>
    export default {
        name: 'StatisticsComp',
        props: {}
    }
</script>

<style scoped lang="scss">
    .statistics_container {
        padding: 0 15%;
        display: flex;
        justify-content: space-around;
        margin-bottom: 50px;
    }

    .single_statistic {
        text-align: center;
        
        div:first-of-type{
            color: #20ad96;
            font-size: 2rem;
            font-weight: bold;
            margin-bottom: 15px;
        }
        
    }
</style>