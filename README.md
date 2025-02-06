# Happy-Birthday
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Yellow Flower Petals</title>
    <style>
        /* Set the body to have a full-screen background color */
        body {
            margin: 0;
            height: 100vh;
            background-color: #fff7e6; /* Light background color */
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            position: relative;
        }

        /* Petal container to center the petals */
        .petal {
            position: absolute;
            width: 30px;
            height: 30px;
            background-color: #ffcc00; /* Yellow petal */
            clip-path: polygon(50% 0%, 0% 100%, 100% 100%); /* Shape of petal */
            animation: float 6s ease-in-out infinite, rotate 10s linear infinite;
        }

        /* Create multiple petals with different positions and timings */
        .petal:nth-child(1) { animation-delay: 0s; top: 50%; left: 20%; }
        .petal:nth-child(2) { animation-delay: 1s; top: 30%; left: 40%; }
        .petal:nth-child(3) { animation-delay: 2s; top: 70%; left: 30%; }
        .petal:nth-child(4) { animation-delay: 3s; top: 80%; left: 60%; }
        .petal:nth-child(5) { animation-delay: 4s; top: 20%; left: 80%; }
        .petal:nth-child(6) { animation-delay: 5s; top: 60%; left: 50%; }

        /* Animations for floating and rotating petals */
        @keyframes float {
            0% {
                transform: translate(0, 0) rotate(0);
            }
            100% {
                transform: translate(50px, -50px) rotate(360deg);
            }
        }

        @keyframes rotate {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
    </style>
</head>
<body>
    <!-- Petals will be created using divs -->
    <div class="petal"></div>
    <div class="petal"></div>
    <div class="petal"></div>
    <div class="petal"></div>
    <div class="petal"></div>
    <div class="petal"></div>

</body>
</html>
