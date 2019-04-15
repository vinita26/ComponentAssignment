<template>
    <div>
        <div class="col-xs-12 col-sm-6">
            <p v-if="!server">Please select a server to display details</p>
            <p v-else>Server #{{server.id}} is selected,Server status: {{server.status}}</p>
            <hr>
            <button @click="resetStatus">Change Status</button>
        </div>
        
    </div>
</template>

<script>
    import { serverBus } from '../../main';

    export default {
        data: function() {
            return{
                server: null
            }
        },
        methods: {
            resetStatus(){
                this.server.status= 'Normal'
            }
        },
        created() {
            serverBus.$on('serverSelected',(server) => {
                this.server = server;
            })
        }
    }
</script>

<style>
</style>