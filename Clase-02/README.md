# Clase 02  

## Apuntes de clase 

  - Conversar sobre obras de galería UNIACC

   ### En  processing 
    
```int tamano = 50;

int t1 = 10;
int t2 = 40;
int t3 = 15;

void setup() {
  size(300, 300);
  //forzar que los fps vayan a 30
  frameRate(30);
}

void draw() {
  background(0);
  
  if (frameCount < 30){
    tamano = t1;
  } 
  
  if (frameCount > 30){
    tamano = t2;
  }
  
  if (frameCount > 60){
    tamano = t3;
  }
  
  //tamano = frameCount;
  
  println(frameCount);
  fill(220,220,100);
  circle(150,150,tamano);
}



