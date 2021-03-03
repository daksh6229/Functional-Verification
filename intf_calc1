// Code your testbench here
// or browse Examples
interface intf_calc1 (input bit clk_c);
  logic [0:7] reset;
  logic [0:3] req1_cmd_in;
  logic [0:31] req1_data_in;
  logic [0:3] req2_cmd_in;
  logic [0:31] req2_data_in;
  logic [0:3] req3_cmd_in;
  logic [0:31] req3_data_in;
  logic [0:3] req4_cmd_in;
  logic [0:31] req4_data_in;
  logic [0:1] out_resp1;
  logic [0:31] out_data1;
  logic [0:1] out_resp2;
  logic [0:31] out_data2;
  logic [0:1] out_resp3;
  logic [0:31] out_data3;
  logic [0:1] out_resp4;
  logic [0:31] out_data4;
  
  clocking clk_mon_calc @(posedge clk_c);
    input clk_c;
    input [0:7] reset;
  	input [0:3] req1_cmd_in;
  	input [0:31] req1_data_in;
  	input [0:3] req2_cmd_in;
  	input [0:31] req2_data_in;
  	input [0:3] req3_cmd_in;
  	input [0:31] req3_data_in;
  	input [0:3] req4_cmd_in;
  	input [0:31] req4_data_in;
  	input [0:1] out_resp1;
  	input [0:31] out_data1;
  	input [0:1] out_resp2;
  	input [0:31] out_data2;
  	input [0:1] out_resp3;
  	input [0:31] out_data3;
  	input [0:1] out_resp4;
  	input [0:31] out_data4;
  endclocking:clk_mon_calc
  
  clocking clk_drv_calc @(posedge clk_c);
    input clk_c;
    input [0:7] reset;
  	output [0:3] req1_cmd_in;
  	output [0:31] req1_data_in;
  	output [0:3] req2_cmd_in;
  	output [0:31] req2_data_in;
  	output [0:3] req3_cmd_in;
  	output [0:31] req3_data_in;
  	output [0:3] req4_cmd_in;
  	output [0:31] req4_data_in;
  endclocking:clk_drv_calc
  
  modport monitor (clocking clk_mon_calc);
  
  modport driver (clocking clg_drv_calc);
  
endinterface
