(setq markdown-css-paths '("Chapter08.css"))
## Đồ thị cây
- **Định nghĩa**
- Cây là một đồ thị vô hướng liên thông mà không có chu trình đơn.
    + Liên thông vô hướng
    + Không có chu trình đơn

<img src="Pictures_Source/Screenshot 2024-11-02 002855.png" alt="Tree Graph" class="custom-img">

- **Định lý**
- Một đồ thị vô hướng là cây ...
## Cây có gốc
- **Định nghĩa**
- Một cây có gốc là cây có một đỉnh là gốc và mỗi cạnh đi ra trực tiếp từ gốc.

<img src="Pictures_Source\Screenshot 2024-11-02 003946.png" alt="Root Tree" class="custom-img">

## Cây m phân
- **Định nghĩa**
- Một cây có gốc gọi là một cây m phân nếu mỗi giao điểm không có nhiều hơn m con
- Một cây gọi là m phân đủ nếu mỗi giao điểm có chính xác m con.
- Một cây m phân với m=2 được gọi là nhị phân.
- Một cây có gốc có thứ tự ...
- **Tính chất**
1. Một cây có n đỉnh có n-1 cạnh
2. Với mọi cây m phân
    n = i + l
3. Với mọi cây m phân đủ
    n = mi + 1 và l = (m - 1)i + 1
- n là số nodes
- i là số giao điểm
- l là số lá
    - VD 1:
    ![Cây m phân ví dụ 1]()
        m = 5 (full), n = 56
        i = (n - 1) / m = 11
        l = 55 - 11 = 44
    - VD 2:
    ![Cây m phân ví dụ 2]()
        m = 3 (full), l = 27
        i = (l - 1) / (m - 1) = 13
        |E| = 13 * 3 = 39
        n = 39 + 1 = 40

## Chiều cao và cấp của cây có gốc
- **Định nghĩa**
- *Level (mức)* của một đỉnh trong một cây có gốc là chiều dài từ một gốc tới một đỉnh
- *Level of the root* định nghĩa là 0
- *Height* là *level* tối đa của các đỉnh.
![Cây có gốc có level và height]()
- **Định lý**
- Với một cây m-phân thì $$l \leq m^{th} => h \ge log_m(l)$$
## Cây nhị phân
- **Định nghĩa**
- Cây nhị phân là cây có cây con trái chứa các giá trị nhỏ hơn giá trị gốc và cây con phải chứa các giá trị lớn hơn cây con phải.
## Mã tiền tố
- **Định nghĩa**
- Mã tiền tố là mã mà sâu bit mã hóa không chứa các giá trị bị trùng lặp.
- **Thuật toán Huffman**
    
    google      ASCII=6 * 8 = 48 bits
    
    Bước 1:
    |char|g|o|l|e|
    |----|-|-|-|-|
    |freq|$$\frac{2}{6}$$|$$\frac{2}{6}$$|$$\frac{1}{6}$$|$$\frac{1}{6}$$|
    
    Bước 2:
    
    ![Biểu đồ cây Huffman]()
<table>
    <tr>
        <td>1</td>
        <td>11</td>
    </tr>
    <tr>
        <td>e</td>
        <td>10</td>
    </tr>
    <tr>
        <td>g</td>
        <td>01</td>
    </tr>
    <tr>
        <td>o</td>
        <td>00</td>
    </tr>
    <tr>
        <td colspan="2">12</td>
    </tr>
</table>

$$\frac{48}{12} = 4$$
- **Duyệt cây**
- *Pre-Order* là duyệt gốc -> trái -> phải
- *In-Order* là duyệt từ trái -> phải (nhỏ đến lớn)
- *Post-Order* là duyệt trái -> phải -> gốc
