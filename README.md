# the EARTH and the SUN
# circular-orbit
<html>
    <head>
<style>
    #sun{
        position:absolute;
        top:150px;
        left:150px;
        height:50px;
        width:50px;
        border-radius:50%;
        background-color:darkorange;

    }
    #orbit{
        position:absolute;
        top:50px;
        left:50px;
        height:250px;
        width:250px;
        border-radius:50%;
        border:1px solid white;
    }
    #earth{
        position:absolute;
        top:45px;
        left:170px;
        height:10px;
        width:10;
        border-radius:50%;
        background-color:darkgreen;
    }

    body{
         background-color:black;   
    }
</style>
    </head>
    <body>
        <div id="sun"></div>
        <div id="orbit"></div>
        <div id="earth"></div>


        <script>
            var earth=document.getElementById("earth");
            var a = 0;
            setInterval(function myFunc()
            {
                earth.style.top=(170-Math.cos(a)*125);
                earth.style.left=(170+Math.sin(a)*125);
                a = a + (1/360);
        
        
            },10)
        </script>
    </body>
</html>
