# Nitrox

A FO2 do Nitrox representa o valor em percentagem de O2 numa data mistura.

## Fórmula:  PO2 = Pdesejada * ( (Fdesejada - Ftop-off) / (Fenchimento - Ftop-off) ) , em que:

### PO2 - Pressão de Oxigénio puro no enchimento
### Pdesejada - Pressão final da garrafa pós enchimento
### Fdesejada - Fração oxigénio que queremos obter no produto do enchimento
### Ftop-off - Fração oxigénio presente no gás do top-off (.21 no caso do ar)
### Fenchimento - Fração oxigénio presente no gás do enchimento do oxigénio (1 no caso do oxigénio puro)


## Sabemos também que a pressão total é igual ao somatório das pressões parciais.
Assim: Ptotal = PmixExistente + PmixBlend
### Ptotal - Pressão total no enchimento
### PmixExistente - Pressão do mix existente na garrafa
### PmixBlend - Pressão do mix a fazer blend



### Questão: Como calcular quantos bares de O2 necessários para enchimento de 200 bar EANX 32?
Assumir garrafa com 50 bar ar
Assumir TOP OFF a ar

 ---
(   )
|***|
|***|Top-Off a ar
|???|O2 puro a adicionar
|???|
|###|50 bar EAN21
|###|

## Resposta requer dois passos:
### 1 - Qual o nitrox a produzir nos 150 bares restantes para o enchimento?
### 2 - Como o fazer?

1 - Qual o nitrox a produzir?
Ptotal = PmixExistente + PmixBlend

200 * 0.32 = 50 * 0.21 + (200-50) X
64 = 10.5 + 150X
-150X = 10.5 - 64
-150X = -53.5
X = -53.5 / -150
X = **0.36, esta é a F02 do nitrox a produzir.**


2 - Como fazer 150 bares de nitrox 36?
PO2 = Pdesejada * ( (Fdesejada - Ftop-off) / (Fenchimento - Ftop-off) )

P02 = 150 * ( (0.36 - 0.21) / (1 - 021) )

PO2 = 150 + ( 0.15 / 0.79)

PO2 = 150 * 0.19

PO2 = **29 bar de O2 seguido de top off a ar.**

Resultado:
 ---
(   )
|***|
|***|Top-Off a ar
|+++|29 bar O2
|+++|
|###|50 bar EAN21
|###|