Calculator
==========

package base;
import java.text.DecimalFormat;
import java.text.DecimalFormatSymbols;
public class NewJFrame extends javax.swing.JFrame {
    private float a;
    private float c;
    private float b;
    private float d;
    public NewJFrame() {
        initComponents();
    }                       
a = Float.parseFloat(jTextField1.getText());
c = Float.parseFloat(jTextField2.getText()); 
b = Float.parseFloat(jTextField3.getText());
d = Float.parseFloat(jTextField4.getText());
this.textArea1.append(String.valueOf("\r\n"));
double e1 =((a-d)+(((a-d)*(b/100))/12*c));
e1=e1*100;
int y=(int) Math.round(e1);
e1=(double)y/100;
double f =((a-d)/c);
f=f*100;
int i = (int) Math.round(f);
f=(double)i/100;
textArea1.setText(String.valueOf("Ежемесячный платеж=" +  f +"\r\n"+ "\r\n"+"Общая сумма выплат=" +e1));
    }                                        
    private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {                                         
a = Float.parseFloat(jTextField1.getText());
c = Float.parseFloat(jTextField2.getText()); 
b = Float.parseFloat(jTextField3.getText());
d = Float.parseFloat(jTextField4.getText());
this.textArea1.append(String.valueOf("\r\n"));
 double m=0;
 double l=0;
 double j=a/c;
 double s1=a-d;
 while (c> 0) {
     double f1=j+(s1-(j*m))*(b/100)/12;
     f1=f1*100;
     int i = (int) Math.round(f1);
     f1=(double)i/100;
     this.textArea1.append(String.valueOf("\r\n"+"Ежемесячный платеж= " +f1 + "\r\n"));
     c=c-1;
     l=l+f1;
     m=m+1;
 }
 this.textArea1.append(String.valueOf("\r\n" +"Общая сумма выплаты=  " +l));
    }                                        
    public static void main(String args[]) {    
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new NewJFrame().setVisible(true);
            }
        });
    }
    // Variables declaration - do not modify                     
    private javax.swing.JButton jButton1;
    private javax.swing.JButton jButton2;
    private javax.swing.JColorChooser jColorChooser1;
    private javax.swing.JLabel jLabel1;
    private javax.swing.JLabel jLabel2;
    private javax.swing.JLabel jLabel3;
    private javax.swing.JLabel jLabel4;
    private javax.swing.JLabel jLabel5;
    private javax.swing.JPanel jPanel1;
    private javax.swing.JScrollPane jScrollPane1;
    private javax.swing.JScrollPane jScrollPane3;
    private javax.swing.JTextArea jTextArea1;
    private javax.swing.JTextField jTextField1;
    private javax.swing.JTextField jTextField2;
    private javax.swing.JTextField jTextField3;
    private javax.swing.JTextField jTextField4;
    private javax.swing.JTextPane jTextPane1;
    private java.awt.TextArea textArea1;
}
