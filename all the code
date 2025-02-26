const ship = "https://codehs.com/uploads/8fb970bbd3c254f872c15fc3353ae958";
const deathStarr = "https://codehs.com/uploads/528fca47ecf91a70517896a0cc532df1";
const tie = "https://codehs.com/uploads/279cca7c3b59371d421e55ce52efcedd";
const e = "https://codehs.com/uploads/ed67d6d45cb08711c729c16dc99ca29f";
const starD = "https://codehs.com/uploads/c731fcfcdc3fae3b21299d988e49e17e";
const trooper = "https://codehs.com/uploads/a2529b96b3818bb8b2a22b5616e3a4e0";
const l = "https://codehs.com/uploads/3099ec615dc6564315d1c13eb6743674";
const darth = "https://codehs.com/uploads/c35a9fb889a9f9e6f771fd14e5ee5ffe";
let t;
let image; 
let dx = 4;
let dy = 0;
let d;
let dy2 = 4;
let dx2 = 0;
let s;
let tr;
let lu;
let vader;
let bullet;
let bulle;
const dv = "https://codehs.com/uploads/58254ef0e717f7da19c85c400d99401b";
const li = "https://codehs.com/uploads/310460972f54a83126dd4152e6ab20f2";

function main(){
    console.log("Welcome to the game starwars!  To play use the arrows to move your ship and use the space bar to shoot! To Become god Press p and it makes you invinsable! If You press V you can fight darth vader! If you press b you can restart the game!");
    let j = readLine("Press Enter to start!");
    backGround();
    planet();
    falcon();
    for(let i = 0; i < 300; i++){
        stars(2 , Randomizer.nextInt(0 , 500 ) , Randomizer.nextInt(0 , 500));
}
    deathStar();
    setTimer(move , 100);
    keyDownMethod(shipMove);
    
    tieFighter(200 , 180);
    setTimer(move2 , 300);
    
    setTimer(badGuy , 1000);
    setTimer(moveB , 1000);
    //kill();
    
}


function moreBattle(){
     let rightEdge = image.getX() + image.getWidth();
     if(rightEdge > getWidth()){
         remove(d);
         stopTimer(badGuy);
         stopTimer(moveB);
         stopTimer(createB);
         stopTimer(moveT);
         setTimer(createB , 1000);
         setTimer(moveT , 1000);
         backGround();
         falcon();
         for(let i = 0; i < 300; i++){
             stars(2 , Randomizer.nextInt(0 , 500 ) , Randomizer.nextInt(0 , 500));
         }
         starDeatroyers(0 , 100);
         setTimer(move3 , 200);
         tieFighter(300 , 150);
         deadTrooper();
         setTimer(move4 , 200);
     }
    
}

function leftBattle(){
    let leftEdge = image.getX() + image.getWidth();
    if(leftEdge < 0){
        remove(d);
        stopTimer(badGuy);
        stopTimer(moveB);
        backGround();
        for(let i = 0; i < 300; i++){
            stars(2 , Randomizer.nextInt(0 , 500) , Randomizer.nextInt(0 , 500));
            
        }
        falcon();
        tieFighter(0 , 150);
        tieFighter(50 , 150);
        tieFighter(100 , 150);
        tieFighter(150 , 150);
        tieFighter(200 , 150);
        tieFighter(250 , 150);
        tieFighter(300 , 150);
        tieFighter(350 , 150);
        tieFighter(400 , 150);
        
        
        tieFighter(0 , 300);
        tieFighter(50 , 300);
        tieFighter(100 , 300);
        tieFighter(150 , 300);
        tieFighter(200 , 300);
        tieFighter(250 , 300);
        tieFighter(300 , 300);
        tieFighter(350 , 300);
        tieFighter(400 , 300);
        
    }
}

function northBattle(){
    let up = image.getY() + image.getHeight();
    if(up < 10){
        remove(d);
        stopTimer(badGuy);
        stopTimer(moveB);
        backGround();
    
    for(let i = 0; i < 300; i++){
        stars(2 , Randomizer.nextInt(0 , 500) , Randomizer.nextInt(0 , 500));
        
    }
    falcon();
    tieFighter(0 , 0);
    tieFighter(50 , 0);
    tieFighter(100 , 0);
    tieFighter(150 , 0);
    tieFighter(200 , 0);
    tieFighter(250 , 0);
    tieFighter(300 , 0);
    tieFighter(350 , 0);
    tieFighter(400 , 0);
    
    tieFighter(0 , 50);
    tieFighter(50 , 50);
    tieFighter(100 , 50);
    tieFighter(150 , 50);
    tieFighter(200 , 50);
    tieFighter(250 , 50);
    tieFighter(300 , 50);
    tieFighter(350 , 50);
    tieFighter(400 , 50);
    
    tieFighter(0 , 100);
    tieFighter(50 , 100);
    tieFighter(100 , 100);
    tieFighter(150 , 100);
    tieFighter(200 , 100);
    tieFighter(250 , 100);
    tieFighter(300 , 100);
    tieFighter(350 , 100);
    tieFighter(400 , 100);
        
    
    }
    
}
    
