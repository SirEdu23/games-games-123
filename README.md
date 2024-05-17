let gravityY = 12
let circleY = 0
let squareY = 0

function setup() {
  createCanvas(400, 400)
}

function draw() {
  background(220, 10, 33)
  
  fill(0, 0, 200);
  circle(250, circleY, 100)
  
  fill(0, 0, 250);
  square(150, squareY, 100)
  
  circleY += gravityY;
  squareY += gravityY;
  
  
  if (circleY > height - 50) {
    circleY = height - 50
  }
  
  if (squareY > height - 100) {
    squareY = height - 100
  }
}
