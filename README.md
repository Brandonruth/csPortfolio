 # Brandons ACS Portfolio
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
Lightning was a fairly easy lab, the randomization was a little difficult to understand at first but with some practice I managed to understand it.<br>
3. Lightning JS [here](https://brandonruth.github.io/lightning2/)
4. Dice [here](https://brandonruth.github.io/dice3/)
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
The most difficult part of the dice lab was getting arrays to cooperate, as I had forgotten how to begin them, a fellow classmate helped me create the array and it was quite easy from that point on.<br>
5. College presentation[here](https://docs.google.com/presentation/d/e/2PACX-1vSSNUgvo11X_pQfsNkG32qAnl7cZUq5_w5fK-nVq8Fr5ZdfvCIji_pSYRRGiNqIwTfOEP8zzdp0ANLy/pub?start=true&loop=true&delayms=5000)
6. Chemotaxis [here](https://brandonruth.github.io/chemotaxis4/)
```java
if(mouseX<xpos&&mouseX>xpos-size/2&&mouseY>ypos&&mouseY<ypos+size/2){
      size=size+1;
      scolor-=1;
    }
    if(mouseX>xpos&&mouseX<xpos+size/2&&mouseY>ypos&&mouseY<ypos+size/2){
      size = size+1;
      scolor-=1;
   }
   if(mouseX>xpos&&mouseX<xpos+size/2&&mouseY<ypos&&mouseY>ypos-size/2){
      size=size+1;
       scolor-=1;
    }
    if(mouseX<xpos&&mouseX>xpos-size/2&&mouseY<ypos&&mouseY>ypos-size/2){
      size = size+1;
       scolor-=1;
   }
   if(size==250){
     explosionx=xpos;
     explosiony=ypos;
    size=0;
    
   }
   ```
   The most difficult part of chemotaxis was getting the program to recognize that the mouse was over the given dot, this just took a lot of trial and error to solve.<br>
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
The most difficult part of this code was the intial design, as I was unable to create something I was happy with, until i took inspiration from a classmate and expanded upon it.<br>

8. Christmas card Alpha [here]("https://ryggj.github.io/ChristmasCard/")<br>
```java
class snowpile
{
  int snowy=600;
  int x1= -25;
  int y1=150;
  int x2= width+50;
  int y2= 150;
  void show(){
   fill(255);
   rect(0,snowy,width,200);
  }
  void daynight(){
   if(x1<width/2){
    fill(255,255,0);
   ellipse(x1,y1,50,50);
   x1+=5;
   y1-=1;
   snowy+=1;
   r+=1;
   g+=1;
   b+=1;
   }
   else if(x1>=width/2&&x1<width){
     fill(255,255,0);
   ellipse(x1,y1,50,50);
   x1+=5;
   y1+=1;
   snowy+=1;
   r-=2;
   g-=1;
   b-=1;
   }
   else if(x1>=width&&x1<width+20){
     x2=-25;
     x1=width+40;
     y2=150;
   }
      if(x2<width/2){
    fill(254, 252, 215);
   ellipse(x2,y2,50,50);
   x2+=5;
   y2-=1;
   snowy-=1;
   r-=1;
   g-=1;
   b-=1;
   }
   else if(x2>=width/2&&x2<width){
     fill(254, 252, 215);
   ellipse(x2,y2,50,50);
   x2+=5;
   y2+=1;
   snowy-=1;
   r+=1;
   g+=1;
   b+=1;
   }
   else if(x2>=width&&x2<width+20){
     x1=-25;
     x2=width+40;
     y1=150;
   }
   noFill();
   stroke(0);
   ellipse(500,900,1700,1700);
  }
  
}
```
9. Word counter [here]("https://github.com/Brandonruth/wordcounter")<br>
```java
StringParser strp = new StringParser();
String vowels = "aeiou";
String text = "It is not the critic who counts, not the man who points out how the strong man stumbles, or where the doer of deeds could have done them better. The credit belongs to the man who is actually in the arena, whose face is marred by dust and sweat and blood; who strives valiantly; who errs, who comes short again and again, because there is no effort without error and shortcoming; but who does actually strive to do the deeds; who knows great enthusiasms, the great devotions; who spends himself in a worthy cause; who at the best knows in the end the triumph of high achievement, and who at the worst, if he fails, at least fails while daring greatly, so that his place shall never be with those cold and timid souls who neither know victory nor defeat." ;
String str[] = text.split("[//, \\/|@]");
String stre[] = text.split("[.!?]");
void setup() {
  println("This text contains "+strp.countWords()+ " words");
  println("This text contains "+strp.countVowels()+ " vowels");
  println("This text contains "+strp.countSyllables()+ " Syllables");
  println("This text contains "+strp.countSentences()+ " Sentences");
  
}

public class StringParser {

  public StringParser() {
  }
  /**
   *countWords();
   * A "word" is defined as a contiguous string of alphabetic characters
   * i.e. any upper or lower case characters a-z or A-Z.  This method completely 
   * ignores numbers when you count words, and assumes that the document/paragraph does not have 
   * any strings that combine numbers and letters. 
   */

  public int countWords() {
    int wordcount = 0;
for( String a : str){
  wordcount ++;
}







    return wordcount;
  }

  public int countVowels() {
    int vowelcount=0;
for(int i = 0; i < text.length(); i++){
  if(text.charAt(i)=='a'||text.charAt(i)=='a'||text.charAt(i)=='e'||text.charAt(i)=='i'||text.charAt(i)=='o'||text.charAt(i)=='u'||text.charAt(i)=='y')
vowelcount++;
}







    return vowelcount;
  }
  /**
  
   *       Each contiguous sequence of one or more vowels is a syllable, 
   *       with the following exception: a lone "e" at the end of a word 
   *       is not considered a syllable unless the word has no other syllables. 
   *       You should consider y a vowel.
   */

  public int countSyllables() {
   int syllablecount = 0;
    for(int i = 0; i < text.length(); i++){
 if(text.charAt(i)=='a'||text.charAt(i)=='a'||text.charAt(i)=='e'||text.charAt(i)=='i'||text.charAt(i)=='o'||text.charAt(i)=='u'||text.charAt(i)=='y'){
   if(text.charAt(i+1)!='a'&&text.charAt(i+1)!='a'&&text.charAt(i+1)!='e'&&text.charAt(i+1)!='i'&&text.charAt(i+1)!='o'&&text.charAt(i+1)!='u'&&text.charAt(i+1)!='y'){
    if(text.charAt(i)=='e'&&text.charAt(i+1)!=' '&& text.charAt(i+1)!=','&&text.charAt(i+1)!='?'&& text.charAt(i+1)!='!'&& text.charAt(i+1)!='.'||text.charAt(i)!='e'){
      syllablecount ++;
    }
    
   }
 }
    }







    return syllablecount;
  }



  /**
   * Eventually write this one too. Get the number of sentences in the document/paragraph.
   * Sentences are defined as contiguous strings of characters ending in an 
   * end of sentence punctuation (. ! or ?) or the last contiguous set of 
   * characters in the document, even if they don't end with a punctuation mark.
   */

  public int countSentences() {

  int sentencecount=0;
for( String b : stre){
  sentencecount++;
}






    return sentencecount;
  }
}
```
This bit of code was fairly difficult for me to do as it required a lot of trial and error to get the coridantes correct aswell as allow for everything to work together as intended. This code controls the snowpile growing and melting as well as the day night cycle of the sky. I overcame this code by simply not giving up and being determined to finish it and have a quality product.<br><br>
Reflection<br>
These projects taught me that i simply cant solve every problem on my own, I needed to ask questions and I needed to ensure that I understood how the code worked. I had to ask classmate for help on multiple different problems which is something I do not like doing usually, these projects made me more comfortable to do so.

