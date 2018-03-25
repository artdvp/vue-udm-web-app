## Vue.js Learning

from [Vue JS 2.0 - Mastering Web Apps](https://www.udemy.com/vue-web-apps/learn/v4/)

# Chap - 01 - Vue Instance

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
