## Vue.js Learning

from [Vue JS 2.0 - Mastering Web Apps](https://www.udemy.com/vue-web-apps/learn/v4/)

### Chapter - 01 - Vue Instance

```html
<body>
  <div class="" id="app">
    <h1>Text : {{ text }}</h1>
  </div>
  <script type="text/javascript">
    var app = new Vue({
      el: '#app',
      data: {
        text: 'Hello, World'
      }
    });
  </script>
</body>
```

### Chapter - 02 - Vue Directive

```html
<body>
  <div class="" id="app">
    <div v-bind:title="randNum" 
    v-if="shown" 
    >Hover over me for your random number</div>
  </div>
  <script type="text/javascript">
    var app = new Vue({
      el: '#app',
      data: {
        randNum: Math.floor(Math.random() * 50) + 1,
        shown: false
      }
    });
  </script>
</body>
```

### Chapter - 03 - V-for for List Rendering

```html
<body>
  <div class="" id="app">
    <ul>
      <li v-for="color in xcolors" v-if="color.primary">
        {{ color.text }}
      </li>
    </ul>
  </div>
  <script type="text/javascript">
    var app = new Vue({
      el: '#app',
      data: {
        colors: ['red', 'green', 'blue', 'yellow', 'orange'],
        xcolors: [{
            text: 'red',
            primary: false
          },
          {
            text: 'green',
            primary: true
          },
          {
            text: 'blue',
            primary: false
          },
          {
            text: 'yellow',
            primary: true
          },
          {
            text: 'orange',
            primary: true
          }
        ]
      }
    });
  </script>
</body>
``` 

### Chapter - 04 - V-on for clicking

```html
<body>
  <div class="" id="app">
    <!-- <button class="vue-btn" v-on:click="reveal">Reveal the Secret Number</button> -->
    <button class="vue-btn" @click="reveal">Reveal the Secret Number</button>
  </div>
  <script type="text/javascript">
    var app = new Vue({
      el: '#app',
      data: {
        secretNumber: Math.floor(Math.random() * 100) + 1
      },
      methods: {
        reveal() {
          alert(`Here's the secret number: ${this.secretNumber}`)
        }
      }
    });
  </script>
</body>
```