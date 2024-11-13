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
![Some logical equivalences](Pictures/Screenshot 2024-11-13 224747.png)
