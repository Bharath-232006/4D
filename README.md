# 4D
Half  Adder

module halfadder(a,b,sum,carry);
 input a,b; 
output sum,carry; 
assign sum=a^b; 
assign carry=a&b; 
endmodule

Half  Substractor

module HS(a,b,diff,borrow); 
input a,b; 
output diff,borrow; 
assign diff=a^b; 
assign borrow=!(a)&b; 
endmodule

Full Adder

module FA(a,b,c,sum,carry);
 input a,b,c; 
output sum,carry; 
assign sum=a^b^c;
 assign carry=(a&b)||(b&c)||(c&a); 
endmodule 

Full Substractor

module FS(a,b,c,diff,borrow);
 input a,b,c; 
output diff,borrow; 
assign diff=a^b^c;
 assign borrow=((!a)&b)|(b&c)|((!a)&c); 
endmodule
