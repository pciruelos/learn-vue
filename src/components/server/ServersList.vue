<template>
    <div>
        <ul>
            <ServerItem v-for="(server,i) in servers" :server="server" :key="i"> 

            </ServerItem>
        </ul>
    </div>
</template>

<script>
import ServerItem from '../ServerItem.vue'

export default {
    
    components: {
        ServerItem
    },
    data: function(){
        return {
            servers: [
                {id:1,status: 'normal'},
                {id:2,status: 'critical'},
                {id:3,status: 'unknow'},
                {id:4,status: 'normal'},
            ]
        }
    }
}
</script>

<style scoped>

</style>