Documentation:
https://github.com/0xl4p/Giao-Trinh-PTIT/blob/main/K%E1%BB%B9%20thu%E1%BA%ADt%20s%E1%BB%91%20-%202013.pdf 

# Các hệ thống số 
1. decimal system 
2. binary system 
    * Cách đếm các số nhị phân
    Với 1 số nhị phan gồm n bit thì:
        - Số trạng thái là; 2^n
        - Số thập phân tương ứng lớn nhất là: 2^n -1
3. Hệ thống số thập lục phân 

# Đại số boolen và cổng logic 
1. Đại số boolen 
    - 2 mức logic 0 và 1 : mô tả hoạt động 
* Phép tính:
    - OR: 1 cộng với bất kì =>> = 1
        0 + 0 = 0
        0 + 1 = 1
        1 + 0 = 1
        1 + 1 = 1
    - AND: nhân
    - NOT: phép đảo 

* Các định lý:
* Đẳng thức hữu dụng 
* Định lý De-Morgan: 
    - Tích đảo = tổng của các đảo 
    - Tổng đảo = Tích của các đảo 

2. Cổng Logic 
7 Gate:   
    * AND
    * OR 
    * NOT 
    * NAND = AND + NOT * cong da nang 
    * NOR = OR + NOT   * cong da nang 
    * EXOR = AND + OR + NOT 
    * EXNOR 

3. Bìa Karnaugh 
Đơn giản các biểu thức logic 
Phương pháp:
    * SOP(Sum of  Products) - 1 - 0 là ĐẢO 
        - Nhóm các bit 1 liền kề nhau với số lượng 1, 2, 4, 8, ... bit 1.
        Ưu tiên cho nhóm có nhiều bit 1 (nếu có thể)
        - Mỗi một bit 1 có thể được nhóm nhiều lần nhưng các nhóm không được chồng lên nhau. (Tức là trong mỗi nhóm phải có ít nhất 1 bit 1 không nằm trong nhóm khác)

        => Xét trong 1 nhóm hững biến nào thây đổi giá trị thì bỏ qua, những biến nào không đổi giá trị thì giữ lại và lấy tích giữa các biến này.
        =>>> lấy TỔNG các TÍCH vừa tìm được ===> có hàm TỐI GIẢN  
    
    * POS(Products of Sums) - 0 - 1 là ĐẢO 
         - Nhóm các bit  0 kề nhau 

         => TÍCH CÁC TỔNG 
    
    * Trạng thái "Don't Care" : X


# Thiết kế mạch logic tổ hợp 
k/n: 
    Mạch tổ hợp là mạch có nhiều ngõ ra và nhiều ngõ vào. Mỗi ngõ ra là một hàm Boole cảu các ngõ vào.

BƯỚC 1: Vẽ sơ đồ khối, xác định các biến ngõ vào và hàm ngõ ra, điều kiện cho biến và hàm 
BƯỚC 2: Viết bảng trạng thái 
BƯỚC 3: Viết hàm ngõ ra
BƯỚC 4: Tối giản hàm ngõ ra 
BƯỚC 5: Vẽ mạch 

NOTE: mạch có chân điều khiển 
    - tích cực thấp 
    - tích cực cao 

thai thi van an
# Mạch cộng trừ nhị phân
1. Mạch cộng nhị phân 
    * Cộng bán phần - half adder 
        + Cộng 2 số binary 1 bit -> cho ra kq  ghi lại 1 bit và "NHỚ LẠI 1 BIT"
        + Chỉ thực hiện cho cột số cuối cùng của một số nhị phân (cột số có trọng số bằng 0)

    * Cộng toàn phần - full adder 
        + Cộng 2 số nhị phân 1 bit và Cộng thêm bit nhớ


2. Mạch trừ nhị phân 

# Mạch Cộng BCD 


# Mạch mã hóa - ENCODER 
MÃ HÓA: 
    - Chuyển đổi thông tin từ dạng này sang dạng khác 

* Mạch mã hóa 4->2
    "ngõ vào tác động" mức cao / mức thấp ---> 1 ngõ được tác động 

* Mạch mã hóa ưu tiên 4->2
    "ngõ vào tác động" mức cao / thấp ---> nhiều ngõ được tác động 


**** PHƯƠNG PHÁP GHÉP MẠCH ****
1. Xét ngõ ra của từng mạch nhỏ
2. Xét ngõ ra của mạch cần ghép
3. xét mối liên quan -> ghép mạch 


# Mạch giải mã - DECODER 
* Mạch 2->4
    "ngõ ra tác động" mức cao / thấp
    "ngõ vào cho phép" E tác động mức cao / thấp 

# Mạch ghép kênh - MULTIPLEXER (nhiều ngõ vào 1 ngõ ra)
MỤC ĐÍCH: 
    Chọn tín hiệu nào (kênh).
    VD: 
        kênh I1, I2, I3, I4,...
        chọn tín hiệu: S1, S2 
        ==> khi có ngõ vào cho phép -> ngõ vào chọn kênh hoạt động =>> kênh tín hiệu I sẽ được chọn VÀ nó là ngõ ra O 
    + I ... : tín hiệu ngõ vào 
    + E: ngõ vào cho phép
    + S ... : ngõ vào chọn kênh 
    + O: Ngõ ra 

* Mạch ghép kênh 2->1
    Ngõ vào cho phép E tác động mức cao 

# DEMULTIPLEXER (một ngõ vào nhiều ngõ ra )
MỤC ĐÍCH:  
    Phân phát ngõ vào (power) ra cho một rõ ra bất kì.
  
    + Có 1 ngõ vào I duy nhất
    + E: ngõ vào cho phép
    + S ... : ngõ vào chọn kênh 


# MẠCH SO SÁNH

