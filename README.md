

# Quy trình thiết kế và sản xuất vi mạch
1. Thiết kế ý tưởng (System Design):
    Xác định yêu cầu chức năng, hiệu suất, và kiến trúc của vi mạch.
2. Thiết kế logic (Front End):
    Chuyển ý tưởng thành mô tả phần cứng (RTL) và kiểm tra tính đúng đắn.
3. Thiết kế vật lý (Back End):
    Biến thiết kế logic thành bố cục vật lý để sản xuất.
4. Sản xuất (Manufacturing):
    Chế tạo vi mạch trên đế silicon bằng quang khắc và các công đoạn khác.
5. Kiểm tra và đóng gói (Testing & Packaging):
    Kiểm tra chức năng và đóng gói vi mạch thành sản phẩm hoàn chỉnh.


# Server EDA

https://docs.google.com/spreadsheets/d/1jVR8F3jywLz7JCUi7hqG29-D_Hrwrarb108F6GJO3dI/edit?gid=0#gid=0

USER: sem_99
PASS: Ictc@123
https://www.google.com/url?q=https://ictc.edu.vn/lo-trinh-bat-dau-nganh-vi-mach-ban-dan/&sa=D&source=editors&ust=1741500818277042&usg=AOvVaw3Y6As0XNnmG2-GAnr_14LM

-------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------

# Theory
1. What is ASIC design flow?
ASIC design flow là quy trình thiết kế và sản xuất một vi mạch tích hợp dành riêng cho một ứng dụng cụ thể. Quy trình này bao gồm các bước từ đặc tả yêu cầu, thiết kế kiến trúc, thiết kế RTL, kiểm tra chức năng, tổng hợp, bố trí và định tuyến, kiểm tra vật lý, và cuối cùng là sản xuất chip.

2. Can you explain a little bit about each step in the ASIC design flow?
    * Specification: Xác định yêu cầu thiết kế.
    * Architecture Design: Thiết kế kiến trúc tổng thể.
    * RTL Design: Mô tả thiết kế bằng ngôn ngữ HDL.
    * Functional Verification: Kiểm tra chức năng của RTL.
    * Synthesis: Chuyển đổi RTL thành netlist.
    * Place and Route: Bố trí và định tuyến các cổng logic.
    * Physical Verification: Kiểm tra layout để đảm bảo tuân thủ các quy tắc sản xuất.
    * Tape-out: Gửi layout đến nhà máy sản xuất.

3. What are the inputs for DV engineers?
    * Tài liệu đặc tả yêu cầu (Specification Document).
    * Code RTL từ nhóm thiết kế.
    * Test Plan (kế hoạch kiểm tra).
    * Công cụ kiểm tra (simulator, coverage tools).

4. What isg the activity of DV after etting input from the RTL designer?
    * Phân tích yêu cầu.
    * Xây dựng Test Plan.
    * Xây dựng Testbench.
    * Viết và chạy Test Cases.
    * Phân tích kết quả và báo cáo lỗi.
    * Thu thập và phân tích coverage.

5. What is DV engineer responsibility?
    * Hiểu và phân tích yêu cầu thiết kế.
    * Xây dựng Test Plan và Testbench.
    * Viết và chạy Test Cases.
    * Phân tích kết quả và báo cáo lỗi.
    * Thu thập và phân tích coverage.
    * Hợp tác với nhóm thiết kế để sửa lỗi.

-------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------
``` bash 
vsim // open tools

folder:
    counter.v # RTL Design 
    tb_counter.v  # test bench - board ### DV - counter.v -> tb_counter.v -> test 
    Makefile

file -> change directory -> folder test 
1. compile // syntax
2. simulation // check function - giai thuat 

STEP 1:
    compile -> compile 
    simulation -> start simulation -> optimization options -> apply full ... -> ok
                -> work -> tb_file -> ok
STEP 2:
    GET SIGNAL on "objects" -> add wave 
    simulation -> run/ run all -> no 

```


-------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------
# Makefile
``` bash 
build:
run:
wave:
help:

```
-------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------
# Use VIM
``` bash
: set nu # set number line 
vi ~/.vimrc # set command use for file 

```


=============================================================================================
# ROADMAP 
1. Hệ thống số và cổng logic - 3 days
    * Các thành phần cơ bản trong hệ thống máy tính https://www.youtube.com/watch?v=J66rEt1YOB4 
    * khái niệm, chức năng cổng CMOS 
    * cổng logic 
    * Ứng dụng bìa Karnaugh để đơn giản hàm Boolean
    * mạch tổ hợp và mạch tuần tự

2. qui trình - 1 days 
3. ngôn ngữ verilog - 5 days 
    * Verilog data type
    * Verilog assignment and operator
    * Module instance
    * Cách tạo một cấu trúc module dùng module instance
    Bài tập: thiết kế một module có sử dụng module instance để tạo thành cấu trúc module

    * Mạch tổ hợp 
    * Cấu trúc always dùng để thiết kế mạch tổ hợp
    * Cách thiết kế mạch tổ hợp dùng continuous assignment và procedural assignment.
    * Multiplexer (mux). Cách thiết kế mux.
    * Cấu trúc if-else và case trong verilog
    * Encoder và decoder
    Bài tập: thiết kế mạch tổ hợp

    * Mạch tuần tự
    * Latch/Flip-flop
    * Dùng asynchronous và synchronous reset cho flip-flop
    Bài tập: thiết kế mạch tuần tự dựa trên sơ đồ nguyên lý


    TEST:
    * Cấu trúc initial, so sánh giữa initial và always
    * Loop trong Verilog (for, repeat, while, forever)
    * Tìm hiểu vể task trong Verilog, so sánh với function
    * System task trong Verilog.

    * Cấu trúc Test bench, cách viết test bench để kiểm tra thiết kế.
    * Ôn tập Design Verification Flow
    * Cách xây dựng verification plan để kiểm tra thiết kế


=============================================================================================

