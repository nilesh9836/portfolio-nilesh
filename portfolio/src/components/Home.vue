<template>
    <v-container fluid grid-list-md style="background:#2b44ff;height: 100%;">
        <v-row no-gutters>
            <v-col class="pa-0 ma-0 pt-6 pr-6" style="align-items: end;display: flex;">
                <v-spacer></v-spacer>
                <Mobile />
            </v-col>
            <v-col class="pa-0 ma-0 pa-8">
                <vue-terminal :task-list="taskList" :command-list="commandList" :showHeader="false"
                    :greeting="greeting" />
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
    data() {
        return {
            taskList: {},
            commandList: {},
            greeting: `<pre>Hello! I'm Nilesh Mishra 
                       Here's some facts about me:
                        ✅ Web Developer
                        ✅ App Developer
                        ✅ Cricket Fanatic</pre>`
        }
    }

}
</script>

<style>

</style>