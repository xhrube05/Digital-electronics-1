## 1. cvičení
### De Morgan's laws simulation
#### VHDL code
```vhdl
architecture dataflow of gates is
begin
    f_o 	<= ((not b_i) and a_i) or ((not c_i) and (not b_i));
    fnand_o <= not(a_i and b_i and c_i);
    fnor_o  <= not(a_i or b_i or c_i);

end architecture dataflow;
```
#### Screenshot
![Simulace De Morgan's laws](Images/demorganslawsimulation.png)
#### EDA playground link
https://www.edaplayground.com/x/E8RC
