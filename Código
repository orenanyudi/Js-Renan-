import javax.swing.*;
import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class AnimacaoSimples extends JPanel implements ActionListener {
    private int x = 0;
    private int y = 150;
    private int velocidade = 5;
    
    public void actionPerformed(ActionEvent e) {
        x += velocidade;
        if (x > 400) {
            x = 0;
        }
        repaint();
    }

    @Override
    protected void paintComponent(Graphics g) {
        super.paintComponent(g);
        g.setColor(Color.BLUE);
        g.fillOval(x, y, 50, 50);
    }

    public static void main(String[] args) {
        JFrame frame = new JFrame("Animação Simples");
        AnimacaoSimples animacao = new AnimacaoSimples();
        frame.add(animacao);
        frame.setSize(400, 200);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setVisible(true);

        Timer timer = new Timer(50, animacao);
        timer.start();
    }
}
