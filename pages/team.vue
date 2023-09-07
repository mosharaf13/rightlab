<template>
    <div>
        <div class="slogan ">
            <div class="container mx-auto px-4">
                <div class="text-2xl font-bold">
                    The team that makes it all happen
                </div>
                <div class="font-bold mt-2">
                    Exploring Human Behavior for a better tomorrow
                </div>
            </div>
        </div>
        <div class="container mx-auto w-3/5">
        <div v-for="member in members" class="member flex flex-col bg-transparent rounded py-10 divide-black bg-white opacity-80">
            <div class="header flex flex-row justify-between">
                <div class="intro flex flex-row">
                    <div class="image">
                        <img class="w-28 h-28 rounded-full object-cover" :src="require('~/assets/member_images/' + member.image)" />
                    </div>
                    <div class="identity flex flex-col justify-center mx-5">
                        <div class="name">
                            <h2 class="text-2xl font-bold mb-3">{{ member.firstName }} {{ member.lastName }}</h2> 
                        </div>
                        <div class="title">
                            <h3 class="text-base mb-2">{{ member.position }}</h3>
                        </div>
                    </div>
                </div>

                <div class="contact flex flex-col text-right text-base justify-center underline">
                    <a href="http://linkedin.com">LinkedIn</a>
                    <a href="http://linkedin.com">Google Scholar</a>
                    <a href="http://linkedin.com">ResearchGate</a>
                    <a href="http://linkedin.com">Personal Website</a>                    
                </div>
            </div>

            <div class="body flex flex-row mt-5">
                <div class="description leading-7 text-base">

                    Rifat Ara Tasnim is a second year PhD student in Computer Science at the University of New Orleans. She is currently working as a research assistant under Dr. Farjana Zebin Eishita at the Idaho State University.
                    <br> <br> Her main research interest focuses on providing psychological treatment through wearable or handheld devices using serious games. Her current research explores incorporating CBT in video games playable in smartphones. Her primary concern is to implement CBT in a video game to treat young adults who have Obsessive Compulsive Disorder (OCD). She is also working on a digital game to detect different types of cognitive distortions present among the players. 

                    <br> <br>Rifat holds a B.Sc. in Computer Science and Engineering from Khulna University of Engineering and Technology, Bangladesh. Before starting her PhD journey, she worked as a software engineer in an IT company.                </div>
            </div>
        </div>


        
  
        <!-- Repeat similar code for more cards -->
  
        <!-- Add more cards as needed -->
    </div>  
    </div>

  </template>
  
  <script>

import {
    members,
} from '~/docs/team_members.json'


  export default {
    data() {
    return {
      members
    };
  },
  }
  </script>
  
  <style scoped>
  .member{
    color: #24242E;
    font-weight: 500;
    border-bottom: 1px solid #241c15;
  }

  .slogan {
    background-color: #FBEECA;
    padding: 3rem 0;
  }
  </style>
  