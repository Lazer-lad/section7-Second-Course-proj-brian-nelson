<template>
    <v-col cols="6">
        
                <v-list>
                    <v-list-item-content v-for="index in 5" :key="index">
                      
                    Server #{{ index }}
<v-divider :inset="inset"></v-divider>

                    </v-list-item-content>
                </v-list>
            </v-col>
</template>