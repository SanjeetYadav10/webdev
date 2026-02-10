<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex Playground</title>

    <style>
        body {
            text-align: right align;
        }

        div {
            height: 100px;
            width: 100px;
            display: inline-block;
            border: 2px solid black;
        }

        #container {
            width: 800px;
            height: 200px;
            display: flex;
            flex-direction: column;
            justify-content: space-around;
            transition: all 1s steps(5) 0.1s;
        }

        #box1 {
            background-color: blue;
            transform: rotate(30deg);
        }

        #box2 {
            background-color: red;
            transform: rotate(30deg);
        }

        #box3 {
            background-color: aquamarine;
            transform: rotate(45deg);
        }

        #box4 {
            background-color: brown;
        }

        #box5 {
            background-color: blueviolet;
        }

        #sq {
            height: 125px;
            width: 125px;
            background-color: pink;
            margin: 25px auto;
        }

        @media (max-width: 400px) {
            #sq {
                background-color: brown;
            }
        }

        div:hover {
            background-color: red;
            color: aliceblue;
            transform: skew(30deg) translate(50px);
        }

        @keyframes colorAnimate {
            from { background-color: red; }
            to { background-color: blue; }
        }

        .loader {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border: 5px solid black;
            border-top: 10px solid blue;
            margin: 30px auto;
            animation: spinanimate 1s steps(20) infinite;
        }

        @keyframes spinanimate {
            from {
                transform: rotate(0deg);
            }
            to {
                transform: rotate(360deg);
            }
        }
    </style>
</head>

<body>

    <h1>Flex Playground</h1>

    <div id="container">
        <div id="box1">box1</div>
        <div id="box2">box2</div>
        <div id="box3">box3</div>
        <div id="box4">box4</div>
        <div id="box5">box5</div>
    </div>

    <div id="sq"></div>

    <div class="loader"></div>

</body>
</html>
