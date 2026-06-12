import javax.swing.*;
import java.awt.event.*;

public class GradeCalculator extends JFrame implements ActionListener{
   JTextField n1,n2,n3,n4,n5,n6,g1,g2,g3,g4,g5,g6,total,cgpa;
   JButton sum;
	public GradeCalculator() {
		setTitle("Grade Calculator");
		setSize(400, 400);
		setLayout(null);
		
		n1 = new JTextField("Subject 1");
		n2 = new JTextField("Subject 2");
		n3 = new JTextField("Subject 3");
		n4 = new JTextField("Subject 4");
		n5 = new JTextField("Subject 5");
		n6 = new JTextField("Subject 6");
		g1 = new JTextField("Grade 1");
		g2 = new JTextField("Grade 2");
		g3 = new JTextField("Grade 3");
		g4 = new JTextField("Grade 4");
		g5 = new JTextField("Grade 5");
		g6 = new JTextField("Grade 6");
		sum = new JButton("calculate");
		total = new JTextField("Total Numbers");
		cgpa = new JTextField("CGPA");
		
		n1.setBounds(50,20,80,25);
		n2.setBounds(50,50,80,25);
		n3.setBounds(50,80,80,25);
		n4.setBounds(50,110,80,25);
		n5.setBounds(50,140,80,25);
		n6.setBounds(50,170,80,25);
		g1.setBounds(150,20,80,25);
		g2.setBounds(150,50,80,25);
		g3.setBounds(150,80,80,25);
		g4.setBounds(150,110,80,25);
		g5.setBounds(150,140,80,25);
		g6.setBounds(150,170,80,25);
		sum.setBounds(50,210,100,30);
		total.setBounds(50,250,180,25);
		cgpa.setBounds(50,280,180,25);
		
		add(n1); add(n2); add(n3); add(n4); add(n5); add(n6);
		add(g1); add(g2); add(g3); add(g4); add(g5); add(g6);
		add(sum); add(total); add(cgpa);
		
		sum.addActionListener(this);
		
		setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		setVisible(true);		
	}
	
	public String getGrade(int marks) {
	    if (marks >= 85) return "A";
	    else if (marks >= 75) return "B";
	    else if (marks >= 65) return "C";
	    else if (marks >= 50) return "D";
	    else return "F";
	}
	
	public void actionPerformed(ActionEvent z) {
			int a = Integer.parseInt(n1.getText());
			int b = Integer.parseInt(n2.getText());
			int c = Integer.parseInt(n3.getText());
			int d = Integer.parseInt(n4.getText());
			int e = Integer.parseInt(n5.getText());
			int f = Integer.parseInt(n6.getText());
			
			g1.setText(getGrade(Integer.parseInt(n1.getText())));
			g2.setText(getGrade(Integer.parseInt(n2.getText())));
			g3.setText(getGrade(Integer.parseInt(n3.getText())));
			g4.setText(getGrade(Integer.parseInt(n4.getText())));
			g5.setText(getGrade(Integer.parseInt(n5.getText())));
			g6.setText(getGrade(Integer.parseInt(n6.getText())));
			
			int add = a+b+c+d+e+f;
			total.setText(String.valueOf(add));
			
			double cg = (add / 600.0) * 4;
		    cgpa.setText(String.valueOf(cg));
	}
	public static void main(String[] args) {
		new GradeCalculator();
	}
}
