# Lightning1

int startx = 0;
int starty = 150;
int endx = 0;
int endy = 150;

void setup()
{
  background(156, 150, 206);
  size(350,350);
  
 
}


void draw()
{
 
 fill(255,0,29);
 rect(75,200,200,150);
fill(255,0,29);
triangle(75,200,175,100,275,200);

 
stroke((int)(Math.random() * 256), (int)(Math.random() * 256), (int)(Math.random() * 256));
 while ( endx < 350) {
  endx = (int)startx + (int)(Math.random() * 9); 
  endy = (int)startx + (int)(Math.random() -9 * 0);
line(startx,starty,endx,endy);


startx=endx;
starty=endy;
 }






}


void mousePressed()
{
int startx = 0;
int starty = 150;
int endx = 0;
int endy = 150;

stroke((int)(Math.random() * 256), (int)(Math.random() * 256), (int)(Math.random() * 256));
 while ( endx < 350) {
  endx = (int)startx + (int)(Math.random() * 9); 
  endy = (int)startx + (int)(Math.random()-9 * 0);
line(startx,starty,endx,endy);
startx=endx;
starty=endy;
 }

}
