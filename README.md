# csPortfolio
* WebPage [here]()
* Lightning [here]()
* Lightning JS [here]()
* Dice [here]()

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
