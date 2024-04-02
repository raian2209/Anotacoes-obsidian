#programação 
## Definições

* linguagem interpretada 
	* [[Interpretador]] : CPython
* dinamicamente tipada 
	*  [[Typing]]
* [[Garbage collector]]
* Paradigmas:
	* [[Orientação a Objeto]]
	* [[Programação Funcional]]
	* [[Programação Estruturada]]
* a



### declaração de variáveis:
```python

x = 1  

y = 2.5 

z,l = 2+2j, complex(2,2)

a = True

q = [10,8]

p = {'Amanda': 1.65, 'ana': 1.60}

f = (5,4)

s = 'amanda'

```

* Tupla: imutável
* String: imutável , Construtor: `str()`
	* [[Orientação a Objeto#^construtor]]
	

### Observações importantes:
usa ponteiros por referencia em memoria 
ex:
```python

x = []

y=x

x.append(5)

```