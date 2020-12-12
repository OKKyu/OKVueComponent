# Name  
  AudioBufPlayer  
  Free audio tag that only deal buffer.  

# Overview  
  Feature of This original audio tag is below.  
1.Made out of Vue.js  
2.Treat only array buffer (otherwords, only memory), not file or file's url  
3.Only Sequential playing, can't random access  
  (Because of using AudioBufferSourceNode)  

# Requirement  
   Vue.js  
    Please import Vue.js before importing AudioBufPlayer.js  

# Download  
  Please copy you to your any directory.  
  You can use browser or git command for downloading.  

# Setup  
  Please importing AudioBufPlayer.js on your html with script tag.
  And this package include default style and button image.  
  You may use AudioBufPlayerDefault.css for styling wether customize or not it.

# Usage
1. You shoud write AudioBufPlayer tag in your html code.  
    &lt;div id="AudioBufPlayer1"&gt;  
    &nbsp; &lt;audio-buf-player  
    &nbsp; &nbsp; v-bind:arybuf="arybuf"&gt;  
    &nbsp; &lt;/audio-buf-player&gt;  
    &lt;/div&gt;  
2. You shoud create instance of AudioBufPlayer in your javascript.  
  Sample code is below.  
    var player1 = new Vue({  
    &nbsp; &nbsp; el:'#AudioBufPlayer1',  
    &nbsp; &nbsp; &nbsp; data:{  
    &nbsp; &nbsp; &nbsp; &nbsp; arybuf:null  
    &nbsp; &nbsp; &nbsp; }  
    });  
  You must set same value to el property and id of html tag.  
  If you already prepared arraybuffer of audio data, you can set it to data.arybuf property immediately.  
3. If you want to set or change audio data, please set arybuf propety in your app code.  
  Sample code is below.  
    player1.arybuf = your_prepared_audio_data;  
4. This project include samples of implement.  
  Please refer to AudioBufPlayerTest_use_vue.html.  
  *You no needs to read AudioBufPlayerTest_no_vue.html.  
  This code is for compare with using vue.js and without vue.js.  

# Lisense  
   OKVueComponent version 0.1.1  
   (c) 2020 OKKyu allrights reserved under MIT license.  
   
## Author  
OKKyu  
