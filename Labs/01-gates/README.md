## 1. cvičení
### De Morgan's laws simulation
#### VHDL code
```vhdl
architecture dataflow of gates is
begin
    f_o 	<= ((not b_i) and a_i) or ((not c_i) and (not b_i));
    fnand_o <= (not(a_i) or not(b_i) or not(c_i));
    fnor_o  <= (not(a_i) and not(b_i) and not(c_i));

end architecture dataflow;
```
#### Screenshot
![Simulace De Morgan's laws](Images/demorganslawsimulation.png)
#### EDA playground link
https://www.edaplayground.com/x/E8RC
#### Table
| **c** | **b** |**a** | **f(c,b,a)** | **fnand(c,b,a)** | **fnor(c,b,a)** |
| :-: | :-: | :-: | :-: | :-: | :-: |
| 0 | 0 | 0 | 1 | 1 | 1 |
| 0 | 0 | 1 | 1 | 1 | 0 |
| 0 | 1 | 0 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 1 | 0 |
| 1 | 0 | 0 | 0 | 1 | 0 |
| 1 | 0 | 1 | 1 | 1 | 0 |
| 1 | 1 | 0 | 0 | 1 | 0 |
| 1 | 1 | 1 | 0 | 0 | 0 |
