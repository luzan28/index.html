# index.html
&lt;!DOCTYPE html> &lt;html lang ="en" >     &lt;head>         &lt;meta charset ="UTF-8">         &lt;title>Digital Clock&lt;/title>         &lt;link rel="stylesheet" type="text/css" href="styles/styles.css">          &lt;/head>     &lt;body>         &lt;div id="clock">07:10:35&lt;/div>         &lt;script type="text/javascript">          function showTime()          {              var time=new Date();              var hr = time.getHours();              var min =time.getMinutes();              var sec =time.getSeconds();                          if(hr==12)             {                 hr-=12;             }             if(hr==0)             {                 hr ==12;             }             hr =(hr&lt;10) ? "0"+ hr :hr;             min =(min&lt;10) ? "0" + min :min;             sec =(sec&lt;10) ? "0" + sec :sec;                           var currentTime =hr +":" + min +":"+ sec;              document.getElementById("clock").innerHTML =currentTime;               setTimeout(showTime,1000);               }               showTime();         &lt;/script>     &lt;/body> &lt;/html>
