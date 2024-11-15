<template>
    <div id="service-main">
        <h1 id="service-header">Our Services</h1>
    </div>
    <!-- Buttons to switch content -->
    <div class="button-group">
        <button class='styled-btn' @click="changeContent('option1')">Surveying</button>
        <button class='styled-btn' @click="changeContent('option2')">Building Showcase</button>
        <button class='styled-btn' @click="changeContent('option3')">Videography</button>
    </div>

    <!-- Display Field -->
    <div class="display-field">
        <img src="../assets/dronesurvey.png" v-if="selectedContent === 'option1'" />
        <img src="../assets/dronecity.png" v-else-if="selectedContent === 'option2'" />
        <img src="../assets/dronehouse.png" v-else-if="selectedContent === 'option3'" />
    </div>

</template>

<script>
export default {
    data() {
        return {
            selectedContent: null
        };
    },
    methods: {
        changeContent(option) {
            this.selectedContent = option;
        }
    }
};
</script>

<style scoped>
.styled-btn {
    background-color: #2c3e50;
    color: #EDF2F4;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.styled-btn:hover {
    background-color: #2980b9;
}

#service-main {
    display: flex;
    padding: 20px 300px;
    justify-content: center;
}

#service-header {
    width: 300px;
    border: none;
    border-radius: 5px;
    height: max-content;
    text-align: center;
    margin: 5px 2px;
    color: #EDF2F4;
    background-color: #2c3e50;
}

.button-group {
    margin-bottom: 1em;
}

button {
    margin-right: 10px;
}

.display-field {
    padding: 1em;
    background-color: #4D685A;
}

.display-field img {
    display: flex;
    width: 600px;
    height: 400px;
    margin: auto;
}
</style>