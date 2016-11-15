>#**Huỳnh Tấn Phát**
>
>###**BÁO CÁO HỌC CHUỖI KÍ TỰ**

>>[1.Khái niệm chuỗi kí tự](#Khái niệm chuỗi kí tự)  
>>[2.Các thao tác trên chuỗi](#Các thao tác trên chuỗi)  
>>[3.Mảng và chuỗi kí tự](#Mảng và chuỗi kí tự)  

<a name="Khái niệm chuỗi kí tự">
##1.Khái niệm chuỗi kí tự

* **Chuỗi ký tự là một dãy các ký tự đặt trong cặp dấu nháy kép.**  
* Chuỗi rỗng được ký hiệu bằng hai dấu nháy kép đi liền nhau.  
* Một chuỗi ký tự được cấp phát một khoảng nhớ cho một mảng kiểu char chứa các ký tự của chuỗi và chứa thêm ký tự `\0` là ký tự kết thúc chuỗi.  
* Mỗi ký tự của chuỗi được chứa trong một phần tử của mảng.  
Chuỗi ký tự là một trường hợp riêng của mảng một chiều khi mỗi thành phần của mảng là ký tự.  
**Khai báo:**
		`char ten_chuoi[];`  
  *Hoặc*
    `char *ten_chuoi;`  

<a name="Các thao tác trên chuỗi">
##2.Các thao tác trên chuỗi  

Ðể thực hiện các thao so sánh, gán nội dung của chuỗi này cho chuỗi khác ta sử dụng  một thư viện các hàm chuẩn là `<string.h>`.  
* **Hàm strlen:**  `int strlen(char s[])`  
	Trả về độ dài của chuỗi s, chính là chỉ số của ký tự NULL trong chuỗi.  
* **Hàm strcpy:** `strcpy(char dest[], char source[])`  
	Sao chép nội dung chuỗi source vào chuỗi dest.  
* **Hàm strchr:**  `char *strchr(char s[], char c)`  
	Tìm lần xuất hiện đầu tiên của ký tự c trong chuỗi s, trả về địa chỉ của ký tự này.  
* **Hàm strncpy:** `strncpy(char dest[], char source[], int n)`  
	 Sao chép n ký tự trong  chuỗi source vào chuỗi dest.  
* **Hàm strcat:** `strcat(char ch1[], char ch2[])`  
	Nối chuỗi ch2 vào cuối chuỗi ch1. Sau lời gọi hàm này độ dài chuỗi ch1 bằng tổng độ dài của cả hai chuỗi ch1 và ch2 trước lời gọi hàm.  
* **Hàm strncat:** `strncat(char ch1[], char ch2[],int n)`  
	Nối n  ký tự đầu tiên của ch2 vào ch1  
* **Hàm strstr:** `char *strstr(char s1[], char s2[])`  
	Tìm kiếm chuỗi s2 trong chuỗi s1, Trả về địa chỉ của lần xuất hiện đầu tiên của s2 trong s1 hoặc NULL khi không tìm thấy.  
* **Hàm strcmp:** `int strcmp(char ch1[], char ch2[])`  
	So sánh hai chuỗi ch1 và ch2. Nguyên tắc so sánh theo kiểu từ điển.  
  *Giá trị trả về:*  
     +`= 0` nếu chuỗi ch1 bằng chuỗi ch2.  
     +`>0` nếu chuỗi ch1 lớn hơn chuỗi ch2.  
     +`<0` nếu chuỗi ch1 nhỏ hơn chuỗi ch2.  

<a name="Mảng và chuỗi kí tự">
##3.Mảng và chuỗi kí tự  
**Một dạng sử dụng con trỏ đặc biệt là việc sử dụng một mảng các biến con trỏ.**  
**Khai báo:  
`type *pointer_array[size];`
*VD:* `char *temp[10];` (sẽ khai báo một mảng 10 con trỏ char có thể được dùng để khai báo một mảng để lưu trữ địa chỉ của mười chuỗi ký tự nào đó)  
***************************________________________________ THE END ________________________________***************************


