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

```hmtl

``` 