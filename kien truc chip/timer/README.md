# 8 bit timer 
+ 4 block 
    * Register <=> APB bus
    * Interrupt  -> interrupt 
    * Clock divisior  <-> ker_clk
    * Counter -> 


=============================================
khai niem:
D fliflop // cach hoat dong 
```bash
module d_ff(D, Clk, reset_n, Q);
    // Port declaration
    input wire D;
    input wire Clk;
    input wire reset_n;
    output reg Q;

    // Functionality of design 
    always @ (posedge CLk or negedge reset_n)
        begin 
            if(reset_n == 1'b0) begin 
                Q <= 1'b0
            end
            else begin 
                Q <= D;
            end
        end
endmodule
```
