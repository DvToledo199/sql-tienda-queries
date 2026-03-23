# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 16 correctas de 28 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.42 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 5: Error
- **Descripción**: 1582 (42000): Incorrect parameter count in the call to native function 'ROUND'


## ❌ Query 6: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'FROM producto' at line 3


## ❌ Query 7: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'FROM producto' at line 3


## ✅ Query 8: Correcto

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 10: Error
- **Descripción**: 1054 (42S22): Unknown column 'numero' in 'field list'


## ✅ Query 11: Correcto

⏱ Tiempo: 0.45 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 12: Correcto

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ✅ Query 13: Correcto

⏱ Tiempo: 0.32 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 14: Correcto

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 15: Correcto

⏱ Tiempo: 0.34 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 16: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 17: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 18: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 19: Correcto

⏱ Tiempo: 0.32 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 20: Correcto

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ❌ Query 21: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | precio | nombre del fabricante
+nombre | precio | nombre
 Disco duro SATA3 1TB | 86.99 | Seagate
 Memoria RAM DDR4 8GB | 120.00 | Crucial
 Disco SSD 1 TB | 150.99 | Samsung
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: PRIMARY, codigo_fabricante

---

## ❌ Query 22: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,12 @@
-nombre | precio | nombre del fabricante
+nombre | precio | nombre
+Disco duro SATA3 1TB | 86.99 | Seagate
+Memoria RAM DDR4 8GB | 120.00 | Crucial
+Disco SSD 1 TB | 150.99 | Samsung
+GeForce GTX 1050Ti | 185.00 | Gigabyte
+GeForce GTX 1080 Xtreme | 755.00 | Crucial
 Monitor 24 LED Full HD | 202.00 | Asus
 Monitor 27 LED Full HD | 245.99 | Asus
-Memoria RAM DDR4 8GB | 120.00 | Crucial
-GeForce GTX 1080 Xtreme | 755.00 | Crucial
-GeForce GTX 1050Ti | 185.00 | Gigabyte
+Portátil Yoga 520 | 559.00 | Lenovo
+Portátil Ideapd 320 | 444.00 | Lenovo
 Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
 Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
-Portátil Yoga 520 | 559.00 | Lenovo
-Portátil Ideapd 320 | 444.00 | Lenovo
-Disco SSD 1 TB | 150.99 | Samsung
-Disco duro SATA3 1TB | 86.99 | Seagate
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: PRIMARY, codigo_fabricante

---

## ❌ Query 23: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'ORDER BY producto.nombre' at line 1


## ❌ Query 24: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,12 @@
-nombre | precio | fabricant
-Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
+codigo | nombre | codigo_fabricante | nombre_fabricante
+1.00 | Disco duro SATA3 1TB | 5.00 | Seagate
+2.00 | Memoria RAM DDR4 8GB | 6.00 | Crucial
+3.00 | Disco SSD 1 TB | 4.00 | Samsung
+4.00 | GeForce GTX 1050Ti | 7.00 | Gigabyte
+5.00 | GeForce GTX 1080 Xtreme | 6.00 | Crucial
+6.00 | Monitor 24 LED Full HD | 1.00 | Asus
+7.00 | Monitor 27 LED Full HD | 1.00 | Asus
+8.00 | Portátil Yoga 520 | 2.00 | Lenovo
+9.00 | Portátil Ideapd 320 | 2.00 | Lenovo
+10.00 | Impresora HP Deskjet 3720 | 3.00 | Hewlett-Packard
+11.00 | Impresora HP Laserjet Pro M26nw | 3.00 | Hewlett-Packard
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: PRIMARY, codigo_fabricante

---

## ❌ Query 25: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
 nombre | precio | fabricante
-GeForce GTX 1080 Xtreme | 755.00 | Crucial
+Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
```

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: PRIMARY, codigo_fabricante

---

## ❌ Query 26: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,2 @@
-nombre | precio
-Portátil Yoga 520 | 559.00
-Portátil Ideapd 320 | 444.00
+nombre | precio | fabricante
+GeForce GTX 1080 Xtreme | 755.00 | Crucial
```

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: PRIMARY, codigo_fabricante

---

## ❌ Query 27: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,3 @@
 nombre | precio
-GeForce GTX 1080 Xtreme | 755.00
+Portátil Yoga 520 | 559.00
+Portátil Ideapd 320 | 444.00
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: PRIMARY, codigo_fabricante

---

## ❌ Query 28: Error
- **Descripción**: 'NoneType' object is not iterable

