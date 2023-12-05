<script>
import AppFreeLesson from './AppFreeLesson.vue';
import AppLearningDrive from './AppLearningDrive.vue';
import AppCourses from './AppCourses.vue';


export default {
    data() {
        return {};
    },
    components: { AppFreeLesson, AppLearningDrive,AppCourses }
}
</script>
<template>
<AppFreeLesson />
<AppLearningDrive />
<AppCourses />

</template>
<style scoped lang="scss">

</style>