#### chat 
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>hello</title>
    <style>
        .chat{
            width: 100%;
            height: 500px;
            background-color: aqua;
        }
    </style>
</head>
<body>
<div class="chat"></div>
<input id="message" type="text">
<button type="button" onclick="send()">send</button>
<script>
    function send() {
        let input=document.getElementById("message");
        let message =input.value
        input.value=""
        addChartMessage (message)
    }
    function  addChartMessage (message){
        let chat= document.querySelector(".chat")
        chat.innerHTML+=`<p>${message}</p>`
    }
</script>
</body>
</html>
```
