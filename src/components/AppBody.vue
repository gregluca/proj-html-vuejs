<script>
import AppFreeLesson from './AppFreeLesson.vue';
import AppLearningDrive from './AppLearningDrive.vue';
import AppCourses from './AppCourses.vue';
import AppInstructors from './AppInstructors.vue';


export default {
    data() {
        return {};
    },
    components: { AppFreeLesson, AppLearningDrive, AppCourses, AppInstructors }
}
</script>
<template>
<AppFreeLesson />
<AppLearningDrive />
<AppCourses />
<AppInstructors />

</template>
<style scoped lang="scss">

</style>