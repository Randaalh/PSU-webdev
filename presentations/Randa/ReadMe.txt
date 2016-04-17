<!DOCTYPE html>
<html>
<head>
<title>Image Slider</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style type="text/css">
#wrapper{
width: 650px;
height: 450px;
margin: 20px auto;
position: relative;
}

#flower{
width: 650px;
height: 450px;
position: absolute;
}


#leftA{
width: 100px;
height: 450px;
position: absolute;
left: 0px;
top: 0px;
}

#rightA{
width: 100px;
height: 450px;
position: absolute;
right: 0px;
top: 0px;
}

.left{
width: 50px;
height: 50px;
position: absolute;
top: 40%;
left: 0px;

}
.right{
width: 50px;
height: 50px;
position: absolute;
top: 40%;
right: 0px;

}


</style>
<script type="text/javascript">
<!--
var flowercount = 1;
var total = 5;

function slide(x){
var flowerpic = document.getElementById("flower");
flowercount = flowercount + x;

if (flowercount > total){ flowercount = 1; }
if (flowercount < 1) { flowercount = total; }
flowerpic.src = "img/f" + flowercount + ".jpg";
}


-->
</script> 
</head>
<body>
<div id="wrapper">

<img id="flower" src="img/f1.jpg" alt="flower">
<div id="leftA"> <img onClick="slide(-1)" class="left" src="img/left.png" alt="left arrow"> </div>
<div id="rightA"> <img onClick="slide(1)" class="right" src="img/right.png" alt="right arrow"> </div>

</div>
</body>
</html>

    
   
