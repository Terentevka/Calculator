             
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
   
