<template>
    <div>
        <p v-if="!server"> selecte a server</p>
        <p v-else>{{server.id}} selected status: {{server.status}}</p>
    </div>
</template>

<script>
import {serverBus} from '../../main'
export default {
    //lo qeu hago segundo
    data: function() {
        return {
            server: null
        }
    },
    //lo que hago primer
    created() {
        serverBus.$on('serverSelected', (server) => this.server = server)
        // la parte del callback es la tercera y ultima
    }
}
</script>