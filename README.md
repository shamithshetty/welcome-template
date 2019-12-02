# welcome-template
Company welcome template
<!DOCTYPE html>
<html>
<meta name="viewport" content="width=device-width">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular.min.js"></script>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular-animate.js"></script>
<style>

  html,body{
	  height:100%;
	   
  }
  input[type=checkbox]{
	display:none;
   }
  input[type=checkbox] ~ label {
     background-image:linear-gradient(gray,black);
     height: 50px;
	 width:50px; 
	 color:white;
     padding: 16px;
     display: block;
	 border-radius:50%;
	 border:8px solid gray;
	 box-shadow:2px 10px gray;
	 position:fixed;
	 bottom:0;
	 right:0;
	 margin-bottom:80px;
	 margin-right:80px;
	 text-align:center;
	 vertical-align:middle;
   }
   .p_style{
	 color:white;
	 border-radius:50%;
	 border:4px solid gray;
	  background-image:linear-gradient(gray,black);
     height:60px;
	 width:60px;
	 position:fixed;
	 bottom:0;
	 right:0;
	 margin-bottom:190px;
	 margin-right:93px;
	  vertical-align:middle;
	 text-align:center;
	 padding-top:15px;
   }
   .e_style{
	 color:white;
	 border-radius:50%;
	 border:4px solid gray;
	 background-image:linear-gradient(gray,black);
     height:60px;
	 width:60px;
	 position:fixed;
	 bottom:0;
	 right:0;
	 margin-bottom:280px;
	 margin-right:93px; 
	 vertical-align:middle;
	 text-align:center;
	 padding-top:15px;
   }
   @keyframes myChange {
        from {
           height:60px;
	       width:60px;
         } to {
	        margin-bottom:170px;
            margin-right:122px;
            width: 0px;
	        height:0px;
            }
   }
   .p_style.ng-hide {
  animation: 2s myChange;
   .e_style.ng-hide {
  animation: 2s myChange;
   }
</style>
<body ng-app="ngAnimate">
<div class="main" ng-app="">
  <input type="checkbox" ng-init='myCheck=true' id="toggle" name="toggle" ng-model="myCheck" >
  <label for="toggle"><center><i class="fa fa-snowflake-o" style='font-size:36px;opacity:1'></i></center>
  </label>
  <div class="p_style" data-tooltip="9008809863" ng-hide="myCheck"><center><i ng-hide="myCheck" class="fa fa-phone" style="'font-size:26px;opacity:0.9;'"> </i></center></div>
  <div class="e_style" data-tooltip="shamithniz@gmail.com" ng-hide="myCheck"><center><i ng-hide="myCheck" class="fa fa-envelope" style='font-size:26px;opacity:0.9;'> </i></center></div>
</div>
</body>
</html>
