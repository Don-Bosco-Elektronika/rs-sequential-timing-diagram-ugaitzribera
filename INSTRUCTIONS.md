# 🛠️ Cronograma de Circuitos Secuenciales / Zirkuitu Sekuentzialen Kronograma / Sequential Circuit Timing Diagram

| **Alumnos** | **Curso** | **Módulo** |
|-------------|-----------|------------|
| 2ME         | 1º        | EEM (Equipos Microprogramables) |

---

## 📌 Ariketa 


**Ariketa (EU): (ZENBAKIA IDATZI)**  
| Izena                     | Txip Zenbakia | Sinboloa         | Funtzionamendu Describapena                                                                |
|---------------------------|------------------|------------------|---------------------------------------------------------------------------------|
| RS | 4044            |  <img width="311" height="222" alt="4044 RS Sinboloa" src="https://github.com/user-attachments/assets/df653832-a4f7-4c4f-9833-ae66496ec6d0" />
| ? |  



## Tabla de la verdad

| Entrada A | Entrada B | Entrada C | Salida    | Salida |
|-----------|-----------|-----------|-----------|--------|
| 0         | 0         | 0         | ░0░       | ░0░    |
| 0         | 0         | 1         | ░1░       | ░1░    |
| 1         | 1         | 0         | ░1░       | ░1░    |
| 1         | 1         | 1         | ░0░       | ░0░    |

----

## 🔲  Simulatzeko Zirkuituak 

<img width="1021" height="556" alt="4044 RS ariketa proteus Ugaitz" src="https://github.com/user-attachments/assets/635c2bfa-03ab-4053-b923-1f6f4fea0fd1" />


---

## 🔲  Kronogramaren Emaitza 
RS Asincrono

<img width="942" height="742" alt="RS asincrono ariketa" src="https://github.com/user-attachments/assets/9612310e-848b-4113-bd28-f2a1b902cb2e" />

RS Flanco ascendente

<img width="960" height="758" alt="RS flanco ascendente ariketa" src="https://github.com/user-attachments/assets/de236d27-afb0-4508-8187-a0c44de2175d" />

RS Flanco descendente

<img width="971" height="686" alt="RS flanco descendente ariketa" src="https://github.com/user-attachments/assets/47c72376-b08b-4770-b486-b2470dae5cc1" />

RS Nivel alto

<img width="962" height="772" alt="RS nivel alto ariketa" src="https://github.com/user-attachments/assets/f5a610ac-ba45-4f93-8ef6-ad8f3ce5e4c2" />

RS Nivel bajo

<img width="937" height="775" alt="RS nivel bajo ariketa" src="https://github.com/user-attachments/assets/aa4e67aa-3a2d-4b2e-a1d6-a7be4b0e0ae9" />



---


## 🔲  Kronogramaren Kodea
RS Asincrono

{signal: [

  {name: 'Set',   wave: 'lhlh..l..h.l.hlh.'},
  
  {name: 'Reset', wave: 'h..l.h.lhlh..l..h'},
  
  {},
  
  {name: 'Q',     wave: '0x.1.x0..1x0.1..x'},
  
  {name: '-Q',    wave: '1x.0.x1..0x1.0..x'}
  
]}


RS Flanco ascendente

{signal: [ 

{name: 'clk', wave: 'P................'},

 {name: 'Set', wave: '0101.0...1.0..1.0'},
 
 {name: 'Reset', wave: '1.0....1010..1..0'},
 
 {},
 
 {name: 'Q', wave: '0x.1...0.x1..0x..'},
 
 {name: '-Q', wave: '1x.0...1.x0..1x..'}
 
]}


RS Flanco descendente

{signal: [ 

{name: 'clk', wave: 'N................'}, 

{name: 'Set', wave: '01.00110.1.1101.0'}, 

{name: 'Reset', wave: '1..010.1010.1..01'}, 

{},

 {name: 'Q', wave: '0xx.01.0.x1.x0x10'},
 
 {name: '-Q', wave: '1xx.10.1.x0.x1x01'}
 
 ]}

 RS Nivel alto

 {signal: [
 
  {name: 'clk',   period: 2, wave: 'p................'},
  
  {name: 'Set',   wave: '010.....1..0..1.0'},
  
  {name: 'Reset', wave: '1.0101010101...01'},
  
  {},
  
  {name: 'Q',     wave: '0x..0...x1..0....'},
  
  {name: '-Q',    wave: '1x..1...x0..1....'}
  
]}

RS Nivel bajo

{signal: [

  {name: 'clk',   period: 2, wave: 'n........'},
  
  {name: 'Set',   wave: '0..1010.1..01010.'},
  
  {name: 'Reset', wave: '1...0..1.0..1..01'},
  
  {},
  
  {name: 'Q',     wave: '0...1..x1..x0....'},
  
  {name: '-Q',    wave: '1...0..x0..x1....'}
  
]}

---


## 📤 Igo  

➡️ **Instrucciones:**  


- **EU:** Igo hurrengo fitxategiak. Igotako fitxategi guztiek zure izena eduki behar dute.  
  - Sinboloaren argazki bat.  
  - Proteus fitxategia eta zirkuitu bakoitzaren irudia (captura) Proteusen.  
  - Wavedrom bakoitzaren emaitzaren kaptura (grafikoa bakarrik).  
  - **KONTUZ:** Kronogramaren kodea kodea izan behar da, ez irudi bat.



