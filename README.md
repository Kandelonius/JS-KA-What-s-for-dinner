# JS-KA-What-s-for-dinner
javascript program for a Khan Academy challenge

Creates a "dinner plate" with fish, as well as peas and carrots and some
mashed potatoes and butter.

/*
*javascript* Creates a "dinner plate" with fish, as well as peas and carrots and some
mashed potatoes and butter.
*/

background(184, 113, 20); // wooden table
fill(0, 0, 200);
ellipse(200, 200, 350, 350); // plate
fill(86, 229, 245);
ellipse(200, 200, 300, 300); 
   
for (var i = 0; i < 150; i++) {// Peas and carrots
    fill(17, 255, 0);
    var ranX = random(150, 250);
    var ranY = random(150, 250);
    var combo = ranX + ranY;
    if(combo > 375 && combo < 425){
        ellipse(ranX, ranY, 10, 10);
    }
    fill(255, 209, 3);
    var ranX = random(150, 250);
    var ranY = random(150, 250);
    var combo = ranX + ranY;
    if(combo > 375 && combo < 425){
        ellipse(ranX, ranY, 10, 10);
    }
}

bezier(195, 250, 355, 220, 350, 5, 210, 300);//fish
noStroke();
fill(255, 255, 255);// mashed potatoes
var potX = random(115, 140);
var potY = random(160, 142);
for (var i = 0; i < 4; i+=1) {
    var potW = random(45, 60);
    var potH = random(45, 60);
    ellipse(potX, potY, potW, potH);
    potX += 15;
    potY -= 15;
}
fill(255, 238, 0);
rect(140, 125, 15, 15);// butter
