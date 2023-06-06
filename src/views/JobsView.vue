<template>
    <h1>Jobs</h1>
    <div v-for="job in jobs" :key="job.id" class="job">
        <router-link :to="{name: 'JobsDetail', params:{id: job.id}}">
            <h1>{{ job.title }}</h1>
        </router-link>
    </div>
</template>

<script>
export default {
    data () {
        return {
            jobs: [
                {title: 'UX Designer', id: 1, details: 'This is UX designing Job'},
                {title: 'Web developer', id: 2, details: 'This is Web developer Job'},
                {title: 'Android developer', id: 3, details: 'This is android developer Job'}
            ]
        }
    }

}
</script>

<style>
    .job h1 {
        background: #e9e9e9;
        padding: 20px;
        border-radius: 10px;
        margin: 10px auto;
        max-width: 600px;
        cursor: pointer;
        color: #0a0a0a44;
    }
    .job h2:hover {
        background: #cdc2c2dd;
    }
    .job a {
        text-decoration: none;
    }
</style>