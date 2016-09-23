/**
 * This program's lucky subscriber is Łɛɠợℓɑş Ǥṛɛɛɳℓɛɑƒ check out this friendly programmer's awesome projects here:
 * https://www.khanacademy.org/profile/Indeluin/projects
 *                        Credits:
 * Chester Banks for the logo
 */
var page = 0;
var Logo = function() {
    this.speed = 50;
    this.swing = 100;
    this.speedPlus = this.speed;
    this.glowPlus = width * 1.4;
    this.leg = function(x, y, rot) {
        pushMatrix();
        translate(x, y);
        rotate(rot);
        line(0, 0, 50, -20);
        line(90, 40, 50, -20);
        popMatrix();
    };
    this.arm = function(x, y, rot) {
        pushMatrix();
        translate(x, y);
        rotate(rot);
        line(0, 0, 50, 20);
        line(50, 20, 90, -10);
        popMatrix();
    };
};
Logo.prototype.draw = function() {
    noStroke();
    textAlign(CENTER, CENTER);
    textFont(createFont("Trebuchet MS"));
    pushMatrix();
    rotate(-15);
    for (var i = 0; i < height * 1.5; i += 15) {
        fill(lerpColor(
            color(102, 102, 102),
            color(0, 0, 0),
            i / (height * 1.5)));
        rect(-width / 3.9, i, width + 200, 16);
    }
    popMatrix();
    pushMatrix();
    scale(1.0, 0.8);
    translate(-250 + ((frameCount * 10) - 200) % (width * 2), height / 4);
    rotate(frameCount / 10);
    fill(0, 0, 0);
    stroke(0, 0, 0);
    strokeWeight(20);
    ellipse(200, 100, 100, 100);
    noFill();
    strokeWeight(30);
    arc(184, 211, 15, 112, -270, -90);
    this.leg(180, 270, 80 + sin(frameCount * (this.speed - this.speedPlus)) * this.swing);
    this.leg(180, 270, 80 + sin(-frameCount * (this.speed - this.speedPlus)) * this.swing);
    this.arm(175, 200, 80 + sin(-frameCount * (this.speed - this.speedPlus)) * this.swing);
    this.arm(175, 200, 80 + sin(frameCount * (this.speed - this.speedPlus)) * this.swing);
    popMatrix();
    this.speedPlus /= 1.001;
    textSize(60);
    textLeading(50);
    fill(255, 255, 255, 30);
    pushMatrix();
    translate(width / 2, height / 4.7);
    if (this.speedPlus < 40 && this.glowPlus) {
        scale(sin(frameCount * 5), 1);
        rotate(cos(frameCount * 3) * 20);
    }
    for (var i = 0; i < 360; i += 30) {
        text('SHADOW\nRUNNER', sin(i) * this.glowPlus, cos(i) * this.glowPlus);
    }
    popMatrix();
    if (this.speedPlus < 40 && this.glowPlus) {
        this.glowPlus /= 1.1;
    }
    if (this.speedPlus < 30) {
        page = 1;
    }
};
var logo = new Logo();
var cherry = function(x, y, s) {
    translate(x, y);
    scale(s);
    strokeCap(ROUND);
    fill(255, 0, 0);
    ellipse(155, 200, 100, 100);
    fill(0);
    ellipse(130, 210, 15, 15);
    ellipse(180, 210, 15, 15);
    arc(155, 220, 30, 30, 360, 539);
    fill(255);
    ellipse(131, 208, 8, 8);
    ellipse(181, 208, 8, 8);
    fill(200, 0, 0);
    arc(155, 230, 15, 10, 180, 360);
    noStroke();
    fill(255);
    ellipse(175, 168, 10, 10);
    strokeWeight(10);
    stroke(0, 0, 0, 25);
    fill(0, 0, 0, 0);
    arc(155, 160, 18, 5, 360, 540);
    noFill();
    stroke(0, 190, 0);
    arc(198, 124, 100, 120, 150, 280);
    fill(0, 190, 0);
    strokeCap(ROUND);
    noStroke();
    strokeWeight(10);
    stroke(255);
    noFill();
    rotate(45);
    arc(257, 5, 35, 20, 260, 320);
    resetMatrix();
};
var olive = function(x, y, s) {
    translate(x, y);
    scale(s);
    fill(0, 0, 0, 25);
    ellipse(80, 270, 120, 20);
    fill(51, 122, 0);
    ellipse(80, 200, 110, 150);
    fill(173, 226, 255);
    arc(80, 134, 80, 20, 180, 360);
    fill(0, 103, 0);
    arc(80, 134, 40, 20, 180, 360);
    fill(0);
    ellipse(50, 225, 15, 15);
    fill(255);
    ellipse(53, 222, 5, 5);
    fill(0);
    ellipse(110, 225, 15, 15);
    fill(255);
    ellipse(113, 222, 5, 5);
    fill(0);
    arc(80, 240, 40, 40, 361, 540);
    fill(200, 0, 0);
    arc(80, 250, 20, 10, 180, 360);
    resetMatrix();
};
var mushroom = function(x, y) {
    translate(x, y);
    fill(0, 0, 0, 50);
    ellipse(90, 270, 130, 50);
    fill(255);
    (rect)(55, 200, 70, 80, 0, 0, 15, 15);
    arc(90, 200, 125, 125, 180, 360);
    fill(0);
    ellipse(70, 235, 15, 15);
    ellipse(110, 235, 15, 15);
    arc(90, 265, 30, 30, 181, 360);
    fill(200, 0, 0);
    arc(90, 255, 12, 12, 0, 180);
    fill(255);
    ellipse(73, 233, 5, 5);
    ellipse(113, 233, 5, 5);
    fill(0, 0, 0, 25);
    rect(55, 200, 70, 5);
    resetMatrix();
};
var tomAndCherry = function() {
    // Cherry
    fill(0, 0, 0, 25);
    ellipse(250, 180, 50, 50);
    ellipse(320, 180, 50, 50);
    triangle(50, 85, 90, 70, 50, 20);
    triangle(130, 75, 170, 85, 170, 20);
    ellipse(100, 250, 200, 50);
    ellipse(285, 250, 100, 50);
    cherry(130, 20);
    noStroke();
    fill(0);
    arc(285, 225, 25, 25, 0, 180);
    stroke(0, 0, 0, 50);
    strokeWeight(5);
    point(265, 242);
    point(304, 242);
    stroke(0);
    noFill();
    arc(250, 225, 60, -30, 180, 270);
    arc(255, 243, 80, -20, 180, 270);
    arc(320, 229, 60, 20, 360, 450);
    arc(320, 242, 60, 20, 360, 450);
    // Tomato
    noStroke();
    fill(255, 0, 0);
    ellipse(110, 165, 200, 200);
    fill(0);
    (rect)(50, 170, 30, 30, 50, 50, 0, 50);
    (rect)(135, 170, 30, 30, 50, 50, 50, 0);
    triangle(90, 185, 125, 185, 107.5, 200);
    fill(255);
    ellipse(70, 180, 10, 10);
    ellipse(155, 180, 10, 10);
    strokeWeight(5);
    stroke(0);
    noFill();
    arc(117, 198, 20, 25, 360, 540);
    arc(97, 198, 20, 25, 360, 540);
    stroke(0);
    noFill();
    arc(50, 195, 86, -30, 180, 270);
    arc(55, 218, 90, -20, 180, 270);
    arc(170, 198, 90, 20, 360, 450);
    arc(165, 218, 100, 20, 360, 450);
    strokeWeight(8);
    stroke(0, 0, 0, 50);
    point(70, 210);
    point(145, 210);
    noStroke();
    fill(0, 255, 0);
    triangle(100, 110, 110, 70, 120, 110);
    triangle(120, 110, 160, 90, 130, 122);
    triangle(130, 120, 170, 140, 125, 134);
    triangle(125, 134, 110, 165, 100, 134);
    triangle(100, 134, 95, 120, 65, 128);
    triangle(95, 120, 100, 110, 70, 96);
    ellipse(112, 122, 35, 35);
};
mouseClicked = function() {
    page++;
};
draw = function() {
    textAlign(LEFT);
    noStroke();
    background(173, 226, 255);
    textFont(createFont("Trebuchet MS"));
    textSize(15);
    fill(0);
    text("CLICK!", 346, 383);
    switch (page) {
        case 0:
            logo.draw();
            break;
        case 1:
            fill(0);
            textSize(80);
            text("CUTE", 100, 150);
            fill(0);
            textSize(40);
            text("FRUITS AND VEGGIES", 20, 255);
            textSize(13);
            translate(200, 294);
            resetMatrix();
            break;
        case 2:
            // Cherry 1
            cherry(0, 0, 1);
            // Cherry 2
            noStroke();
            cherry(100, 0, 1);
            // Cherry 1 bubble
            noStroke();
            fill(255);
            rect(10, 100, 110, 70, 70);
            textSize(22);
            fill(0);
            text("We're", 30.5, 130);
            text("twins!", 33, 155);
            fill(255);
            triangle(100, 165, 110, 175, 119, 125);
            // Cherry 2 bubble
            noStroke();
            fill(255);
            rect(295, 100, 110, 125, 70);
            fill(0);
            text("I never", 310, 132);
            text("forget", 312, 155);
            text("his", 328, 180);
            textSize(20);
            text("birthday!", 308, 205);
            fill(255);
            triangle(300, 220, 310, 212, 320, 219);
            // The text below
            rect(130, 340, 150, 50, 50);
            fill(0);
            textSize(30);
            text("Cherries", 145, 375);
            break;
        case 3:
            // Olive 1
            olive();
            // Olive 2
            olive(125, 1, 1);
            // Olive 3
            olive(250, 0, 1);
            // Olive 1 bubble
            fill(255);
            rect(20, 30, 120, 70, 50);
            triangle(60, 85, 80, 120, 90, 100);
            fill(0);
            textSize(30);
            text("Love us", 25, 75);
            // Olive 2 bubble
            fill(255);
            rect(150, 30, 120, 70, 50);
            triangle(190, 85, 210, 120, 220, 100);
            fill(0);
            textSize(23);
            text("or hate us", 155, 75);
            // Olive 3 bubble
            fill(255);
            rect(275, 30, 120, 70, 50);
            triangle(315, 85, 335, 120, 345, 100);
            fill(0);
            textSize(21);
            text("You've got", 280, 60);
            text("to love us!", 285, 85);
            // The text below
            fill(255);
            rect(130, 340, 150, 50, 50);
            fill(0);
            textSize(30);
            text("Olives", 160, 375);
            break;
        case 4:
            background(107, 0, 143);
            textSize(15);
            fill(0);
            text("CLICK!", 346, 383);
            // Mushroom 1
            mushroom(20, 0);
            // Mushroom 2
            mushroom(200, 0);
            // Mushroom 1 bubble
            fill(255);
            rect(40, 30, 150, 90, 150);
            triangle(95, 120, 125, 120, 110, 135);
            fill(0);
            textSize(25);
            text("No one tells\nus anything", 46, 70);
            // Mushroom 2 bubble
            fill(255);
            rect(220, 30, 175, 90, 150);
            triangle(275, 120, 305, 120, 290, 135);
            fill(0);
            textSize(25);
            text("We're always", 230, 70);
            textSize(22);
            text("kept in the dark", 225, 95);
            // The text below
            fill(255);
            rect(110, 340, 180, 50, 150);
            fill(0);
            textSize(25);
            text("Mushrooms", 130, 370);
            break;
        case 5:
            tomAndCherry();
            // The text below
            fill(255);
            rect(80, 340, 220, 50, 150);
            fill(0);
            textSize(25);
            text("Tom and Cherry", 100, 370);
            break;
        case 6:
            page = 1;
            break;
    }
};
