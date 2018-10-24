# csPortfolio
* WebPage [here]()
* Lightning [here](https://brandonruth.github.io/lightning2/)
* Lightning JS [here](https://brandonruth.github.io/lightning2/)
* Dice [here](https://brandonruth.github.io/dice3/)
* College presentation[here](https://docs.google.com/presentation/d/e/2PACX-1vSSNUgvo11X_pQfsNkG32qAnl7cZUq5_w5fK-nVq8Fr5ZdfvCIji_pSYRRGiNqIwTfOEP8zzdp0ANLy/pub?start=true&loop=true&delayms=5000)
*Chemotaxis [here](https://brandonruth.github.io/chemotaxis4/)
```Java
   void change(){
     if(mouseX >xpos){
       xpos-=(int)(Math.random()*3);
     }
     else if(mouseX <xpos){
      xpos+=(int)(Math.random()*3); 
     }
     if(mouseY >ypos){
       ypos-=(int)(Math.random()*3);
     }
     else if(mouseY <ypos){
      ypos+=(int)(Math.random()*3); 
     }
     if(xpos<=size/2){
      xpos=xpos+5; 
     }
     if(xpos>=1500-size/2){
      xpos=xpos-5; 
     }
     if(ypos<=size/2){
      ypos=ypos+5;
     }
     if(ypos>=950-size/2){
      ypos=ypos-5; 
     }
if(mouseX<xpos&&mouseX>xpos-size/2&&mouseY>ypos&&mouseY<ypos+size/2){
      size=size+1;
    }
    if(mouseX>xpos&&mouseX<xpos+size/2&&mouseY>ypos&&mouseY<ypos+size/2){
      size = size+1;
   }
   if(mouseX>xpos&&mouseX<xpos+size/2&&mouseY<ypos&&mouseY>ypos-size/2){
      size=size+1;
    }
    if(mouseX<xpos&&mouseX>xpos-size/2&&mouseY<ypos&&mouseY>ypos-size/2){
      size = size+1;
   }
   if(size==500){
     explosionx=xpos;
     explosiony=ypos;
    size=0;
    image(explosion,explosionx,explosiony,500,500);
   }
 }  
```Java
void draw()
{
   background(125, 25, 25);
  int xpos = 10;
  int ypos = -45;
  for (int t = 0; t < 15; t++) {
    ypos = ypos + 55;
    xpos= 10;
    for (int i= 0; i < 18; i++) {
      fill(255, 255, 255);
      rect(xpos, ypos, 50, 50,15);
      die = new Die(xpos, ypos);
      die.roll();
      xpos += 55;

    }
    
  }
   stats();
   
}
void stats(){
  textSize(100);
   text("Total: "+total,260,900);
  
}

```Java
int startX=0;
int startY=150;
int endX=0;
int endY=150;

void setup()
{
strokeWeight(3);
background(0, 0, 0);
size(300,300);
}

void draw()
{
stroke((int)(Math.random()*255),(int)(Math.random()*255),(int)(Math.random()*255));

while(endX<301){

endX = startX + (int)(Math.random() * 10) + 0;
endY = startY + (int)(Math.random()*19)+ -9;

line(startX,startY,endX,endY);
startX=endX;
startY=endY;
}
}

void mousePressed()
{
startX=0;
startY=150;
endX=0;
endY=150;

}
```
