# Project 1 
---
## Porta logica 
### Descrição CHIP
### Expressão booleana
### Porta logica

---
## Logical Gate NOT: 

### Descrição CHIP:
<strong>  in </strong>: entrada unitária de um Bit
<strong>  out </strong>: saída unitária de um Bit

a entrada descrita como <strong>  in</strong> é  colocada nas duas entradas da porta logica <strong>  NAND</strong> fazendo a saída ser o not.

### Expressão booleana:

$in= \text{NAND}(\text{in}, \text{in})  = \overline{\text{in}}=out$

### Porta logica:
![[not.png]]


---
## Logical Gate NOT16:
### Descrição CHIP:
<strong>  in </strong>: entrada  de 16 Bits ou 2 Bytes
<strong>  out </strong>: saída de 16 Bits ou 2 Bytes

O mesmo comportamento é mesma logica só mudando o tamanho da entrada  é  saída do CHIP NOT. 

---
## Logical Gate And:

### Descrição CHIP:
<strong>  a </strong>: entrada unitária de um Bit
<strong>  b </strong>: entrada unitária de um Bit
<strong>  out </strong>: saída unitária de um Bit

a entrada descrita como <strong>  a </strong> é  colocada em uma entrada é  a <strong>  b </strong> em outra da porta logica <strong>  NAND</strong> é a saída da  <strong>Nand </strong> logicamente sera utilizada a porta  <strong>Not  </strong>para assim negar a saída é assim obter a saída esperada da porta  <strong>And  </strong>.

### Expressão booleana:

$\overline{\text{NAND}(\text{a}, \text{b})} = \overline{\text{aNandb}} = \overline{\text{out}}$


---
## Logical Gate And16:

### Descrição CHIP:
<strong>  a </strong>: entrada de 16 Bits ou 2 Bytes
<strong>  b </strong>: entrada de 16 Bits ou 2 Bytes
<strong>  out </strong>: saída de 16 Bits ou 2 Bytes

O mesmo comportamento é mesma logica só mudando o tamanho da entrada  é  saída do CHIP <Strong>And</Strong>. 

---
### Logical Gate OR:

### Descrição CHIP:
<strong>  a </strong>: entrada unitária de um Bit
<strong>  b </strong>: entrada unitária de um Bit
<strong>  out </strong>: saída unitária de um Bit

a entrada descrita como <strong>  a </strong> é  negado sera  colocada em uma entrada é  a <strong>  b </strong> é  negada também sendo colocada em outra entrada da porta logica <strong>  NAND</strong> é a saída da  <strong>Nand </strong>  sera a saída <Strong>out</Strong> , para assim obter a porta logica <Strong >OR</Strong>.

### Expressão booleana:

$\text{NAND}(\overline{\text{a}}, \overline{\text{b}}) = \text{out}$



---
### Logical Gate OR16:

### Descrição CHIP:
<strong>  a </strong>: entrada de 16 Bits ou 2 Bytes
<strong>  b </strong>: entrada de 16 Bits ou 2 Bytes
<strong>  out </strong>: saída de 16 Bits ou 2 Bytes

O mesmo comportamento é mesma logica só mudando o tamanho da entrada  é  saída do CHIP <Strong>Or</Strong>. 


---
### Logical Gate OR8Way:

### Descrição CHIP:
<strong>  in[8] </strong>: entrada de 8 Bits ou 1 Byte
<strong>  out </strong>: saída unitária de um Bit

a entrada descrita como <strong>  in[8] </strong>  onde o primeiro bit de  entrada é colocado em uma porta <Strong>Or</Strong> com o segundo é assim conseguinte com todos os bits então teremos 4 saídas resultantes disso é repetimos o processo para essas 4 fazendo a porta  <Strong>Or</Strong>  com a primeira said com a segunda resultando em duas saídas que ira ser repetir o processo aplicando a porta <Strong>Or</Strong> nessas duas saídas é assim essa ultima saída   sera a saída <Strong>out</Strong> , para assim obter a porta logica <Strong >OR8Whay</Strong>.

Com o objetivo final de ser  usada na ULA , fazendo a checagem se o  output  é zero aplicando a porta nos 8 primeiros bits é nos 8 últimos da saída é depois aplicando uma porta Or simples   

### Porta Logica:

![[Or8wai.png]]


---
### Logical Gate XOR:

### Descrição CHIP:
<strong>  a </strong>: entrada unitária de um Bit
<strong>  b </strong>: entrada unitária de um Bit
<strong>  out </strong>: saída unitária de um Bit

