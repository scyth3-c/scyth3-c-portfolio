<template>
     <b-container class="mt-5 contenedor col-md-6" >
    <b-badge class="w-100 text-white font-weight-bolder mx-auto p-1" variant="dark">Projects</b-badge>
    <b-carousel    
        id="carousel"
        style="text-shadow: 0px 0px 5px black;"
        v-model="open_slide"
        :interval="0"
        controls
        indicators
    >
      <a :href="slides[open_slide].link">
         <b-carousel-slide
         v-for="(slide, index) in slides"
        :key="index"
        :caption="slide.caption"
        :img-src="slide.src"
        :id="slide.link"
        class="vtam"
        text="click to open GitHub"
     >   
     </b-carousel-slide>
      </a>
    </b-carousel>
    </b-container>
</template>

<script>
export default {
    name: 'projectsVue',
    data() {
        return {
            slides: [
                {caption: "C++ Online Compiler", src: require("../assets/projects/compiler.png"), link: "https://github.com/scyth3-c/knock-cpp-online"},
                {caption: "C++ Terminal Chat Room", src: require("../assets/projects/chatroom.png"), link: "https://github.com/scyth3-c/rwnio-chatroom"},
                {caption: "C++ compile node api", src: require("../assets/projects/cpp-api.png"), link: "https://github.com/scyth3-c/knock-cpp-API"},
                {caption: "C++ anchor pincel", src: require("../assets/projects/gl-pincel.png"), link: "https://github.com/scyth3-c/gl-pincel"},
                {caption: "Public Notes App", src: require("../assets/projects/knocknotes.jpg"), link: "https://github.com/scyth3-c/Vue-Electron-Port"},
                {caption: "Public Desktop Notes App", src: require("../assets/projects/notesdesktop.jpg"), link: "https://github.com/scyth3-c/knock-notes-desktop"},
                {caption: "SHA256 Control", src: require("../assets/projects/sha256.jpg"), link: "https://github.com/scyth3-c/vue-knock-sha256"},
                {caption: "Discord Global Economy Bot", src: require("../assets/projects/discord.gif"), link: "https://github.com/scyth3-c/public-ccMegalo-bot-ramake"},
                {caption: "TypeScript API (demo without docker and cpp  addons)", src: require("../assets/projects/api.jpeg"), link: "https://github.com/scyth3-c/API-TS-NODEJS"},
                {caption: "Real Time Chat", src: require("../assets/projects/chat.png"), link: "https://github.com/scyth3-c/Node.js-sockets-chat"},
                {caption: "Pincel C++ OpenGL Legacy", src: require("../assets/projects/draw.jpg"), link: "https://github.com/scyth3-c/opengl-draw-all-modes"},
                {caption: "Text Font C++ OpenGL Legacy", src: require("../assets/projects/font.png"), link: "https://github.com/scyth3-c/opengl-comic-text-font"},
                {caption: "All Done for C++ GLFW", src: require("../assets/projects/lib.png"), link: "https://github.com/scyth3-c/glfw-glad-cmake-linux"},
                {caption: "Template for C++ Modern  OpenGL", src: require("../assets/projects/glfw.png"), link: "https://github.com/scyth3-c/modern-opengl-easy-template"},
            ],  
            open_slide: 0
        }
    }

}
</script>

<style>
.vtam {
   height:40vh;
   background: #292b2c;
 }
</style>