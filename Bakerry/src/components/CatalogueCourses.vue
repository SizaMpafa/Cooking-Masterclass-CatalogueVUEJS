<script>
    export default{
        data(){
            return{
                    courses: [
    {
        "id": 1,
        "title": "Fundamentals of Italian Cooking",
        "chef": "Gianni Moretti",
        "price": 89.99,
        "skill": "Beginner",
        "availability": true,
        "imageSrc": "https://images.squarespace-cdn.com/content/v1/5dd5b5e9f226644911c4d733/abf69080-4f8f-4385-8f42-f147478a59cc/italian-cooking-classes-in-italy.jpg"
    },
    {
        "id": 2,
        "title": "Modern French Cuisine Techniques",
        "chef": "Claire Duval",
        "price": 129.00,
        "skill": "Intermediate",
        "availability": true,
        "imageSrc": "https://www.thespruceeats.com/thmb/pahH2ciNrqG4m3qq6WkN03hEYaM=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/different-courses-in-formal-french-meal-1375353_final-ddd9245e8d994258ad4bd967b20e32d2.png"
    },
    {
        "id": 3,
        "title": "Mastering Japanese Knife Skills",
        "chef": "Hiroshi Takeda",
        "price": 149.50,
        "skill": "Advanced",
        "availability": false,
        "imageSrc": "https://i.ytimg.com/vi/FDNNG9doFe4/hq720.jpg?sqp=-oaymwEhCK4FEIIDSFryq4qpAxMIARUAAAAAGAElAADIQj0AgKJD&rs=AOn4CLCtEB-OlY7qODLGuZwcQpWuy6OuEQ"
    },
    {
        "id": 4,
        "title": "Plant-Based Cooking for Everyone",
        "chef": "Amara Lewis",
        "price": 79.99,
        "skill": "Beginner",
        "availability": true,
        "imageSrc": "https://prodimage.images-bn.com/pimages/9781621455776_p3_v4_s600x595.jpg"
    },
    {
        "id": 5,
        "title": "The Art of Pastry & Desserts",
        "chef": "Lucille Moreau",
        "price": 140.00,
        "skill": "Intermediate",
        "availability": true,
        "imageSrc": "https://thepastryacademy.com/wp-content/uploads/2022/12/dc.jpg"
    },
    {
        "id": 6,
        "title": "Authentic Mexican Street Food",
        "chef": "Carlos Mendoza",
        "price": 95.00,
        "skill": "All Levels",
        "availability": true,
        "imageSrc": "https://media-cdn.tripadvisor.com/media/attractions-splice-spp-674x446/0e/10/a3/d6.jpg"
    },
    {
        "id": 7,
        "title": "Professional Bread Baking",
        "chef": "Elena Fischer",
        "price": 120.00,
        "skill": "Advanced",
        "availability": false,
        "imageSrc": "https://www.ice.edu/sites/default/files/content/program/header-video-image/Bread-167-72dpi.jpg"
    },
    {
        "id": 8,
        "title": "Seafood Mastery & Fine Dining Plates",
        "chef": "Miguel Santos",
        "price": 159.00,
        "skill": "Advanced",
        "availability": true,
        "imageSrc": "https://i.ytimg.com/vi/iZ0NQHNDXgg/hq720.jpg?sqp=-oaymwEhCK4FEIIDSFryq4qpAxMIARUAAAAAGAElAADIQj0AgKJD&rs=AOn4CLBH96s2CbG2TITDRDK-NiWySuuXUg"
    },
    {
        "id": 9,
        "title": "Quick & Healthy 20-Minute Meals",
        "chef": "Sophie Andrews",
        "price": 59.99,
        "skill": "Beginner",
        "availability": true,
        "imageSrc": "https://www.allrecipes.com/thmb/9bjdeeY3e7OWke-gx33cYM2S8Ls=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/AR-Pizza-Lava-Toast-4x3-0de18c7a898346dfab1ede9f00471aed.jpg"
    },
    {
        "id": 10,
        "title": "BBQ, Smoking & Meat Perfection",
        "chef": "Jack Ruger",
        "price": 110.00,
        "skill": "Intermediate",
        "availability": true,
        "imageSrc": "https://assets3.thrillist.com/v1/image/3119896/792x529/scale;webp=auto;jpeg_quality=60;progressive.jpg"
    }
]

            }
        }
    }
</script>

<template>
    <ul>
        <li v-for="course in courses">
            <div class="card" style="width: 50rem;">
    <!-- If you have an image source in your data, you can use it here -->
    <img :src="course.imageSrc" class="card-img-top" alt="Course image">
    
    <div class="card-body">
      <!-- Title -->
      <h5 class="card-title">{{ course.title }}</h5>

      <!-- Chef/Skill/Price Info -->
      <p class="card-text">
        <strong>Chef:</strong> {{ course.chef }}
      </p>
      <p class="card-text">
        <strong>Skill Level:</strong> {{ course.skill }}
      </p>
      <p class="card-text">
        <strong>Price:</strong> {{ course.price }}
      </p>

      <!-- Example Button -->
      <a href="#" class="btn btn-primary">Enroll Now</a>
    </div>
  </div>
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