a entrada descrita como <strong>  a </strong> é  negada e sera  colocada em uma entrada é  a <strong>  b </strong> em outra entrada de uma porta <Strong>And</Strong> , <strong>  a </strong> sera  colocada em uma entrada é  a <strong>  b </strong> é  negada  sendo colocada em outra porta <Strong>And</Strong> , a saída  dessas duas portas logicas é  colocada em uma porta logica <Strong>Or</Strong> assim a saída dessa porta sendo o out e assim obtendo a porta logica <Strong>XOR</Strong>

### Porta Logica:
![[XOR_CHIP.png]]

### Tabela Verdade: 
![[XOR_TAB.png]]

---
### CHIP MUX:

### Descrição CHIP:
<strong>  a </strong>: entrada , unitária de um Bit
<strong>  b </strong>: entrada , unitária de um Bit
<strong>  Sel</strong>: seletor de a ou b , unitária de um Bit
<strong>  out </strong>: saída unitária de um Bit

a entrada  <strong>  a </strong> é colocada em uma porta <strong >and</strong> Junto com a entrada <strong >Sel </strong> negada,   <strong>  b </strong> é  colocada em outra porta <strong >and</strong> com o seletor como outra entrada. As duas saídas dessas duas portas <strong >and</strong>  é colocada como entrada em uma porta <strong >Or</strong>    assim a saída dessa porta sendo o out e assim obtendo o CHIP <Strong>MUX</Strong>

Sendo sendo comparado com  um if em linguagem de programação tendo o mesmo comportamento  

### Porta Logica:
![[tabMUX.png]]
### Tabela Verdade: 
![[MUX.png]]

---
### CHIP MUX16:

### Descrição CHIP:
<strong>  a </strong>: entrada , 16 Bits 
<strong>  b </strong>: entrada , 16 Bits
<strong>  Sel</strong>: seletor de a ou b , unitária de um Bit
<strong>  out </strong>: saída, 16 Bits

Tem o mesmo comportamento do <Strong>Mux </Strong> mas mudando a largura de entrada <strong>a</strong>,<strong>b</strong>  é de saída <strong>out</strong> desse chip.

---
### CHIP MUX4Way16:

### Descrição CHIP:
<strong>  a </strong>: entrada , 16 Bits 
<strong>  b </strong>: entrada , 16 Bits
<strong>  c </strong>: entrada , 16 Bits
<strong>  d </strong>: entrada , 16 Bits
<strong>  Sel</strong>: seletor de a ou b ou c ou d,   dois Bits
<strong>  out </strong>: saída, 16 Bits

Tem o mesmo comportamento do <Strong>Mux </Strong> mas mudando a largura de entrada <strong>a</strong>,<strong>b</strong> ,<strong>c</strong> ou <strong>d</strong>  é que por ter 4 entradas o <strong>sel </storng> tem largura de  dois bits então pode escolher entre 4 possibilidades de saída arquitetura desse chip consiste em dois Mux na primeira onde as entradas são os valores de entrada é o bit de SEL é o primeiro é depois a saída desses MUX vão na entrada do próximo é o bit de SEL é o segundo bit é então obtemos o  <strong>out</strong> .

### Porta Logica:
![[Mux8Way.png]]



---
### CHIP MUX8Way16:

### Descrição CHIP:
<strong>  a </strong>: entrada , 16 Bits 
<strong>  b </strong>: entrada , 16 Bits
<strong>  c </strong>: entrada , 16 Bits
<strong>  d </strong>: entrada , 16 Bits
<strong> e </strong>: entrada , 16 Bits 
<strong>  f </strong>: entrada , 16 Bits
<strong>  g </strong>: entrada , 16 Bits
<strong>  h </strong>: entrada , 16 Bits
<strong>  Sel</strong>: seletor de a ou b ou c ou d ou e ou f ou g ou h ,   3 Bits
<strong>  out </strong>: saída, 16 Bits

Tem as mesma função de Mux4way16 so que com o dobro das opções é com mais um bit de seleção para se adequar a quantidades de entrada. 

---
### CHIP DMux:

---
### CHIP DMux4Way:
---
### CHIP DMux8Way:
---
# Project 2 


---
### CHIP FULL_ADD:
---
### CHIP HALF_ADD:
---
### CHIP ADD16:
---
### CHIP INC16:
---
### CHIP ALU: