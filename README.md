# Random-Process
陳伯寧教授ocw-note
  
second order: 能量、first order: DC能量  
工程上care: 傳輸訊號需要花多少瓦特  

- Average power: 能量必大於0  
- Autocovariance: 能量影響的偏差(扣掉期望值)  
- Correlation Coefficient: 看相關性的程度
- Coefficient: 有時候相關性的能量很強，但事實上基礎能量很大 -> 基本上就是normalized  
- Cross Correlation: 兩個不同random process之間的相關性(x, y需定義在相同的probability space)  
  -> 最關心的是輸入與輸出之間的關係 (從通訊角度，x和y能量的相互影響。通常x:input, y:output)  
  
General Properties: 給random process一些限制，方便做實驗  
- independent: 兩個random process所有的"finite dimensional sample"為independent，joint distribution直接機率相乘。  
-> 但muti-dimensional distribution並不能表示完整random process，唯有給probability distribution才會知道。  
- Orthogonality: 能量傳送不會相互影響  
-> Antocorrelation=0(包含1st moment, 2nd moment)  
- Uncorrelation: 數學上的定義，排除1st moment(DC能量)，variance(2nd moment)沒有變異  
- White: red to purple份量都一樣，所有頻譜能量的份量是一樣的  
-> indirect: 與white這個字無關(此書定義較為廣泛)
- Independent Increment: 量子運動(布朗花粉實驗)  
  
Riemann Integral: 切長方形(分兩類: 長方形低處(比實際小)、高處(比實際大))  
-> 用step function逼近最真實面積  
  
E[s]先積分再取期望值  
-> Riemann integral保證積分和期望值可以交換: 可以先做期望值再積分 (Lebesque intergral不行)  

For example: 燈泡
- Point Process: 每個燈泡壞掉的時間點t1, t2, t3, ...  
- Renewal Process: 兩個t之間的間格是每個燈泡的life time (燈泡壞掉的週期-> renewal lightbub)  
- Counting Process: 在某段時間內燈泡壞掉的次數。  

Poisson Process:  
1. 一段時間[t1, t2]之中事件發生的隨機數目(k個poisson point)  
-> P[(N(t2)-N(t1))=k] = ...  
2. 任何兩個non-overlapping interval彼此之間為independent  
