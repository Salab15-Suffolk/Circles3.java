# Circles3.java
Hank
echo # Circles3.java >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/Salab15-Suffolk/Circles3.java.git
git push -u origin master//// Wild circles #3.
String title= "Creature ";
String Name= "Hank" ;
String subtitle=  "Press any key to erase";
String author=  "Bruce Alan Martin";

// GLOBAL VARIABLES //
  
float x,y, z, a, d, e, f, g, i,j,k,l,m,n,o, p, q; 
int h,w,b,c;
// Setup:  screen size, initialization. //
void setup() {
  size(500, 500);
  x=  width/2;
  y=  height/2;
  z=x+30;
  a=y+30;
  d=x-30;
  e=y+30;
  w=  150;          // width of ellipse.
  h=  80;          // height of ellipse
  b=20;            //width of rectangle
  c=60;            //height of rectangle
  f=x-75;
  g=f-100;
  i=y;
  j=x+75;
  k=j+100;
  l=x+40;
  m=y-20;
  n=x-40;
  o=y-20;
  p=x;
  q=y-10;
  
  
  
}

// Next frame. //
void draw() {
  text (title, 10,10);
  text( Name, 230, 200);
  text( subtitle, width/2, 10 );
  text( author, 10, height-10 );
  text( w+"x"+h, width/2,height-10 );
  //
  ellipse(x, y, w, h);
  rect(z,a, b,c); 
  rect(d,e,b,c);
  line(f,y,g,i);
  line (j,y, k,i);
  ellipse (l,m, 10,10); 
  ellipse (n,o,10,10);
  ellipse (p,q,20,20);

}


//  Handle mouse clicks //
void mousePressed() {
  x=  mouseX;
  y=  mouseY;
  z=x+30;
  a=y+30;
  d=x-30;
  e=y+30;
  f=x-75;
  g=f-100;
  i=y;
  j=x+75;
  k=j+100;
  l=x+40;
  m=y-20;
  n=x-40;
  o=y-20;
  p=x;
  q=y-10;
  
  
  
 }


//  Handle keyboard //
void keyPressed() {
  // Erase everything, change size & color. //
  background(random(255), random(255), random(255) );
  fill( (255), random(255), random(255), random(255)  );
  w=  int( random(50,150) );
  h=  int( random(50,150) );
}
