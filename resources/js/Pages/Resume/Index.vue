<template>
    <Header />

    <div class="container">
        <div class="p-3 left-column">
            <Contact />

            <Skills />

            <Education />
        </div>

        <div class="right-column">
            <ProfessionalProfile />

            <Experience />
        </div>
    </div>
</template>

<script>
import Header from "@/Components/Resume/Header.vue";
import Contact from "@/Components/Resume/Contact.vue";
import Skills from "@/Components/Resume/Skills.vue";
import Education from "@/Components/Resume/Education.vue";
import ProfessionalProfile from "@/Components/Resume/ProfessionalProfile.vue";
import Experience from "@/Components/Resume/Experience.vue";

export default {
    components: {
        Header, Contact, Skills, Education, ProfessionalProfile, Experience
    },
};
</script>

<style scoped>
    .container {
        display: flex;
        flex-direction: row;
    }

    .left-column {
        width: 30%;
        border-right: 1px solid lightblue;
    }

    .right-column {
        width: 70%;
        text-align: center;
    }
</style>
