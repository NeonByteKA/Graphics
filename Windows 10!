/**
 * This program's lucky subscrber is Josiah The Calculus Way!!!. 
 * Look at his projects here:
 * https://www.khanacademy.org/profile/Hsh3/projects
 * Subscribe to me here:
 * https://www.khanacademy.org/computer-programming/subscribe-to-shadow-runner/6083696511
 *                  Credits
 * Chester Banks: For telling me how to add the typing 
functionality
 */ 
var scene = "startingScreen";
var username = "Shadow Runner";
var language = "eng";
var powerOff = function() {
    stroke(255);
    noFill();
    strokeWeight(2);
    arc(560, 580, 25, 25, 280, 620);
    line(560, 562, 560, 575);
};
var netSign = function(x, y, s) {
    translate(x, y);
    scale(s);
    stroke(255);
    strokeWeight(2);
    arc(535, 590.3, 18, 18, 180, 270);
    arc(535, 590.3, 28, 28, 180, 270);
    arc(535, 590.3, 38, 38, 180, 270);
    strokeWeight(5);
    point(533, 589);
    resetMatrix();
};
var startingScreen = function() {
    cursor(ARROW);
    fill(163, 163, 163);
    ellipse(300, 195, 180, 180);
    strokeWeight(8);
    strokeCap(SQUARE);
    stroke(255, 255, 255);
    ellipse(300, 160, 70, 70);
    arc(300, 245, 100, 100, 181, 360);
    noStroke();
    fill(255);
    textFont(createFont("Segoe UI"));
    textSize(35);
    text(username, 185, 320);
    textFont(createFont("Calibri Light"));
    stroke(255);
    textSize(25);
    fill(255);
    textFont(createFont("Calibri"));
    text(language.toUpperCase(), 460, 585);
    powerOff();
    netSign();
    if(mouseX >= 460 && mouseX <= 500 && mouseY >= 565 && mouseY <= 585) {
        cursor(HAND);
        noStroke();
        fill(0, 0, 0, 80);
        rect(457, 555, 52, 40);
        fill(255);
        textSize(25);
        textFont(createFont("Calibri"));
        text(language.toUpperCase(), 460, 585);
        if(mouseIsPressed) {
            scene = "keyboardLanguageOptions";
        }
    }
    if(mouseX > 515 && mouseX < 535 && mouseY > 570 && mouseY < 590) {
        cursor(HAND);
        if(mouseIsPressed) {
            scene = "net";
        }
    }
    if(mouseX > 180 && mouseX < 405 && mouseY > 350 && mouseY < 380) {
        cursor(TEXT);
    }
};
var homePage = function() {
    
};
var keyboardLanguageOptions = function() {
    startingScreen();
    noStroke();
    fill(50);
    rect(250, 445, 250, 120);
    fill(2, 171, 171);
    rect(250, 453, 250, 55);
    fill(255);
    textFont(createFont("Calibri"));
    textSize(25);
    text(language.toUpperCase(), 260, 480);
    text(language.toUpperCase(), 260, 535);
    textFont(createFont("Segoe UI"));
    textSize(15);
    text("English (United States)", 320, 473);
    text("US Keyboard", 320, 493);
    text("English (India)", 320, 528);
    text("Indian Keyboard", 320, 548);
};
var net = function() {
    startingScreen();
};
draw = function() {
    noStroke();
    image(getImage("landscapes/mountains-and-lake"), 0, 0, 600, 600);
    if(scene === "startingScreen") {
        startingScreen();
    }
    if(scene === "keyboardLanguageOptions") {
        keyboardLanguageOptions();
    }
    if(scene === "net") {
        net();
    }
    if(scene === "homePage") {
        homePage();
    }
};
