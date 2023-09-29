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
        <div v-for="member in members" class="member flex flex-col bg-transparent py-10 divide-black bg-white opacity-80">
            <div class="header flex flex-row justify-between">
                <div class="intro flex flex-row">

                  <div class="h-48">
                    <div class="h-full w-48 flex flex-col overflow-visible">
                      <img class="w-full rounded-full object-cover min-h-0" :src="require('~/assets/member_images/' + member.image)"/>
                    </div>
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
                    <a v-for="({ link }, platform) in member.links" :href="link">{{ platform}}</a>
                </div>
            </div>

            <div class="body flex flex-row mt-5">
                <div class="description leading-7 text-base" v-html="member.aboutMe">

                </div>
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
