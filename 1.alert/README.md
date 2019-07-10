
  <!DOCTYPE html>
  <html lang="en">
  <head>
      <meta charset="UTF-8">
      <title>事件监听</title>
  </head>
  <body>
  
  <ul id="no">
      <li>1</li>
      <li>2</li>
      <li>3</li>
      <li>4</li>
      <li>5</li>
      <li>6</li>
      <li>7</li>
  </ul>
  
  <script>
     // write your code here 
     ocument.addEventListener('DOMContentLoaded', function() {
             let app = document.getElementById('no');
             // 事件侦听器绑定到整个容器上
             app.addEventListener('click', function(e) {
                 if(e.target && e.target.nodeName === 'LI') {
                     let item = e.target;
                     alert( item.innerHTML);
                 }
             });
         });
  </script>
  </body>
  </html>

