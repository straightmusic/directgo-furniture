<template>
    <button class="appointment-btn">
        {{ btnText }}
    </button>
</template>

<script setup>
defineProps({
    btnText: String,
})
</script>

<style scoped>
.appointment-btn {
    font-size: 0.5rem;
    color: #FFFFFF;

    height: 3rem;
    background: #000000;
    box-shadow: 0px 8px 8px rgba(0, 0, 0, 0.25);
    border-radius: 2000px;

    cursor: pointer
}
</style>