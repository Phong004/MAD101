# Đồ thị cây
- **Định nghĩa**
- Cây là một đồ thị vô hướng liên thông mà không có chu trình đơn.
    + Liên thông vô hướng
    + Không có chu trình đơn
![Tree Graph](<Pictures_Source/Screenshot 2024-11-02 002855.png>)

- **Định lý**
- Một đồ thị vô hướng là cây ...
## Cây có gốc
- **Định nghĩa**
- Một cây có gốc là cây có một đỉnh là gốc và mỗi cạnh đi ra trực tiếp từ gốc.
![Root tree](<Pictures_Source\Screenshot 2024-11-02 003946.png>)

## Cây m phân
- **Định nghĩa**
- Một cây có gốc gọi là một cây m phân nếu mỗi giao điểm không có nhiều hơn m con
- Một cây gọi là m phân đủ nếu mỗi giao điểm có chính xác m con.
- Một cây m phân với m=2 được gọi là nhị phân.
![m-arry tree](<Pictures_Source/Screenshot 2024-11-02 004017.png>)
- Một cây có gốc có thứ tự là cây có các con của giao điểm là có thứ tự
![Ordered Tree](<Pictures_Source/Screenshot 2024-11-02 004034.png>)
- **Tính chất**
1. Một cây có n đỉnh có n-1 cạnh
2. Với mọi cây m phân</br>
    n = i + l
3. Với mọi cây m phân đủ</br>
    n = $$m*i$$ + 1</br>
    l = $$(m - 1)*i$$ + 1
- n là số nodes
- i là số giao điểm
- l là số lá
    - **VD 1: How many leaves are there in a full 5-ary tree with 56 nodes?**</br>
        m = 5 (full), n = 56</br>
        $$i = \frac{n - 1}{m} = 11$$</br>
        l = 55 - 11 = 44</br>
    - **VD 2: How many leaves are there in a full 5-ary tree with 56 nodes?**</br>
        m = 3 (full), l = 27</br>
        $$i = \frac{l - 1}{m - 1} = 13$$</br>
        |E| = $$13 * 3$$ = 39</br>
        n = 39 + 1 = 40</br>
### Chiều cao và cấp của cây có gốc
- **Định nghĩa**
- ***Level (mức)*** của một đỉnh trong một cây có gốc là chiều dài từ một gốc tới một đỉnh
- ***Level of the root*** định nghĩa là 0
- ***Height*** là ***level*** tối đa của các đỉnh.
![Cây có gốc có level và height](<Pictures_Source/Screenshot 2024-11-02 at 00-41-01 Chapter 8 Trees - MAD101 - Chapter08_MAD.png>)
- **Định lý**
- Một cây m-phân có chiều cao *h* cân bằng khi tất cả các nút lá đều nằm tại *h* hoặc *h-1*
- Với một cây m-phân thì</br>
    $$l \leq m^{h} => h \ge \lceil\log_m(l)\rceil$$
## Cây nhị phân
- **Định nghĩa**
- Cây nhị phân là cây có cây con trái chứa các giá trị nhỏ hơn giá trị gốc và cây con phải chứa các giá trị lớn hơn cây con phải.

## Mã tiền tố
- **Định nghĩa**
- Mã tiền tố là mã mà sâu bit mã hóa không chứa các giá trị bị trùng lặp.
- **Thuật toán Huffman**
    1. Tìm tần số xuất hiện của mỗi ký tự
    2. Cấu trúc 1 cây nhị phân biểu diễn mã tiền tố của ký tự.
    **Notes:**
    - Sắp xếp tần số từ nhỏ tới lớn sau mỗi bước
    - Cây con có trọng số lớn nằm bên trái của cây nhị phân.
    
1. **VD1:** Use Huffman coding algorithm to encode the word “google”</br>
    google      ASCII = $$6 * 8$$ = 48 bits
    
    Bước 1:
    |char|g|o|l|e|
    |----|-|-|-|-|
    |freq|$$\frac{2}{6}$$|$$\frac{2}{6}$$|$$\frac{1}{6}$$|$$\frac{1}{6}$$|
    
    Bước 2:
    
    ![Biểu đồ cây Huffman](<Pictures_Source/image.png>)

    |o|1|
    |-|-|
    |g|01|
    |l|001|
    |e|000|
    |12|011101001000|
    
$$\frac{48}{12}=4$$

2. **VD2:** Use Huffman coding algorithm to encode the text “maximum”. 
What is the average number of bits?</br>
    maximum     ASCII = $$7*8$$ = 56 bits
    
    |char|m|a|x|i|u|
    |----|-|-|-|-|-|
    |freq|$$\frac{3}{7}$$|$$\frac{1}{7}$$|$$\frac{1}{7}$$|$$\frac{1}{7}$$|$$\frac{1}{7}$$|

    ![Binary Tree](<Pictures_Source/Screenshot 2024-11-02 031459.png>)

    |m|0|
    |-|-|
    |a|111|
    |u|100|
    |x|110|
    |i|101|
    |15|011111010101000|

    Avg bits = $$\frac{15}{7} \approx 2.14 bits$$

## Duyệt cây
- **Định nghĩa** là duyệt qua tất cả các đỉnh của cây *có gốc*.
- *Pre-Order* là duyệt gốc -> trái -> phải (N -> L -> R)
- *In-Order* là duyệt từ trái -> phải (nhỏ đến lớn) (L -> N -> R)
- *Post-Order* là duyệt trái -> phải -> gốc (L -> R -> N)
    **Note**: 
    - N: Root node
    - L: Left subtree
    - R: Right substree
    ![Tree Traversal](<Pictures_Source/Screenshot 2024-11-02 151657.png>)
    - 


