# simplex-method
## background
作業研究加分程式
![simplex method drawio](https://user-images.githubusercontent.com/64023999/149705470-283fdeaa-ca60-435b-bfa5-f5dd861703a8.png)

本程式沒有處理化成標準式的規定
1. 目標函數最大
2. 約束條件等式
3. 決策變亮非負
4. 資源限量非負
需使用者在輸入參數時，需要注意，須符合上述四個條件。

```
void compute();
```
```
bool optimality_test();
//check if the solution is optimal
```
Parameter:
  No parameter
Return value:retuen a boolean which show the optimal solution is found
```
int find_col_pivot();
//
```
int find_row_pivot(int);
//minimum ratio test
Parameter:
  int val:  pivot column
Return value:
  int val: pivot row
```
void Gaussian_elimination(int, int);
//矩陣運算
```
Parameter:
  pivot row、pivot column
Return value:
  No return value
## install
g++
## usage
![image](https://user-images.githubusercontent.com/64023999/149707205-62521139-2909-473f-9c46-b26a6b9f398e.png)<br>

我要處理的問題為:<br>
MAX = 3 * X1 + 5 * X2;<br>
s.t.<br>
X1 <= 4;<br>
2 * X2 <= 12;<br>
3 * X1 + 2 * x2 <= 18;<br>
and<br>
X1 , X2 >= 0;<br>

請寫成線性規劃的標準型<br>
row size: ```3 ``` <br>
col size: ```6``` <br>
isMax: ```1``` <br>
objective: ```-3 * X1 -5*X2 - 0 - 0 - 0 =0```<br>
MATRIX:
```
1 * X1 + 0 * X2 + 1 * X3 + 0 * X4 + 0 * X5 = 4;
0 * X1 + 2 *X2 + 0 * X3 + 1 * X4 + 0 * X5 = 12;
3 * X1 + 2 *X2 + 0 * X3 + 0 * X4 + 1 * X5 = 18;
```
![image](https://user-images.githubusercontent.com/64023999/149711167-1ecc92d4-a72b-499b-953d-fdd52d413173.png)
```
code<test.txt
```
## example
## program function
## maintainers
## Contributing
## License
