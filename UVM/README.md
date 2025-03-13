// sysnopsys 
https://www.youtube.com/watch?v=igYsB_sKeNc&list=PLEgCreVKPx5AP61Pu36QQE0Pkni2Vv-HD

// code 
https://github.com/mayurkubavat/UVM-Examples/tree/master/projects/ahb2_uvm_tb/sim

// documentation 
https://www.chipverify.com/uvm/uvm-test
https://verificationguide.com/uvm/uvm-tutorial/
https://nguyenquanicd.blogspot.com/2019/05/uvm-bai-1-mo-ta-tong-quan-va-mo-ta-loi.html

# Giới thiệu về Systemverilog và UVM
    * Systemverilog
    * built UVM test-bench 

* What is UVM (Universal Verification Methodology) ? 
    => Xây dụng từ Systemverilog 
* SystemVerilog =>> ngôn ngữ mô tả phân cứng HDL
    + Verilog  + OOP 

* Tại sao sử dụng UVM thay vì test-bench như truyền thống. 

* Phương pháp kiểm tra ? 
    Simulation-Based Verification: Linh hoạt và dễ sử dụng.
    Formal Verification: Đảm bảo tính đúng đắn của thiết kế.
    Emulation: Kiểm tra thiết kế ở tốc độ cao.
    Hardware-Assisted Verification: Kết hợp simulation và emulation.
    Coverage-Driven Verification: Đảm bảo chất lượng kiểm tra.
    Assertion-Based Verification: Phát hiện lỗi sớm.
    Power-Aware Verification: Tối ưu hóa tiêu thụ năng lượng.
    Mixed-Signal Verification: Kiểm tra các thiết kế hỗn hợp.

* Có khả năng tái sử dụng và mở rộng 
    VD: ? 

==================================================================================
* TƯ DUY CHUNG:
    + Mục Tiêu:
        - Đảm bảo được tính đúng đắn (hoạt động đúng)
        - tìm ra lỗi 
    
    + Quy trình chung: 
        - Hiểu rõ yêu cầu của thiết kế
        - Thiết kế môi trường kiểm tra/ testbench 
        - Testcases
        - run + analyst (bug)
        - Đảm bảo các trường hợp đã thực hiện (coverage)

    + Dùng công cụ EDA (Electronic Design Automation) nào 
        - Simulation: VCS, QuestaSim, Xcelium.
        - Formal Verification: JasperGold, VC Formal.
        - Emulation: Palladium, Veloce.
    + Debug + fixbug 
==================================================================================
# LEARN TO UVM 
1. Verilog and SystemVerilog
    * Verilog
    * SystemVerilog

2. Các khái niệm cơ bản trong xác minh
    * Phương pháp 
        + phương pháp xác minh truyền thống: 
            testbench, mô phỏng, và kiểm tra chức năng.
    * Kĩ thuật: 
        + coverage-driven verification: Phương pháp xác minh dựa trên độ phủ để đảm bảo kiểm tra toàn diện thiết kế.
==================================================================================
# UVM Testbench Structure
