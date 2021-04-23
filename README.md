# NIGERIAN-TAX-CALCULATOR
A javascript code to calculate Nigeria self / direct assessment tax liability
/gross income = g, consolidated relief = c, taxable income = b, tax payable = t, minimum tax 
var g = prompt ("please enter your gross annual pay");
if  (g <= 200000) {
var t = 0.01*g;
prompt ("your tax payable is "+t);
} else {
var c = (200000 + (0.2*g));
var b = (g-c);
var a1 = ((b-300000)*0.11);
var d1 = ((b-600000)*0.15);
var e1 = ((b-1100000)*0.19);
var f1 = ((b-1600000)*0.21);;
var h1 = ((b-3200000)*0.24);
var t = null;
if (b<=300000) {
    t = 0.07*b;
    prompt ("your tax payable is "+t);
}
else if ((b>300000 )&&(b<=600000)){
    t = a1+21000;
    prompt ("your tax payable is "+t);
}
else if ((b>600000 )&&(b<=1100000)){
    t = d1+54000;
    prompt ("your tax payable is "+t);
}
else if ((b>1100000 )&&(b<=1600000)){
    t = e1+129000;
    prompt ("your tax payable is "+t);
}
else if ((b>1600000 )&&(b<=3200000)){
    t = f1+224000;
    prompt ("your tax payable is "+t);
}
else if (b>3200000){
    t = h1+560000;
    prompt ("your tax payable is "+t);
}
}
