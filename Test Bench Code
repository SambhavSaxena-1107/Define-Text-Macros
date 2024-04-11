//Example of `define text macros
`define MY_NUMBER 5
`define MY_STRING "This is Verilog"
`define ADD2PLUS2 2+2
`define ADD5(RESULT, SOURCE) \
	RESULT = SOURCE + 5; \
$display("Inside ADD5 macro. Scope is %m");

module test;
  
  reg [7:0] a, b;
  
  initial begin
    
    $display(`MY_NUMBER);
    $display(`MY_STRING);
    $display(`ADD2PLUS2);
    $display(2+2);
    
    a=1;
    `ADD5(b,a)
    $display("a:%0d, b:%0d", a, b);
     
  end
endmodule
