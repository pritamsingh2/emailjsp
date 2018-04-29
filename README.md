<!DOCTYPE html>
<html lang="en">
<head>
  <title>Login Form</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
<style type="text/css">
    p.detail { color:"black";font-weight:bolder;font-family:sans-serif;font-size:x-large; }
     span.detail2 { color:"black";font-weight:bold;font-family:sans-serif;font-size:small; }
    span.name {font-weight:lighter;font-family:Tahoma;font-size:medium; }
   body {background-color:lightgray;height: 100%;}
    </style>
	</head>
	<script type="text/javascript">
	function validateEmail(email) {
  var re = /^(([^<>()[\]\\.,;:\s@\"]+(\.[^<>()[\]\\.,;:\s@\"]+)*)|(\".+\"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
  return re.test(email);
}

function validate() {
  var $result = $("#result");
  var email = $("#email").val();
  $result.text("");

  if (validateEmail(email)) {
    $result.text(email + " is valid ");
    $result.css("color", "green");
  } else {
    $result.text("Please enter valid email ID(example:***@***.com)");
    $result.css("color", "red");
  }
  return false;
}

$("#validate").bind("click", validate);
	</script>
	

<body oninput="validate()">
<div class="container-fluid">


<div class="col-sm-12">
<p class="detail">Login <span class="detail2">or</span>  <span class="name" ><a href="" style="text-decoration: underline;">Register a new Account</a></span></p>





 <br> 
 <br> 
 <br> 
<div class="col-sm-4">
 <p><b><h3> Forgot password?</h3></b></p>
 
<br>
<br>
<form>
<p><h4> Email ID*</h4></p>
<input  id='email' placeholder="***@***.com"/>

<h3 id='result'></h3>
</form>


<br>
<br>
<br>

<button type="button" ; style="background-color: lightblue" >Email Password </button>
 </div>
 <div class="col-sm-4">
 <div style=" border-left: 1px solid black; height: 520px; width:5%; margin-left:50%; text-align: center; position: absolute;">
 <span style="left: -10px; top:160px; position: relative; background-color: white;">
 OR
 </span>
 </div>
 </div>
<div class="col-sm-4">
	<p><b><h3>Have a Facebook Account?</h3></b></p>
	 </br>
	 </br>
	 </br>
	<button type="button" class="btn btn-primary"><span class="badge"><b>f</b></span> Login with Facebook</button>
    </div> </div>

</div>
</body>
</html>
