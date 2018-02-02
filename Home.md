Welcome to the Weight-Converter-APP wiki!


`<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.6/css/bootstrap.min.css" integrity="sha384-rwoIResjU2yc3z8GV/NPeZWAv56rSmLldC3R/AZzGRnGxQQKnKkoFVhFQhNUwEyJ" crossorigin="anonymous">
    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"></script>
<!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">

<!-- jQuery library -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>

<!-- Latest compiled JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
    <title>Hello, world!</title>
  </head>
    <style>
        body
        {
            margin-top:70px;
            background:#333;
            color: #fff;
        }
    </style>
    
  <body>
    <div class="container">
        <div class="row">
            <div class="col-md-6 offset-md-3">
      <h1 class="display-4 text-center">Weight Converter</h1>
            
            
      <form>

      <div class="form-group">
          <input type="number"
            id ="lbsInput"     
                 class="form-control form-control-lg"
                 placeholder="Enter pounds...">
          </div>
          </form>
      
      <div id="output">
      <div class="card btn-primary mb-2">
          <div class="card-block">
          <h4>Grams:</h4>
              <div id="gramsOuput"></div>
          </div>
          </div>
      
      
      
    
      <div class="card btn-success  mb-2">
          <div class="card-block">
          <h4>Ounces:</h4>
              <div id="ozOuput"></div>
          </div>
          </div>
  

      
      <div class="card btn-danger mb-2">
          <div class="card-block">
          <h4>Kilograms:</h4>
              <div id="kgOuput"></div>
          </div>
          </div>
          </div>
      


      </div>
</div>
    </div>
     
      <script type="text/javascript">
      document.getElementById('output').style.visibility = ' hidden';
      document.getElementById('lbsInput').addEventListener('input', 
    		  function(e){
    	  document.getElementById('output').style.visibility = ' visible';
    	let lbs = e.target.value;
    	 document.getElementById('gramsOuput').innerHTML= lbs / 0.0022046;
    	 document.getElementById('kgOuput').innerHTML= lbs / 2.2046;
    	 document.getElementById('ozOuput').innerHTML= lbs / lbs *16;
      });
      </script>
      
    <!-- Optional JavaScript -->
      
  
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
    
  </body>
</html>`