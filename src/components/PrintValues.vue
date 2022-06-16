<template>
    <div v-for="task in tasks"> 

          <div class="content">
            {{ task.id }} 

        </div>
    </div>
</template>
<script>
import axios from 'axios'
import { response } from 'express';
    export default {
        name:'PrintValues',
        data(){
            return {
                tasks: []
            }
        },
        mounted(){
            this.get_Tasks();
        },
        methods: {
            get_Tasks(){
                axios({
                    method:'get',
                    url:'http://127.0.0.1:8000/user/',
                    auth: {
                        username:'your name',
                        password:'your Password'
                    }
                }).then(response=>this.tasks =response.data);
            }
        }
    }

</script>
<style scoped>

</style>