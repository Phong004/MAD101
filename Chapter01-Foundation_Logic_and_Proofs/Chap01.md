## Propositional logic
- Mệnh đề là 1 <u>tuyên bố</u> hoặc *đúng*, hoặc *sai*, nhưng *không là cả 2*.

|  p|  q|$$\neg p$$|$$\neg q$$|$$p\land q$$|$$p\lor q$$|$$p\oplus q$$|$$p\rightarrow q$$|$$p\iff q$$|
|:-:|:-:|:--------:|:--------:|:----------:|:---------:|:----------:|:-----------------:|:---------:|
|0|0|1|1|0|0|0|1|1|
|0|1|1|0|0|1|1|1|0|
|1|0|0|1|0|1|1|0|0|
|1|1|0|0|1|1|0|1|1|

- $$q\rightarrow p$$ là đảo (Converse) của $$p\rightarrow q$$
- $$\neg q\rightarrow \neg p$$ là phản đảo (Contrapositive) của $$p\rightarrow q$$
- $$\neg p\rightarrow \neg q$$ là ngược của $$p\rightarrow q$$
**Thứ tự thực hiện phép toán logic**: trong ngoặc -> ngoài ngoặc -> phủ định -> and, or -> condition, bicondition.
## Propositional Equivalences
1. ***Tautology***: là mệnh đề phức luôn đúng không phụ thuộc chân trị của biến. -> 2 mệnh đề p và q tương đương logic $$p\equiv q$$
2. ***Contradiction***: là một mệnh đề phức luôn sai.
3. ***Contingency***: là một mệnh đề đúng, sai phụ thuộc chân trị của biến.
![Some logical equivalences](<Pictures_Source/Screenshot 2024-11-13 224747.png>)
**Following claims:**
1. $$p\rightarrow q\equiv\neg p\lor q$$
2. $$(p\rightarrow q)\lor(q\rightarrow r)\equiv p\rightarrow(q\lor r)$$
3. $$(p\iff q)\equiv(p\rightarrow q)\land(q\rightarrow p)$$
4. $$p\oplus q\equiv\neg(p\iff q)$$
## Predicates and Quantifiers
- Khẳng định của P($$x_1, x_2,..., x_n$$) là giá trị của hàm mệnh đề P (được định nghĩa trong tập U) tại n-tuple $$(x_1, x_2,..., x_n)$$ và P cũng được gọi là vị từ n-place hoặc một vị từ m-ary.
- Có 2 cách để định dạng một mệnh đề P(x) ($$x\in U$$):
  1. Xem xét P(x) tại một số phần tử $$x\in U$$.
  2. Thêm **lượng từ** vào P(x)
**Quantifiers**
1. Universal quantifier: $$\forall xP(x)\equiv$$ "P(x) for all values of $$x\in U$$"
2. Existential quantifier: $$\exists xP(x)\equiv$$ "There exists an element $$x\in U$$ s.t. P(x)"
3. Uniqueness quantifier: $$\exists!xP(x)\equiv$$ " There exists a unique $$x\in U$$ such that P(x) is true"
- **Lượng từ lồng nhau** khẳng định rằng có hữu hạn các lượng từ mà tại đó một lượng từ nằm trong tầm của lượng từ khác.
![The order of quantifiers](<Pictures_Source/Screenshot 2024-11-13 234525.png>)
**Phủ định lượng từ lồng nhau**
  1. Dịch dấu phủ định sang phải ($$\neg$$)
  2. Thay $$forall$$ bằng $$\exists$$ và ngược lại.
## Rule of Inference - Luật suy diễn
![alt text](<Pictures_Source/Screenshot 2024-11-13 235232.png>)
![alt text](<Pictures_Source/Screenshot 2024-11-13 235623.png>)
