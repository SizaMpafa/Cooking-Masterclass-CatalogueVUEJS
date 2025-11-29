<script>
export default {
    props: {
        courses: Array
    },

    computed: {
        savedCourses() {
            return this.courses.filter(course => course.isSaved)
        },

        amountSaved() {
            return this.savedCourses.length
        }
    }
}
</script>

<template>
    <div class="dropdown w-100">
        <button 
            class="btn btn-secondary dropdown-toggle w-100" 
            type="button"
            id="dropdownMenuButton"
            data-bs-toggle="dropdown"
        >
            Wishlist ({{ amountSaved }})
        </button>

        <div class="dropdown-menu w-100" aria-labelledby="dropdownMenuButton">

            <a 
                v-for="course in savedCourses"
                :key="course.id"
                class="dropdown-item"
            >
                {{ course.title }}
            </a>

            <span 
                v-if="savedCourses.length === 0" 
                class="dropdown-item text-muted"
            >
                No courses saved
            </span>
        </div>
    </div>
</template>

<style scoped>
.dropdown-menu {
    max-height: 300px;
    overflow-y: auto;
}
</style>