function celibration(){
    let down = image.getY() + image.getHeight();
    if(down > 500){
       stopTimer(badGuy);
       stopTimer(moveB);
       stopTimer(createB);
       backGround2();
       ground();
       luke();
       metal();
   
      
    }
    
    
}   


function death1(){
   let imageX = image.getX();
   let imageY = image.getY();
   let imageWidth = image.getWidth();
   let imageHeight = image.getHeight();
   
   let dX = d.getX();
   let dY = d.getY();
   let dWidth = d.getWidth();
   let dHeight = d.getHeight();
   

   
   if(imageX + imageWidth > dX && imageX < dX + dWidth && imageY + imageHeight > dY && imageY < dY + dHeight){
       remove(image);
       stopTimer(move);
       stopTimer(badGuy);
       stopTimer(createB);
       
       backGround();
       
       let txt = new Text("Game over!" , "30pt Ariel");
       txt.setColor("Red");
       txt.setPosition(110 , getHeight()/2 );
       add(txt);
     

   }
}


//function kill(){
//    let dX = d.getX();
//    let dY = d.getY();
//    let dHeight = d.getHeight();
 //   let dWidth = d.getWidth();
    
//    let bulletX = bullet.getX();
//    let bulletY = bullet.getY();
//    let bulletHeight = bullet.getHeight();
//    let bulletWidth = bullet.getWidth();
    
//    if(dX + dWidth > bulletX && dX < bulletX + bulletWidth && dY  + dHeight > bulletY && dY < bulletY + bulletHeight){
 //       remove(d);
//    }
    
    
//}
    


function backGround2(){
    let rect = new Rectangle(500 , 500);
    rect.setColor("white");
    rect.setPosition(0 , 0);
    add(rect);
}

function ground(){
    let rect = new Rectangle(500 , 500);
    rect.setColor("Green");
    rect.setPosition(0 , 300);
    add(rect);
}

function luke(){
    lu = new WebImage(l);
    lu.setSize(100 , 100);
    lu.setPosition(150 , 250);
    add(lu);
    
}

function metal(){
    let circ = new Circle(20);
    circ.setColor("Yellow");
    circ.setPosition(200 , 320);
    add(circ);
    
    
    let txt = new Text(1 , "30pt Arial");
    txt.setColor("black");
    txt.setPosition(190 , 337);
    add(txt);
    
    let txt2 = new Text("You Win!" , "30pt Arial");
    txt2.setColor("Black");
    txt2.setPosition(100 , 100);
    add(txt2);
}




let bullets = [];

function createBullet(){
    bullet = new Rectangle(5 , 10);
    bullet.setColor("red");
    bullet.setPosition(image.getX() + image.getWidth()/2 -2.5 , image.getY());
    bullets.push(bullet);
    add(bullet);
}

function moveBullets(){
    for(let i = bullets.length - 1; i >= 0; i--){
        bullets[i].move(0 , -10);
        if(bullets[i].getY() < 0){
            remove(bullets[i]);
            bullets.splice(i , 1);
        }
    }
}


let badBullets = [];  

function badGuy(){
    bulle = new Rectangle(10 , 50);
    bulle.setColor("green");
    bulle.setPosition(d.getX() + d.getWidth() /2 - 2.5 , d.getY());
    badBullets.push(bulle);
    add(bulle);
}

function moveB(){
    for(let i = badBullets.length - 1; i >= 0; i--){
        badBullets[i].move(0 , 10);
        if(badBullets[i].getY() < 0){
            remove(badBullets[i]);
            badBullets.splice(i , 1);
        }
    }
}



let tb = [];

function createB(){
    let tie = new Rectangle(10 , 20);
    tie.setColor("Green");
    tie.setPosition(t.getX() + t.getWidth()/2 -2.5 , t.getY());
    tb.push(tie);
    add(tie);
}

