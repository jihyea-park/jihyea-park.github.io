<template>
  <p> Zugeordnet mit deutschen Tastatur </p>
  <input id="userInput" type="text" v-model="eingabe" @keypress="playSound" onblur="this.focus()" autofocus>
  <template v-for="item in eingabe_list" :key="item"> 
    <!-- <span id="showInput">{{ item }}</span>  -->
  </template>

  <KeyInteraction v-if="showInteraction" :theme="key_"/>
</template>

<script>
import KeyInteraction from './components/KeyInteraction.vue'

export default {
  name: 'App',
  components: { KeyInteraction },
  data() {
    return {
      showInteraction: false,
      eingabe: '',
      key_: '',
      eingabe_list: [],
      audio_list: [
        { alph: 'a', src: 'http://127.0.0.1:8887/audio/kick1.mp3'},
        { alph: 'b', src: 'http://127.0.0.1:8887/audio/key_b6.mp3'},
        { alph: 'c', src: 'http://127.0.0.1:8887/audio/snap.mp3'},
        { alph: 'd', src: 'http://127.0.0.1:8887/audio/clap_phat.mp3'},
        { alph: 'e', src: 'http://127.0.0.1:8887/audio/hihat2.mp3'},
        { alph: 'f', src: 'http://127.0.0.1:8887/audio/key_a8.mp3'},
        { alph: 'g', src: 'http://127.0.0.1:8887/audio/key_b1.mp3'},
        { alph: 'h', src: 'http://127.0.0.1:8887/audio/key_b2.mp3'},
        { alph: 'i', src: 'http://127.0.0.1:8887/audio/key_a5.mp3'},
        { alph: 'j', src: 'http://127.0.0.1:8887/audio/key_b3.mp3'},
        { alph: 'k', src: 'http://127.0.0.1:8887/audio/key_b4.mp3'},
        { alph: 'l', src: 'http://127.0.0.1:8887/audio/key_b5.mp3'},
        { alph: 'm', src: 'http://127.0.0.1:8887/audio/key_b8.mp3'},
        { alph: 'n', src: 'http://127.0.0.1:8887/audio/key_b7.mp3'},
        { alph: 'o', src: 'http://127.0.0.1:8887/audio/key_a6.mp3'},
        { alph: 'p', src: 'http://127.0.0.1:8887/audio/key_a7.mp3'},
        { alph: 'q', src: 'http://127.0.0.1:8887/audio/kick_loop.mp3'},
        { alph: 'r', src: 'http://127.0.0.1:8887/audio/key_a1.mp3'},
        { alph: 's', src: 'http://127.0.0.1:8887/audio/snare.mp3'},
        { alph: 't', src: 'http://127.0.0.1:8887/audio/key_a2.mp3'},
        { alph: 'u', src: 'http://127.0.0.1:8887/audio/key_a4.mp3'},
        { alph: 'v', src: 'http://127.0.0.1:8887/audio/vocal.mp3'},
        { alph: 'w', src: 'http://127.0.0.1:8887/audio/hihat.mp3'},
        { alph: 'x', src: 'http://127.0.0.1:8887/audio/clap_phaser2.mp3'},
        { alph: 'y', src: 'http://127.0.0.1:8887/audio/clap_phaser.mp3'},
        { alph: 'z', src: 'http://127.0.0.1:8887/audio/key_a3.mp3'},
        { alph: ',', src: 'http://127.0.0.1:8887/audio/key_b9.mp3'},
        { alph: '.', src: 'http://127.0.0.1:8887/audio/key_b10.mp3'},
        { alph: 'ü', src: 'http://127.0.0.1:8887/audio/key_1n.mp3'},
        { alph: 'ö', src: 'http://127.0.0.1:8887/audio/key_2n.mp3'},
        { alph: 'ä', src: 'http://127.0.0.1:8887/audio/key_3n.mp3'},
      ],
      duration: 0,
      drums: ["Q", "W", "E", "A", "S", "D", "Y", "X", "C", "V"]
    }
  },
  methods: {
    playSound(e) {
      this.key_ = e.key.toUpperCase()
      // var ein = e.key.toUpperCase()
      var index = this.audio_list.map(function(element) {return element.alph.toUpperCase()}).indexOf(this.key_)

      if (index != -1) {
        this.showInteraction = true  
        this.eingabe_list.push(this.key_)
        var audio = new Audio(this.audio_list[index].src)
        // audio.addEventListener('loadeddata', () => {
        //   this.duration = audio.duration * 1000
        //   console.log(this.duration)
        // })
        // setTimeout(function() {
        //   this.showInteraction = false
        // }, this.duration)        
        audio.play()
        this.eingabe = ''
      } else {
        this.eingabe = ''
      } 
    }
  },
  // mounted() {
  //   var self = this;

  //   setTimeout(function() {
  //     self.showInteraction = false;
  //   }, 1000)
  // }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  margin-top: 60px;
}

body {
  background-color: black;
  color: white;
}

#userInput {
  background-color: black;
  width: 100%;
  box-sizing: content-box;
  border: none;
  resize: none;
  text-align: start;
  margin: 20px;
}

*:focus {
  outline: none !important;
}

#showInput {
  font-size: 30px;
  margin: 2px;
}

</style>
