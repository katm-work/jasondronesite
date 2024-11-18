<template>
    <img :src="logoSrc" :alt="altText" :class="logoClass" />
</template>

<script>
export default {
    name: 'Logo',
    props: {
        logoSrc: {
            type: String,
            default: require('@/assets/dronelogo.jpg')
        },
        altText: {
            type: String,
            default: 'Logo'
        },
        logoClass: {
            type: String,
            default: ''
        }
    }
};
</script>
