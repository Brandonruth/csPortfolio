# csPortfolio
* WebPage [here]()
* Lightning [here](https://brandonruth.github.io/lightning2/)
* Lightning JS [here](https://brandonruth.github.io/lightning2/)
* Dice [here](https://brandonruth.github.io/dice3/)
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
