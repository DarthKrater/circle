# circle
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>New webpage</title>
    </head>
       <canvas id="mycanvas"></canvas> 
  <script src="https://cdn.jsdelivr.net/processing.js/1.4.8/processing.min.js"></script> 
<body>
<script>
  var programCode = function(processingInstance) {
    with (processingInstance) {
      size(400, 400); 
      frameRate(75);
var P=1;
var Speed=1;
var DMG=1;
var One=0;
var Add=10;
var H=0;
var Mu=1;
var M=0;
var X=315;
var Health=10+H;

var Circle= function() {

background(34, 0, 255);
fill(0, 255, 26);
rect(100,5,100,30);
rect(200,5,100,30);
rect(150,35,100,30);
fill(255, 0, 255);
rect(150,360,100,35);
fill(255, 0, 0);
text("Buy Multiplier",115,10,100,100);
text("Buy damage",225,10,100,100);
text("Buy ATK Speed",160,40,100,100);
fill(87, 37, 78);
text("Buy prestige",170,370,100,100);
text(Mu*1.5*10*(0.5*Mu),130,25,100,100);
text(DMG*15*(0.5*DMG),230,25,100,100);
if(Speed<14){
text(Speed*15*(0.5*Speed),180,55,100,100);
}
fill(255, 0, 0);
text(P,200,345,100,100);
fill(102, 41, 101);
text(1000*(1000*(P*2*(P)*P)),180,385,100,100);
fill(255, 0, 0);
ellipse(200,200,100,100);
fill(0, 255, 85);
ellipse(385,200,30,30);
rect(X,190,30,15);
text(M,200,100,100,100);
var Health=10+H;
if(Health<=0){
Health=10;
H+=10;
M+=Mu*10;


}
text(Health,200,125,100,100);
    



};

text(Health,200,130,100,100);



draw= function() {
X+=-1*Speed*(1*P);
Circle();    
if(X<=250){
X=315;
fill(237, 225, 113);
ellipse(250,200,55,55);
fill(214, 149, 64);
ellipse(250,200,40,40);
fill(255,0,0);
ellipse(250,200,25,25);

H+=-1*DMG;
mouseClicked=function(){

if(mouseX>=100&&mouseX<=200&&mouseY>=5&&mouseY<=35){
if(M>=10*(Mu*1.5)*(Mu*0.5)){M+=-10*(Mu*1.5)*(0.5*Mu);

Mu+=1;

}
}
if(mouseX>=200&&mouseX<=300&&mouseY>=5&&mouseY<=35){
if(M>=10*(DMG*1.5)*(0.5*DMG)){M+=-10*(DMG*1.5)*(0.5*DMG);
DMG+=1;
}
}
if(Speed<=14){
if(mouseX>150&&mouseX<250&&mouseY>=35&&mouseY<=65){
if(M>=10*(Speed*1.5*(0.5*Speed))){
    M+=-10*(Speed*1.5)*(Speed*0.5);
Speed+=1;
    
}
if(mouseX>150&&mouseX<=250&&mouseY>=360&&mouseY<=395){
if(M>1000*(1000*(pow(p,3)*P))){
P+=1;    
}
if(mouseX>150&&mouseX<=250&&mouseY>=360&&mouseY<=395){
if(M>1000*(1000*(pow(p,3)*P))){
P+=1;    
}




}

}


};
}
};
}    
};
    var canvas = document.getElementById("mycanvas"); 
  var processingInstance = new Processing(canvas, programCode); 
 
    </script>
        </body>

</html>
