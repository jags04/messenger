<template>
    <b-list-group-item :variant="variant">
        <b-row class="p-2">
            <b-col cols="12" md="3" class="text-center">
                <b-img rounded="circle" blank width="60" height="60" blank-color="#777"  alt="Circle image" class="m-1" />
            </b-col>
            <b-col cols="7" align-self="center" class="d-none d-md-block">
                <p class="mb-0">{{ name }}</p>
                <p class="text-muted small mb-0">{{ lastMessage }}</p>
            </b-col>
            <b-col cols="2" class="d-none d-md-block">
                <p class="text-muted small">{{ lastTime }}</p>
            </b-col>
        </b-row>
    </b-list-group-item>
</template>

<script>
    export default {
        props: [
            'variant'
        ],
        data(){
            return {
                name : 'Jesus Gil',
                lastMessage: 'Tú: Hasta luego',
                lastTime: '1:32 pm',
            }
        },
        mounted() {
            console.log('Component mounted.')
        }
    }
</script>
