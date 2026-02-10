<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Tool parts</title>

    <style>
        body {
            text-align: right align;
        }

        div {
            height: 100px;
            width: 100px;
            display: inline-block;
            border: 3px solid black;
        }

        #container {
            width: 800px;
            height: 200px;
            display: flex;
            flex-direction: column;
            justify-content: space-around;
            transition: all 1s steps(5) 1s;
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
            color: blue;
            transform: skew(30deg) translate(50px);
            animation-play-state: paused;
}

        }
        


        @keyframes colorAnimate {
            from { background-color: white; }
            to { background-color: grey; }
        }

        .loader {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border: 5px solid black;
            border-top: 10px solid blue;
            margin: 25px auto;
            animation: spinanimate 1s steps(20) infinite;
        }
@keyframes pulseColor {
    0% {
        background-color: currentColor;
    }
    50% {
        opacity: 0.6;
    }
    100% {
        opacity: 1;
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
