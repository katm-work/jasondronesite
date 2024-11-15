<template>
    <div class="contact-page">
        <div class="contact-header">
            <h1>Contact Us</h1>
        </div>
        <section class="contact-info">
            <p>Email: <a href="mailto:support@example.com">support@example.com</a></p>
            <p>Phone: <a href="tel:+1234567890">+1 (234) 567-890</a></p>
            <p>Address: 123 Main Street, Springfield, USA</p>
        </section>
    </div>

</template>

<style scoped>
.contact-header {
    display: flex;
    width: 250px;
    border: none;
    border-radius: 5px;
    height: 50px;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: #EDF2F4;
    background-color: #2c3e50;
}

.contact-page {
    display: flex;
    flex-direction: column;
    text-align: left;
    justify-content: center;
    align-items: center;
    padding: 20px;

}
</style>