<template>
  <v-container fluid grid-list-md style="background:#2b44ff;height: 100%;">
    <v-row>
        <v-col class="pa-0 ma-0" >
            <Mobile/>
        </v-col>
        <v-col class="pa-0 ma-0">
            <vue-terminal :task-list="taskList" :command-list="commandList" />
        </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Mobile from "./Mobile.vue"
import VueTerminal from 'vue-terminal';
export default {
    components: {
        Mobile,
        VueTerminal
    },
    data(){
        return {
            taskList:{},
            commandList: {}
        }
    }

}
</script>

<style>

</style>