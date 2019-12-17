<!DOCTYPE html>
<html>
    <head>
        <title>Ivan Lein's HomePage</title>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css">
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>
        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js"></script>
    </head>
    <body>
        <div class="jumbotron text-center">
            <h1 id = "header">Hi! Welecome to Ivan's HomePage</h1>
            <p id = 'myDream'>Fight for freedom, Stand With HONG KONG!</p>
        </div>
        <div class = "container">
            <div class = "row">
                <div class="col-sm-4">
                    <h3>About Me</h3>
                    <p>My name is Ivan - Lein Chun Hang</p>
                    <p>I am studying Computer Science at <a href="https://www.cs.cityu.edu.hk/">CityU</a></p>
                </div>
                <div class="col-sm-4">
                    <h3>My wish</h3>
                    <p>Although you may not be interested</p>
                    <p>But I still want to tell you my wish!!!</p>
                    <p id="wish"></p>
                    <button onclick='showMywish()' id ='viewwish'>Click to see my wish</button>
                </div>
                <div class="col-sm-4">
                        <h3>My Programming achievement/product</h3>
                        <p>I mastered website design language(HTML/CSS/JAVASCRIPT) and their framework(REACT/BOOTSTRAP)</p>
                        <p>You can find some of my product in GItHub!</p>
                        <a href="https://github.com/ivanlein1998"><img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" height="60" width="60"></a>
                </div>
            </div>
        </div>
        
    <script>
        var clickedwish = false
        function showMywish(){
            var wish = document.getElementById("wish")
            if (clickedwish == false){             
                wish.innerHTML = "<h5>The night is darkest just before the dawn. And I promise you, the dawn is coming.</h5><img src=\"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRM12ByvPyZxD8UirqOEFBT37D0HYXu-3AN1ePfiZbdmGNjUfLyGw&s\" height=\"250\" width=\"350\">"
                document.getElementById("viewwish").innerHTML = "Click to collapse"
                clickedwish = true
            }
            else{
                wish.innerHTML = ""
                document.getElementById("viewwish").innerHTML = "Click to see my wish"
                clickedwish = false
            }
        }
    </script>
    </body>
</html>