function moveT(){
    for(let i = tb.length - 1; i >= 0; i--){
        tb[i].move(0 , 10);
        if(tb[i].getY() < 0){
            remove(tb[i]);
            tb.splice(i , 1);
        }
    }
}


function deadTrooper(){
    tr = new WebImage(trooper);
    tr.setSize(50 , 50);
    tr.setPosition(200 , 350);
    add(tr);
}

function move4(){
    tr.move(dx , dy);
    tr.rotate(45);
}

function starDeatroyers(x , y){
    s = new WebImage(starD);
    s.setSize(200 , 200);
    s.setPosition(x , y);
    add(s);
        
    
}

function move3(){
    s.move(dy , dx);
}



function planet(){
    let earth = new WebImage(e);
    earth.setSize(400 , 400);
    earth.setPosition(0 , 350);
    add(earth);
}

function tieFighter(x , y){
    t = new WebImage(tie);
    t.setSize(40 , 40);
    t.setPosition(x , y);
    add(t);
    
    setTimer(createB , 120);
    setTimer(moveT , 120);
   
}

function move2(){
    t.move(dx , dy);
}



function backGround(){
    let rect = new Rectangle(500 , 500);
    rect.setPosition(0 , 0);
    rect.setColor("Black");
    add(rect);
}


    


function falcon(){
     image = new WebImage(ship);
     image.setSize(50 , 50);
     image.setPosition(getWidth()/2 , getHeight()/2);
     add(image);
  
}

function stars(radius , x , y){
    let circ = new Circle(radius);
    circ.setPosition(x , y);
    circ.setColor("White");
    add(circ);
}

function deathStar(){
    d = new WebImage(deathStarr);
    d.setSize(200 , 200);
    d.setPosition(0 , 0);
    add(d);
    
    
    setTimer(badGuy , 1000);
    setTimer(moveB , 50);
   
    
    
}



function move(){
    d.move(dx , dy);
    coll1();
    coll2();
    moreBattle();
    leftBattle();
    northBattle();
    moveBullets();
    celibration();
    death1();
    

   
   
   
  
}

function coll1(){
    let rightEdge = d.getX() + d.getWidth();
    if(rightEdge > getWidth()){
        dx = -dx;
  
}
}

function coll2(){
    let leftEdge = d.getX() + d.getWidth();
    if(leftEdge < 200){
        dx = -dx;
    }
}




function shipMove(e){
    if(e.key == "ArrowLeft"){
        image.move(-26 , 0);
        image.rotate(-90 , 0);
    }
    if(e.key == "ArrowRight"){
        image.move(26 , 0);
        
    }
    if(e.key == "ArrowUp"){
        image.move(0 , -26)
        
    }   
    if(e.key == "ArrowDown"){
        image.move(0 , 26);
    }
    if(e.key == " "){
        createBullet();
        soundAffect();
    }
    if(e.key == "p"){
        stopTimer(move);
        stopTimer(badGuy);
        stopTimer(createB);
        stopTimer(move2);
        stopTimer(move3);
        stopTimer(createBullet);
        stopTimer(move4);
    }
    if(e.key == "v"){
        backGround();
        stopTimer(move);
        stopTimer(badGuy);
        stopTimer(createB);
        stopTimer(move2);
        stopTimer(move3);
        stopTimer(createBullet);
        stopTimer(move4);
        dav();
        angryLuke();
        floor();
        window1();
      
        
    }
    if(e.key == "b"){
        main();
    }
 
    
}


function dav(){
    let v = new WebImage(dv);
    v.setSize(80 , 148);
    v.setPosition(300 , 200);
    add(v);
    

}

function angryLuke(){
    let l = new WebImage(li);
    l.setSize(80 , 150);
    l.setPosition( 0 , 200);
    add(l);
}

function floor(){
    let rect = new Rectangle(400 , 200);
    rect.setColor("Gray");
    rect.setPosition(0 , 350);
    add(rect);
}

function window1(){
    let circ = new Circle(100);
    circ.setColor("gray");
    circ.setPosition(200 , 150);
    add(circ);
    
    let circ2 = new Circle(80);
    circ2.setColor("Black");
    circ2.setPosition(200 , 150);
    add(circ2);
    
    for(let i = 0; i < 100; i ++){
        let circ3 = new Circle(2);
        circ3.setColor("White");
        circ3.setPosition(Randomizer.nextInt(140 , 270) , Randomizer.nextInt(100 , 210));
        add(circ3);
    }
    
    
}


function soundAffect(){
    let sound = new Sound("C4" , "drum");
    sound.setVolume(3);
    sound.playFor(2);
    
}


main();
