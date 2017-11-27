function plus(){
var k0,c0,c1,c2,c3,v1,v2,v3,v4,x1,ph1,y,z,m,x2,ph2,n1,n2,n3,x3,ph3;
k0 = document.getElementById('K0').value;
c0 = document.getElementById('C0').value;
c1 = document.getElementById('C1').value;
c2 = document.getElementById('C2').value;
c3 = document.getElementById('C3').value;
v1 = document.getElementById('V1').value;
v2 = document.getElementById('V2').value;
v3 = document.getElementById('V3').value;
v4 = document.getElementById('V4').value;
x1= -1*(k0/2)+Math.sqrt(Math.pow(k0/2,2)+Math.pow(k0,2)*Math.pow(c0,2));
ph1=-1*Math.log10(x1);
y=v1+v2;
z=(c0*v1)/y;
m=(c1*v2)/y;
x2=k0*z/m;
ph2=-1*Math.log10(x2+m);
n1=v1+v2;
n2=(v3*c0-v4*c2)/n1;
n3=(v4*c2)/n1;
x3=-1*(k0+n3/2)+Math.sqrt(Math.pow(k0+n3/2,2)+k0*n2);
ph3=-1*Math.log10(x3);
//innerHTML
document.getElementById('out').innerHTML = ph1+ '    ' +ph2+'     ' +ph3;

} 