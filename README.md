# csPortfolio
1. WebPage [here](https://brandonruth.github.io/SESshowmeyourmussels/showmeyourmusselsSES)
```html
<html>
<head>
  <link rel="icon" href="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRqxBtlRQS_MbOSvTpIWMB0KmvYsqSyL4cAUSlp1nyWY_H0VIY8">
  <title> SHOW ME YOUR MUSSELS (SES) </title>
<body bgcolor="#89cff0" alink=#006633>
  <p><center><font size=7 color=#006633> SES pod 1's Show me your Mussels Campaign <font/></center> </p> 

  <nav> 
    <font size=6 color=#006633>
      <center>
         <a href="https://brandonruth.github.io/SESshowmeyourmussels/showmeyourmusselsSES">Home</a> |
  <a href="https://brandonruth.github.io/SESshowmeyourmussels/showmeyourmusselsSES/threats">Threats</a> |
  <a href="https://brandonruth.github.io/SESshowmeyourmussels/showmeyourmusselsSES/Habitat">Habitat</a> |
  <a href="https://brandonruth.github.io/SESshowmeyourmussels/showmeyourmusselsSES/importance">Importance</a> |
  <a href="https://brandonruth.github.io/SESshowmeyourmussels/showmeyourmusselsSES/spread">Spread/reproduce</a> |
  <a href="https://brandonruth.github.io/SESshowmeyourmussels/showmeyourmusselsSES/interviews">Interviews</a> |
  <a href="https://brandonruth.github.io/SESshowmeyourmussels/showmeyourmusselsSES/economics">Economics</a>  | 
  <a href="https://brandonruth.github.io/SESshowmeyourmussels/showmeyourmusselsSES/sources">Sources</a> |
  <a href="	http://mnzoo.org/show-us-mussels-challenge/">Vote For Us<a/>
      <font/>
        
          <nav/>

        <br><img src="https://twin-cities.umn.edu/sites/twin-cities.umn.edu/files/zebra-mussels_kevin-watson_0.jpg" alt="MN zoo show me you mussels campaign" width="700" height="500">
        <img src="https://www.fws.gov/endangered/map/ESA_success_stories/MN/MN_story1/01.jpg" alt="MN zoo show me you mussels campaign" width="700" height="500">
        <center/>
  <div align=center><a href='https://www.counter12.com'><img src='https://www.counter12.com/img-A7a686D1zbwx6w75-22.gif' border='0' alt='counter'></a><script type='text/javascript' src='https://www.counter12.com/ad.js?id=A7a686D1zbwx6w75'></script></div>
      </body>
      

</head>
</html>
```
This code shows the home page of my website, the most challenging part of this website was navigating between the different tabs, which i was not aware had to in a way be entirely diffrent websites. This was not necessarily difficult but it was quite tedious.<br>
2. Lightning [here](https://brandonruth.github.io/lightning2/)
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
3. Lightning JS [here](https://brandonruth.github.io/lightning2/)
4. Dice [here](https://brandonruth.github.io/dice3/)
5. College presentation[here](https://docs.google.com/presentation/d/e/2PACX-1vSSNUgvo11X_pQfsNkG32qAnl7cZUq5_w5fK-nVq8Fr5ZdfvCIji_pSYRRGiNqIwTfOEP8zzdp0ANLy/pub?start=true&loop=true&delayms=5000)
6. Chemotaxis [here](https://brandonruth.github.io/chemotaxis4/)
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
```
7. Starfield [here](https://brandonruth.github.io/starfield5/)
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
```


