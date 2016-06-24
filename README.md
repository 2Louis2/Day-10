# Day-10

import javax.swing.JApplet;
import java.awt.*;

public class Snowman extends JApplet {
	
	public void paint (Graphics page)
	{
		int MID = 50;
		int TOP = 150;
		int x = 0, y = 0;
		
		for (x = 0; x < 500; x++)
			{
			
				for (y = 0; y < 2000000; y++)
				{
					setBackground (Color.cyan);
				}
		
				page.setColor (Color.green);
				page.fillRect (0, 275, 800, 500);
		
				page.setColor (Color.yellow);
				page.fillOval (-40, -40, 180, 180);
		
				page.setColor(Color.white);
				page.fillOval(MID+150, TOP, 40, 40);
				page.fillOval(MID+135, TOP+35, 70, 50);
				page.fillOval(MID+120, TOP+80, 100, 60);
		
				page.setColor(Color.black);
				page.fillOval(MID+160, TOP+10, 5, 5);
				page.fillOval(MID+175, TOP+10, 5, 5);
		
				page.drawArc(MID+160, TOP+10, 20, 20, 190, 160);
		
				page.drawLine(MID+155, TOP+60, MID+110, TOP+40);
				page.drawLine(MID+205, TOP+60, MID+255, TOP+60);
					
			if ( x % 2 == 0)
				
				{
		
				page.drawLine(MID+150, TOP+5, MID+190, TOP+5);
				page.fillRect(MID+155, TOP-20, 30, 25);
				
				
			    }
			
			}	
	}

}
