<script>
    export default{
        data(){
            return{
                    courses: [
                        {
                            id: 1,
                            title: "Fundamentals of Italian Cooking",
                            chef: "Gianni Moretti",
                            price: 89.99,
                            skill: "Beginner",
                            availability: true
                        },
                        {
                            id: 2,
                            title: "Modern French Cuisine Techniques",
                            chef: "Claire Duval",
                            price: 129.00,
                            skill: "Intermediate",
                            availability: true
                        },
                        {
                            id: 3,
                            title: "Mastering Japanese Knife Skills",
                            chef: "Hiroshi Takeda",
                            price: 149.50,
                            skill: "Advanced",
                            availability: false
                        },
                        {
                            id: 4,
                            title: "Plant-Based Cooking for Everyone",
                            chef: "Amara Lewis",
                            price: 79.99,
                            skill: "Beginner",
                            availability: true
                        },
                        {
                            id: 5,
                            title: "The Art of Pastry & Desserts",
                            chef: "Lucille Moreau",
                            price: 140.00,
                            skill: "Intermediate",
                            availability: true
                        },
                        {
                            id: 6,
                            title: "Authentic Mexican Street Food",
                            chef: "Carlos Mendoza",
                            price: 95.00,
                            skill: "All Levels",
                            availability: true
                        },
                        {
                            id: 7,
                            title: "Professional Bread Baking",
                            chef: "Elena Fischer",
                            price: 120.00,
                            skill: "Advanced",
                            availability: false
                        },
                        {
                            id: 8,
                            title: "Seafood Mastery & Fine Dining Plates",
                            chef: "Miguel Santos",
                            price: 159.00,
                            skill: "Advanced",
                            availability: true
                        },
                        {
                            id: 9,
                            title: "Quick & Healthy 20-Minute Meals",
                            chef: "Sophie Andrews",
                            price: 59.99,
                            skill: "Beginner",
                            availability: true
                        },
                        {
                            id: 10,
                            title: "BBQ, Smoking & Meat Perfection",
                            chef: "Jack Ruger",
                            price: 110.00,
                            skill: "Intermediate",
                            availability: true
                        }
                    ]

            }
        }
    }
</script>

<template>
    <ul>
        <li v-for="course in courses">
            <fieldset>
                {{ course.title }}
                <br>
                {{ course.chef }}
                <br>
                {{ course.price }}
                <br>
                {{ course.skill}}

            </fieldset>
        </li>
    </ul>
</template>

<style>
ul li{
    list-style: none;
    padding-bottom: 20px;
}

fieldset{
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 10px;
}
</style>
