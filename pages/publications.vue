<template>
    <div>
        <div class="slogan">
            <div class="container mx-auto px-4">
                <div class="text-2xl font-bold">
                    Publications
                </div>
                <div class="font-semibold mt-2">
                    List of our recent publications 
                </div>
            </div>
        </div>
        <div class="container mx-auto py-10 px-4">
            <ul>
                <li v-for="publication in publications">{{ publication.title }}</li>
            </ul>
        </div>


        
  
        <!-- Repeat similar code for more cards -->
  
        <!-- Add more cards as needed -->
    </div>  
    </div>

  </template>
  
  <script>

import {
    publications,
} from '~/docs/publications.json'


  export default {
    data() {
    return {
        publications
    };
  },
  }
  </script>
  
<style scoped>

    .slogan {
        background-color: #EFF7EB;
        padding: 3rem 0;
    }

        /* Define a custom square bullet style */
    ul {
        list-style-type: none;
        padding: 0;
    }

    ul li::before {
        content: "\25A0"; /* Unicode character for a solid square */
        color: #fff; /* Bullet color */
        display: inline-block;
        width: 1rem; /* Adjust the size of the square */
        margin-right: 0.5em; /* Adjust the spacing between the square and the text */
        text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5); /* Add a shadow to the square */
        font-size: 1.5rem; 
    }

    /* Some additional styling for the list items */
    ul li {
        margin-bottom: 1.5rem;
        font-size: 1rem; 
        line-height: 1.5rem; 
        font-weight: 600;
    }
</style>
  