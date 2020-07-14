# -dom-
练习过程中写出来的，可以生成很多个li方块！！
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        li {
            width: 100px;
            height: 100px;
            background-color:  skyblue;
            margin: 100px auto;
            float: left;
        }
    </style>
</head>
<body>
    <input type="text" name="" id="in1">
    <button id="btn1"></button>
    <ol>
        <li></li>
    </ol>
</body>
    <script>

        var btn1 = document.getElementById('btn1');
        btn1.addEventListener('click', function() {
        var in1 = document.getElementById('in1').value;
        var ol = document.querySelector('ol');
            for(i = 0; i < in1; i++) {
                var li = document.createElement('li');
                ol.appendChild(li);
            }
        })
    </script>
</html>
