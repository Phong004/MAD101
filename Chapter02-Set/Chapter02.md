## Sets
- 1 set là một tập hợp các phần tử không có thứ tự.
  $$\emptyset\neq$${ $$\emptyset\$$ }
## Cardinality
- Nếu S là hữu hạn, lực lượng của S, |S|, là số các phần tử riêng biệt trong S.
## Power sets
- Nếu S là một tập hợp, lũy thừa tập hợp S là $$P(S)=2^S={x:x\subseteq S}$$.
- Nếu S là hữu hạn, $$|2^S|=2^{|S|}$$ (nếu |S|=n, thì $$|2^S|=2^n$$)
## Cartesian Product
- Tích chéo của 2 tập A và B là $$A\times B=\\{(a,b):a\in A\land b\in B\\}$$
- A, B fininte -> $$|A\times B|=|A||B|$$
## Set operations
- Union: $$A\cup B=\\{x:x\in A\lor x\in B\\}$$
- Intersection $$A\cap B=\\{x:x\in A\land x\in B\\}$$
- Complement (bù) của A là $$\overline{A}$$
- The symmetric difference: $$A\oplus B=\\{x:(x\in A\land x\notin B)\lor(x\in B\land x\notin A)=(A-B)\cup(B-A)=\\{x:x\in A\oplus x\in B\\}\\}$$
- **Set Indentities**
![](<Pictures_Source/Screenshot 2024-11-14 090312.png>)
![](<Pictures_Source/Screenshot 2024-11-14 090330.png>)
![](<Pictures_Source/Screenshot 2024-11-14 090349.png>)
![](<Pictures_Source/Screenshot 2024-11-14 090402.png>)
**Biểu diễn tập hợp trong máy tính**
![](<Pictures_Source/Screenshot 2024-11-14 090929.png>)
## Functions
- Hàm số f là một quy luật gán mỗi phần tử x trong A chính xác cho một phần tử y=f(x) trong B
  ![](<Pictures_Source/Screenshot 2024-11-14 091316.png>)
- A là tập xác định (domain), B là miền con (codomain) của f
- b=f(a) là ảnh của a và a là tiền ánh xạ của b.
- Tập xác định của f là tập $$\\{f(a),a\in A\\}
- Một hàm số có thể được định nghĩa là một tập các cặp có thứ tự $$\\{(a,b)|b=f(a),a\in A\\}$$
- $$\lfloor{x}\rfloor\le x\le\lceil{x}\rceil$$
**One-to-One**
  $$\forall x,y(f(x)=f(y)\rightarrow x=y) => $$A\rightarrow B$$ là one-to-one $$\iff$$
    $$\forall x,y(x\neq y)\rightarrow f(x)\neq f(y)$$
  => One-to-one trên I là một hàm tăng nghiêm ngặt hoặc giảm nghiêm ngặt
**Onto**
  $$(A\rightarrow B)\rightarrow\forall b\in B,\exists a\in A|f(a)=b$$
**Bijection**
- **Bijective** nếu nó là **one-to-one** và **onto**
## Summations
![](<Pictures_Source/Screenshot 2024-11-14 094605.png>)
  
