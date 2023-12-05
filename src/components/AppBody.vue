<script>
import AppFreeLesson from './AppFreeLesson.vue';
import AppLearningDrive from './AppLearningDrive.vue';
import AppCourses from './AppCourses.vue';
import AppInstructors from './AppInstructors.vue';
import AppTestimonials from './AppTestimonials.vue';
import AppLatestNews from './AppLatestNews.vue';
import AppNewsletter from './AppNewsletter.vue';


export default {
    data() {
        return {};
    },
    components: { AppFreeLesson, AppLearningDrive, AppCourses, AppInstructors, AppTestimonials, AppLatestNews, AppNewsletter }
}
</script>
<template>
<AppFreeLesson />
<AppLearningDrive />
<AppCourses />
<AppInstructors />
<AppTestimonials />
<AppLatestNews />
<AppNewsletter />

</template>
<style scoped lang="scss">
body {
    width: 100%;
}
</style>