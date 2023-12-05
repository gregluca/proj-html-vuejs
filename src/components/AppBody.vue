<script>
import AppFreeLesson from './AppFreeLesson.vue';
import AppLearningDrive from './AppLearningDrive.vue';
import AppCourses from './AppCourses.vue';
import AppInstructors from './AppInstructors.vue';
import AppTestimonials from './AppTestimonials.vue';
import AppLatestNews from './AppLatestNews.vue';


export default {
    data() {
        return {};
    },
    components: { AppFreeLesson, AppLearningDrive, AppCourses, AppInstructors, AppTestimonials, AppLatestNews }
}
</script>
<template>
<AppFreeLesson />
<AppLearningDrive />
<AppCourses />
<AppInstructors />
<AppTestimonials />
<AppLatestNews />

</template>
<style scoped lang="scss">
body {
    width: 100%;
}
</style>