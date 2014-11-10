SnakeGame
=========
import java.awt.Canvas;
import java.awt.Graphics;
import java.awt.Point;
import java.util.LinkedList;



public class SnakeCanvas extends Canvas {
	
	private final int heightBox = 5;
	private final int widthBox = 5;
	private final int widthGrid = 30;
	private final int heightGrid = 30;
	
	private LinkedList<Point> snake;
	
	public void draw(Graphics g)
	{
		
	}
	
	public void drawGrid(Graphics g){
		// drawing the border rectangle
		g.drawRect(0,0, widthBox * widthGrid, heightBox*heightGrid);
		//drawing the vertical lines
		
		for (int y= widthBox; y <heightGrid * heightBox; y+=heightBox){
			
			g.drawLine(0, y, widthGrid*widthBox, y);
		}
		
		
		
	}
	
	
	

}
