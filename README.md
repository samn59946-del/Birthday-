<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Birthday-flyer</title>

    <style>
        body{
            margin: 0;
            padding: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Times New Roman', Times, serif;
            background: radial-gradient(circle at top, #0a0f2c, #02030a)     
           }

           /* main card */
           .flyer{
            width: 360px;
            height: 620px;
            border-radius: 25px;
            position: relative;
            overflow: hidden;
            background: linear-gradient(145deg, #0a0f2c, #111433);
            box-shadow: 0 20px 60px rgba(0,0,0,0.8);
           }

           /* glow lights */ 
           .flyer::before{
            content: '';
            position: absolute;
            width: 300px;
            height: 300px;
            background: radial-gradient(circle, rgba(0, 140, 255, 0.4), transparent);
            top: -100px;
            left: -100px;
            filter: blur(50px);
           }

           .flyer::after{
            content: '';
            position: absolute;
            width: 300px;
            height: 300px;
            background: radial-gradient(circle, rgba(255, 0, 150, 0.4), transparent);
            bottom: -100px;
            right: -100px;
            filter: blur(50px);
           }

           /* text */
           .content{
            position: absolute;
            top: 60px;
            left: 25px;
            color: #fff;
            z-index: 2;
           }

           .content h1{
            font-size: 34px;
            line-height: 1.1;
            margin: 0;
            text-shadow: 0 5px 20px rgba(0,0,0,0.5)

           }

           /* name */
           .name{
            margin-top:20px ;
            padding: 10px 15px;
            background: linear-gradient(90deg, #ff0099, #00d4ff);
            border-radius: 10px;
            font-weight: 700;
            display: inline-block;

           }

           .date{
            margin-top: 15px;
            margin-left: 10px;
            padding: 10px 15px;
            background: #111;
            border-radius: 10px;
            display: inline-block;
           }

           .image{
            position: absolute;
            bottom: 0;
            right: 0;
            width: 70%;
            z-index: 2;
           }

           .image img{
            width: 100%;
            filter: drop-shadow(0 20px 30px rgba(0,0,0,0.9));
           }

           .circle{
            position: absolute;
            right: 40px;
            top: 140px;
            width: 220px;
            height: 220px;
            border-radius: 50%;
            background: linear-gradient(circle, #00d4ff, #090979);
            filter: blur(40px);
            opacity: 0.7;
           }

           .particles{
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: radial-gradient(white 1px, transparent 1px);
            background-size: 25px 25px;
            opacity: 0.05;
           }

           button{
            margin-top: 20px;
            padding: 10px 18px;
            border: none;
            border-radius: 20px;
            background: linear-gradient(90deg, #ff0099, #00d4ff);
            color: #fff;
            cursor: pointer;
            box-shadow: 0 0 15 rgba(255,0,150,0.6);
           }

           @keyframes pulse {
            0%{transform: scale(1);}
            100%{transform: scale(1.05);}
           }

           .name{
            animation: pulse 2s infinite alternate;
           }
    </style>


</head>
<body>
    <div class="flyer">
         <div class="particles"></div>

         <div class="content">
            <h1>HAPPY<br>BIRTHDAY 🎉</h1>

            <div class="name">Suru Bolaji</div>
            <div class="date">15th April</div>

            <br>
            <button onclick="celebrate()">Tap🎁</button>
         </div>

         <div class="circle"></div>

         
         <div class="image">
            <img src="bolaji (1) png.png" alt="Birthday celebrant">
         </div>
    </div>

    <script>
        function celebrate() {
            document.body.style.background =
            "radial-gradient(circle, #ff0099, #0a0f2c)";

            alert("Happy Birthday Suru Bolaji 🎉🔥 More life, more wins")
        }
    </script>

    

    
    
</body>
</html>
