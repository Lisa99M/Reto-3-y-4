# Reto-3-y-4
Repo sobre pseudocódigo y diagramas de flujo. Ejemplo con algoritmos para hallar raíz cuadrada y números primos.

1.	Plantaer el algoritmo para btener los números primos hasta n en una sucesión, usando pseducódigo y diagrama de flujo:


```
Pseudocódigo:
n: entero
i: entero
k: entero
list1: () # A esta lista se añadirán los valores que se determinen como primos

Instrucciones:
n:= (Asignar valor del # final de la sucesión donde queremos buscar los primos)
i:= 2
k= i**0.5+1 (Redondear k a un valor entero)
Si, módulo de n, k es 0
Repetir para k= k+1 mientras k<i
Sino, añadir i a list1
Repetir desde pto.3 para i= i+1
Hacer mientras i<n
Fin

```

Diagrama de flujo
[![](https://mermaid.ink/img/pako:eNpVUs1u00AQfpVPy6U_KWqQuFhNUZrQ0gMcCCfiHqb2pB3Zng27axBK8jA8Auoj5MUY20Ft9zS7-_3NaDau8CW7zK1q_6t4pJDwbZ4r7EyPblUK8cc4O7u8WmoG1sTBjyDPZfVc1hLTOMMUHBP1N0Jk0P4vlRL2fxS1j_hJtQ8c8aPl7rdkIzeirCh847EO0vh4NyS46pwxWyommEZ5UAoD32g13mAlSrXVqM2pLTjK_klRerUn0w9sUrhvY2G8znsQt_wTvLPoE8jJyfnb96djLLok94zAPdvwFQitHuyGFg-pZn2q-abZP5Vt7Tt_NTVrG-cfdgNm3mG2C9ni4_IrrzlJwJoCdaaV-TVikoEiqgu567A3L3lf_PZ6eZgbBMMwxwNuI7iAHmxu-ii9z6fXPtainA4UzF6BTRy3R9eix7m6kWts_CSlbcCmg-UuPXLDucusLClUuct1Zzhqk1_81sJlKbQ8cu26pMRzoYdAjctWVEd75VKSD5-Hleo3a-TWpN-9_4_Z_QNFT8ta?type=png)](https://mermaid.live/edit#pako:eNpVUs1u00AQfpVPy6U_KWqQuFhNUZrQ0gMcCCfiHqb2pB3Zng27axBK8jA8Auoj5MUY20Ft9zS7-_3NaDau8CW7zK1q_6t4pJDwbZ4r7EyPblUK8cc4O7u8WmoG1sTBjyDPZfVc1hLTOMMUHBP1N0Jk0P4vlRL2fxS1j_hJtQ8c8aPl7rdkIzeirCh847EO0vh4NyS46pwxWyommEZ5UAoD32g13mAlSrXVqM2pLTjK_klRerUn0w9sUrhvY2G8znsQt_wTvLPoE8jJyfnb96djLLok94zAPdvwFQitHuyGFg-pZn2q-abZP5Vt7Tt_NTVrG-cfdgNm3mG2C9ni4_IrrzlJwJoCdaaV-TVikoEiqgu567A3L3lf_PZ6eZgbBMMwxwNuI7iAHmxu-ii9z6fXPtainA4UzF6BTRy3R9eix7m6kWts_CSlbcCmg-UuPXLDucusLClUuct1Zzhqk1_81sJlKbQ8cu26pMRzoYdAjctWVEd75VKSD5-Hleo3a-TWpN-9_4_Z_QNFT8ta)

2. Revise el procedimiento matemático para hallar raices cuadradas (son divisiones y restas), plantee el algoritmo en pseudocódigo y en diagrama de flujo.

```
n: entero
r: entero
rc: float
d : entero
dif: entero
m : entero
e(10): entero

Instrucciones: 

n = número al que queremos hallar la raíz cuadrada 
r = 2
d = 1
e = 10
Calcular n/r**2
Si r**2 < n
Repetir para r = r + 1 
Sino calcular dif = n-r**2
Si dif = 0 
raíz cuadrada de n es r
Sino calcular m = (r*2*e1 + d)*d 
Contar cuántos valores tiene m len(m)
Calcular v = dif*e**(len(m)-1) - m
Repetir para d+1 mientras v <= m
raíz cuadrada de n es r.d
Fin

```

Diagrama de flujo:

[![](https://mermaid.ink/img/pako:eNp1UsFy0zAQ_ZUdnVrXAZKjp4WhCSlpmx4oJ-wcdqwN0SBLZiOHgSSf1K_gx1jFceIe8EWrfW_3Pa13q0qvSWVqaf2vcoUc4OukcCDfx4uZM6XxlzAYvL_NXQbkArGHG3BNFQNNFn42BGuSwxATrNBaZLAIjH9f_kDZoGbUmAL3ykcpaOjdh3I3yy6RQgXnmM7hpgsXrcHbaAzG-Rht2URZ95aTZHRExwd0so0puAYHH_YtMInA7tns4FP-hWoKhqFGFstiheEKhovIGPfZT34H07zshMRtnMKgJzeNvLtti7w7id2dxD7nr0ci0xNTtAZe9KmiNDsLVdFSMkpoKL50oo_UWaTe55YcVMfU_eG5DzmcprGR2minamwwtTUlag-1ZyAgS5t4Qzi0GAyhIufXsEEruBjruj7Ero-vx6SvhG7kTzBKBVzfCDvSZm3JY4zn_33sm-4N88h7upgad6lSJftUodGyiNsIFyqsqKJCZRJq5B-FKtxeeNgE__zblSoL3FCqmlpjoInB74yVypZo15IlbYLnebvZhwVPVY3um_cdZ_8PmY3qxQ?type=png)](https://mermaid.live/edit#pako:eNp1UsFy0zAQ_ZUdnVrXAZKjp4WhCSlpmx4oJ-wcdqwN0SBLZiOHgSSf1K_gx1jFceIe8EWrfW_3Pa13q0qvSWVqaf2vcoUc4OukcCDfx4uZM6XxlzAYvL_NXQbkArGHG3BNFQNNFn42BGuSwxATrNBaZLAIjH9f_kDZoGbUmAL3ykcpaOjdh3I3yy6RQgXnmM7hpgsXrcHbaAzG-Rht2URZ95aTZHRExwd0so0puAYHH_YtMInA7tns4FP-hWoKhqFGFstiheEKhovIGPfZT34H07zshMRtnMKgJzeNvLtti7w7id2dxD7nr0ci0xNTtAZe9KmiNDsLVdFSMkpoKL50oo_UWaTe55YcVMfU_eG5DzmcprGR2minamwwtTUlag-1ZyAgS5t4Qzi0GAyhIufXsEEruBjruj7Ero-vx6SvhG7kTzBKBVzfCDvSZm3JY4zn_33sm-4N88h7upgad6lSJftUodGyiNsIFyqsqKJCZRJq5B-FKtxeeNgE__zblSoL3FCqmlpjoInB74yVypZo15IlbYLnebvZhwVPVY3um_cdZ_8PmY3qxQ)


