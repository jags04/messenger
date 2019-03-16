<template>
    <b-media :right-align="writtenByMe" vertical-align="center" class="mb-2">
        <b-img slot="aside" rounded="circle" blank width="48" blank-color="#777"  alt="Circle image" class="m-1" />
        <b-card>
            <slot></slot>
        </b-card>
    </b-media>
</template>


<script>
    export default {
        props:{
            writtenByMe: Boolean
        },
        data(){
            return {
                content : ''
            }
        },
        mounted() {
            console.log('Component mounted.')
        }
    }
</script>

