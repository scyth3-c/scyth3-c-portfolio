<template>
    
      <b-container class="mt-4">
    
          <span title="about me" class="font-weight-bold ch-text-v">About Me</span> <br>
          <hr class="sp-line">

            <b-card class="my-2 shadow-lg">
                <b-icon icon="chat-square-dots-fill"> </b-icon> <span title="kevin" class="text-secondary">Kevin~</span>
                <hr>
                My name is Kevin, and I am 20 years old. I reside in Colombia. My journey into the world of electronics and programming began during high school, where I ventured to explore this fascinating field.
            </b-card>

            <b-card class="my-2 shadow-lg">
                <b-icon icon="chat-text-fill"> </b-icon> <span class="text-secondary">Kevin Bohorquez</span>
                <hr>
                I have hands-on experience working with various microcontrollers, programmable boards, and embedded systems. Some examples of these include Pic, Arduino, Raspberry Pi, and more.
             </b-card>

            <b-card class="shadpow-lg">
                <b-icon icon="chat-right-text-fill"> </b-icon> <span class="text-secondary">scyth3-c</span>
                <hr>
                I started my journey in the programming world on my own with C++. Since then, I have discovered how much I enjoy this field. I have been experimenting with new technologies and languages, including JavaScript, Python, PHP, and more. Currently, my ambition is to work as a web developer, while continuously learning and exploring new technologies. 
            </b-card>
        
    </b-container>

</template>

<script>
export default {
    name: 'aboutVue'
}
</script>

<style>

.ch-text-v {
    text-shadow: 2px 1px 2px white;
    padding: 3px;
    font-weight: bold;
        color: black;
  }
  
  @media (max-width: 768px) {
    .ch-text-v{
        text-shadow: 2px 1px 2px black;
      color: white;
    }
  }
  
</style>