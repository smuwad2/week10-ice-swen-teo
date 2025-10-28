<script>

    export default {
        // Add code if/as necessary
        // Hint: Add properties subject, entry and mood
        
        props: {
            subject: String,
            entry: String,
            mood: String
        },
        computed: {
            img_url(){
                return "/assets/" + this.mood.toLowerCase() + ".png"
            }
        }
    }
</script>


<template>
    <!-- TODO: add your template code here. Use bootstrap card --> 
    <div class="card" style="width: 18rem; margin: 10px;">
    <img :src="img_url" class="card-img-top">
    <div class="card-body">
        <h5 class="card-title">{{subject}}</h5>
        <p class="card-text">{{entry}}</p>
    </div>
    </div>
</template>

