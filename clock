function setup() {
	createCanvas(500, 450);
	background(255, 255, 255)
	noStroke(); 
}

//donut is hour 
//coffee content is minutes 
//steam is seconds 

function draw() {
	var h = hour();
	var m = minute(); 
	var s = second(); 
	
	stroke(255); 
	//outside of donut 
	fill (305, 100, 75, 5) 
	ellipse(150, 300, 200)
	let donutfill = map(h, 0, 24, 0, TWO_PI);
	
	stroke(225); 
	fill(255, 255, 255)
	arc(150, 300, 200, 200, 0, donutfill)
	
	stroke(155); 
	//inside of donut 
	fill(255, 255, 255)
	ellipse(150, 300, 100)

	stroke(255); 
	//coffee cup 
	if (m%2==0){
		fill(130, 53, 20, 0.92) }
	else {
		fill(325,200,5,1)}

	quad(270, 150, 300, 400, 440, 400, 470, 150); 
	let coffeefill = map(m, 0, 60, 0, 250); 
	
	stroke(255); 
	fill (255, 255, 255); 
	quad(270, 400-coffeefill, 470, 400-coffeefill, 470, 150, 270, 150)
	
	//seconds
	stroke(150); 
	strokeWeight(1); 
	triangle(30, 25, 230, 225, map(s, 0, 60, 0, 100), 125); 
	fill(0,0,255,150)
	
	
}
