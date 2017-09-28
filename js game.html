<!DOCTYPE html>
<html lang="en">

<head>
<title>Target Practice</title>
<meta content="text/html;charset=utf-8" http-equiv="Content-Type">
<meta content="utf-8" http-equiv="encoding">
</head>
<body>
<canvas id="gameCanvas" width="800" height="600"></canvas>

<script>
    var crossHairX = 400; 
	var crossHairY = 300;
	var score = 0;
	var timer = 25;
	var ammunition = 30;
	var targetSize = 8+Math.random()*10;
	var mouseIsDown = false;
	var target = [];
	const TARGET_COUNT = 4;
	
   function calculateMousePos(evt) { 
    var rect = canvas.getBoundingClientRect(), root = document.documentElement; 

    var mouseX = evt.clientX - rect.left - root.scrollLeft; 
    var mouseY = evt.clientY - rect.top - root.scrollTop; 
    return { 
      x: mouseX, 
      y: mouseY 
    }; 
  } 
  
    function handleMouseClick(evt) {
	  mouseIsDown = true;
		ammunition -= 1;
	  // Mouse button down for short interval prevents hold down spray fire
		setInterval(function() {
		mouseIsDown = false;
	}, 1000/1);
	}	  

	function handleMouseUnclick(evt) {
		mouseIsDown = false;	
	  }
    
	
	function createTargets(){		// creates array elements
		for(var i=0; i < TARGET_COUNT; i++){
			target.push(new targetClass());
		}
	}

	
   window.onload = function() {		// starts here
    canvas = document.getElementById('gameCanvas');
    canvasContext = canvas.getContext('2d');

    // move and draw 30 times per second.
    var framesPerSecond = 30;
    setInterval(function() {
        moveEverything();
        drawEverything();
      }, 1000/framesPerSecond);
      
	canvas.addEventListener('mousedown', handleMouseClick);  
	canvas.addEventListener('mouseup', handleMouseUnclick);  
	  
    canvas.addEventListener('mousemove', function(evt) {  
        var mousePos = calculateMousePos(evt);
		
		crossHairX = mousePos.x; // mouse position		
        crossHairY = mousePos.y; // mouse position
      } ); 
	  
	// create a countdown timer  
   	var framesPerSecondForTimer = 1;
    setInterval(function() {
		timer--;
	}, 1000/framesPerSecondForTimer);
	  
	createTargets();	  // funtion to create the initial target objects, instances
  }
    
	
	function targetClass() {			// A class or object for creating targets: location, speed, size
		this.targetX = 10;
		this.targetY = 50+Math.random() * (canvas.height-100);
		this.radius = 5 + Math.random() * 25;
		this.targetSpeed = 3 + Math.random() * 2;
		this.targetMove = function(){	// A function within a class is called a method
		
			var dx = this.targetX - crossHairX; 
			var dy = this.targetY - crossHairY;
			var dist = Math.round(Math.sqrt(dx*dx + dy*dy));   // a named value in a class is a property
	  
			if(dist < (this.radius) && mouseIsDown && ammunition > (-1)){	// if mouse click is at a target
				this.targetX = 10;				// reset target x, y location and radius
				this.targetY = 50+Math.random() * (canvas.height-100);
				this.radius = 5 + Math.random() * 25;
				score++;
				console.log ("Target hit! "+score+" Ammo " +ammunition+ " " +dist);
				mouseIsDown = false;
			}else if(dist > (this.radius) && mouseIsDown ){

				console.log ("Target missed! "+score+" Ammo " +ammunition+ " " +dist+ " " + this.radius);
			}
		this.targetX += this.targetSpeed;
		}
		
		this.targetDraw = function(){
			colorCircle(this.targetX, this.targetY, this.radius, 'green');
		
		}
	}
	
	
  
   function moveEverything() {
		for(var i=0; i < TARGET_COUNT; i++){	//TARGET_COUNT is the same as target.length
			target[i].targetMove();
		}
	
   }
    function colorRect(topLeftX, topLeftY, boxWidth, boxHeight, fillColor) {
    canvasContext.fillStyle = fillColor;
    canvasContext.fillRect(topLeftX, topLeftY, boxWidth, boxHeight); 
    }
  
   function colorCircle(centerX, centerY, radius, fillColor) {
    canvasContext.fillStyle = fillColor;
    canvasContext.beginPath();
    canvasContext.arc(centerX, centerY, radius, 0, Math.PI*2, true);
    canvasContext.fill();
   }
  function drawEverything() {
		colorRect(0, 0, canvas.width, canvas.height, 'black');  // clear the game view by filling it with black
  
		// colorCircle(crossHairX, crossHairY, 2, 'white');  //create a crosshair for the pointer
	
		for(var i =0; i < TARGET_COUNT; i++){
			target[i].targetDraw();		// same as target[1].targetDraw() 
		}
		
		canvasContext.fillStyle="red";
		canvasContext.font="20px Arial";
		canvasContext.fillText("Score " + score, 200, 30);
		if(ammunition > (0)){
			canvasContext.fillText("Ammo " + ammunition, 500, 30);
		}else if(ammunition <= (0)){
			canvasContext.fillText("Out of Ammo!", 500, 30);
		}
  }
</script>

</body>
</html>

   <footer>
		 <h2>Welcome to Target Practice. Test your agility and coordination. </h2>
		 <h2>Use your mouse to shoot the targets and score points.  Updates forthcoming.</h2>
		 <h2>Developed by Pete Fralick. <a href="http://www.pfwebdev.com/index.php/games/" >Return to PF Web Dev.com</a></h2>
