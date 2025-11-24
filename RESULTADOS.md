# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 6 correctas de 40 queries

## ❌ Query 1: Error
- **Descripción**: 1146 (42S02): Table 'tienda.productos' doesn't exist


## ✅ Query 2: Correcto

⏱ Tiempo: 0.35 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ❌ Query 4: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,12 @@
 nombre | precio_eur | precio_usd
-Disco duro SATA3 1TB | 86.99 | 86.99
-Memoria RAM DDR4 8GB | 120.00 | 120.00
-Disco SSD 1 TB | 150.99 | 150.99
-GeForce GTX 1050Ti | 185.00 | 185.00
-GeForce GTX 1080 Xtreme | 755.00 | 755.00
-Monitor 24 LED Full HD | 202.00 | 202.00
-Monitor 27 LED Full HD | 245.99 | 245.99
-Portátil Yoga 520 | 559.00 | 559.00
-Portátil Ideapd 320 | 444.00 | 444.00
-Impresora HP Deskjet 3720 | 59.99 | 59.99
-Impresora HP Laserjet Pro M26nw | 180.00 | 180.00
+Disco duro SATA3 1TB | 86.99€ | 86.99$
+Memoria RAM DDR4 8GB | 120€ | 120$
+Disco SSD 1 TB | 150.99€ | 150.99$
+GeForce GTX 1050Ti | 185€ | 185$
+GeForce GTX 1080 Xtreme | 755€ | 755$
+Monitor 24 LED Full HD | 202€ | 202$
+Monitor 27 LED Full HD | 245.99€ | 245.99$
+Portátil Yoga 520 | 559€ | 559$
+Portátil Ideapd 320 | 444€ | 444$
+Impresora HP Deskjet 3720 | 59.99€ | 59.99$
+Impresora HP Laserjet Pro M26nw | 180€ | 180$
```

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 5: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nom del producte | euros | dòlars
+nom_del_producte | euros | dolares
 Disco duro SATA3 1TB | 86.99 | 95.69
 Memoria RAM DDR4 8GB | 120.00 | 132.00
 Disco SSD 1 TB | 150.99 | 166.09
```

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 8: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,10 @@
-nombre | iniciales
-Asus | AS
-Lenovo | LE
-Hewlett-Packard | HE
-Samsung | SA
-Seagate | SE
-Crucial | CR
-Gigabyte | GI
-Huawei | HU
-Xiaomi | XI
+nombre | nombre
+Asus | ASus
+Lenovo | LEnovo
+Hewlett-Packard | HEwlett-Packard
+Samsung | SAmsung
+Seagate | SEagate
+Crucial | CRucial
+Gigabyte | GIgabyte
+Huawei | HUawei
+Xiaomi | XIaomi
```

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 9: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | precio
+nombre | ROUND(precio)
 Disco duro SATA3 1TB | 87.00
 Memoria RAM DDR4 8GB | 120.00
 Disco SSD 1 TB | 151.00
```

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 10: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | precio truncado
+nombre | truncate(precio, 0)
 Disco duro SATA3 1TB | 86.00
 Memoria RAM DDR4 8GB | 120.00
 Disco SSD 1 TB | 150.00
```

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 11: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 12: Correcto

⏱ Tiempo: 0.30 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ❌ Query 13: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'SELECT DISTINCT nombre 
FROM fabricante
ORDER BY nombre DESC' at line 6


## ❌ Query 14: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,12 @@
-nombre
-Xiaomi
-Seagate
-Samsung
-Lenovo
-Huawei
-Hewlett-Packard
-Gigabyte
-Crucial
-Asus
+nombre | precio
+Disco duro SATA3 1TB | 86.99
+Disco SSD 1 TB | 150.99
+GeForce GTX 1050Ti | 185.00
+GeForce GTX 1080 Xtreme | 755.00
+Impresora HP Deskjet 3720 | 59.99
+Impresora HP Laserjet Pro M26nw | 180.00
+Memoria RAM DDR4 8GB | 120.00
+Monitor 24 LED Full HD | 202.00
+Monitor 27 LED Full HD | 245.99
+Portátil Ideapd 320 | 444.00
+Portátil Yoga 520 | 559.00
```

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 15: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,6 @@
-nombre | precio
-Disco duro SATA3 1TB | 86.99
-Disco SSD 1 TB | 150.99
-GeForce GTX 1050Ti | 185.00
-GeForce GTX 1080 Xtreme | 755.00
-Impresora HP Deskjet 3720 | 59.99
-Impresora HP Laserjet Pro M26nw | 180.00
-Memoria RAM DDR4 8GB | 120.00
-Monitor 24 LED Full HD | 202.00
-Monitor 27 LED Full HD | 245.99
-Portátil Ideapd 320 | 444.00
-Portátil Yoga 520 | 559.00
+codigo | nombre
+1.00 | Asus
+2.00 | Lenovo
+3.00 | Hewlett-Packard
+4.00 | Samsung
+5.00 | Seagate
```

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ❌ Query 16: Incorrecto
```diff
--- 
+++ 
@@ -1,6 +1,3 @@
 codigo | nombre
-1.00 | Asus
-2.00 | Lenovo
-3.00 | Hewlett-Packard
 4.00 | Samsung
 5.00 | Seagate
```

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ❌ Query 17: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,6 @@
-codigo | nombre
-4.00 | Samsung
-5.00 | Seagate
+nombre | precio
+Impresora HP Deskjet 3720 | 59.99
+Disco duro SATA3 1TB | 86.99
+Memoria RAM DDR4 8GB | 120.00
+Disco SSD 1 TB | 150.99
+Impresora HP Laserjet Pro M26nw | 180.00
```

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 18: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,6 @@
 nombre | precio
-Impresora HP Deskjet 3720 | 59.99
+GeForce GTX 1080 Xtreme | 755.00
+Portátil Yoga 520 | 559.00
+Portátil Ideapd 320 | 444.00
+Monitor 27 LED Full HD | 245.99
+Monitor 24 LED Full HD | 202.00
```

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 19: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,3 @@
-nombre | precio
-GeForce GTX 1080 Xtreme | 755.00
+nombre
+Portátil Yoga 520
+Portátil Ideapd 320
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 20: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,12 @@
-nombre
-Portátil Yoga 520
-Portátil Ideapd 320
+nombre_producto | precio_producto | nombre_del_fabricante
+Disco duro SATA3 1TB | 86.99 | Seagate
+Memoria RAM DDR4 8GB | 120.00 | Crucial
+Disco SSD 1 TB | 150.99 | Samsung
+GeForce GTX 1050Ti | 185.00 | Gigabyte
+GeForce GTX 1080 Xtreme | 755.00 | Crucial
+Monitor 24 LED Full HD | 202.00 | Asus
+Monitor 27 LED Full HD | 245.99 | Asus
+Portátil Yoga 520 | 559.00 | Lenovo
+Portátil Ideapd 320 | 444.00 | Lenovo
+Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
+Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
```

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 21: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,12 @@
-nombre | precio | nombre del fabricante
-Disco duro SATA3 1TB | 86.99 | Seagate
-Memoria RAM DDR4 8GB | 120.00 | Crucial
-Disco SSD 1 TB | 150.99 | Samsung
-GeForce GTX 1050Ti | 185.00 | Gigabyte
-GeForce GTX 1080 Xtreme | 755.00 | Crucial
+nombre_producto | precio_producto | nombre_del_fabricante
 Monitor 24 LED Full HD | 202.00 | Asus
 Monitor 27 LED Full HD | 245.99 | Asus
+Memoria RAM DDR4 8GB | 120.00 | Crucial
+GeForce GTX 1080 Xtreme | 755.00 | Crucial
+GeForce GTX 1050Ti | 185.00 | Gigabyte
+Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
+Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
 Portátil Yoga 520 | 559.00 | Lenovo
 Portátil Ideapd 320 | 444.00 | Lenovo
-Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
-Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
+Disco SSD 1 TB | 150.99 | Samsung
+Disco duro SATA3 1TB | 86.99 | Seagate
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 22: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,12 @@
-nombre | precio | nombre del fabricante
-Monitor 24 LED Full HD | 202.00 | Asus
-Monitor 27 LED Full HD | 245.99 | Asus
-Memoria RAM DDR4 8GB | 120.00 | Crucial
-GeForce GTX 1080 Xtreme | 755.00 | Crucial
-GeForce GTX 1050Ti | 185.00 | Gigabyte
-Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
-Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
-Portátil Yoga 520 | 559.00 | Lenovo
-Portátil Ideapd 320 | 444.00 | Lenovo
-Disco SSD 1 TB | 150.99 | Samsung
-Disco duro SATA3 1TB | 86.99 | Seagate
+codigo_producto | nombre_del_producto | codigo_fabricante | nombre_del_fabricante
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

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 23: Incorrecto
```diff
--- 
+++ 
@@ -1,12 +1,2 @@
-codigo | nombre | codigo fabricante | nombre fabricante
-1.00 | Disco duro SATA3 1TB | 5.00 | Seagate
-2.00 | Memoria RAM DDR4 8GB | 6.00 | Crucial
-3.00 | Disco SSD 1 TB | 4.00 | Samsung
-4.00 | GeForce GTX 1050Ti | 7.00 | Gigabyte
-5.00 | GeForce GTX 1080 Xtreme | 6.00 | Crucial
-6.00 | Monitor 24 LED Full HD | 1.00 | Asus
-7.00 | Monitor 27 LED Full HD | 1.00 | Asus
-8.00 | Portátil Yoga 520 | 2.00 | Lenovo
-9.00 | Portátil Ideapd 320 | 2.00 | Lenovo
-10.00 | Impresora HP Deskjet 3720 | 3.00 | Hewlett-Packard
-11.00 | Impresora HP Laserjet Pro M26nw | 3.00 | Hewlett-Packard
+nombre | precio | nombre
+Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
```

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 24: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
-nombre | precio | fabricant
-Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
+nombre | precio | nombre
+GeForce GTX 1080 Xtreme | 755.00 | Crucial
```

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 25: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,3 @@
-nombre | precio | fabricante
-GeForce GTX 1080 Xtreme | 755.00 | Crucial
+nombre | precio
+Portátil Yoga 520 | 559.00
+Portátil Ideapd 320 | 444.00
```

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 26: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,2 @@
 nombre | precio
-Portátil Yoga 520 | 559.00
-Portátil Ideapd 320 | 444.00
+GeForce GTX 1080 Xtreme | 755.00
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 27: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,6 @@
-nombre | precio
-GeForce GTX 1080 Xtreme | 755.00
+nombre | precio | nombre
+Disco duro SATA3 1TB | 86.99 | Seagate
+Monitor 24 LED Full HD | 202.00 | Asus
+Monitor 27 LED Full HD | 245.99 | Asus
+Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
+Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 28: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | precio | fabricante
+nombre | precio | nombre
 Disco duro SATA3 1TB | 86.99 | Seagate
 Monitor 24 LED Full HD | 202.00 | Asus
 Monitor 27 LED Full HD | 245.99 | Asus
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

🚨 **Problemas detectados:**
⚠️ Considerar `EXISTS` en lugar de `IN` para eficiencia.

---

## ❌ Query 29: Incorrecto
```diff
--- 
+++ 
@@ -1,6 +1,3 @@
-nombre | precio | fabricante
+nombre | precio | nombre
 Disco duro SATA3 1TB | 86.99 | Seagate
-Monitor 24 LED Full HD | 202.00 | Asus
-Monitor 27 LED Full HD | 245.99 | Asus
-Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
-Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
+GeForce GTX 1050Ti | 185.00 | Gigabyte
```

⏱ Tiempo: 0.37 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 30: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,3 @@
-nombre | precio | fabricante
-Disco duro SATA3 1TB | 86.99 | Seagate
-GeForce GTX 1050Ti | 185.00 | Gigabyte
+nombre | precio | nombre
+Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
+Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
```

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 31: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,8 @@
-nombre | precio | fabricante
-Impresora HP Deskjet 3720 | 59.99 | Hewlett-Packard
+nombre | precio | nombre
+GeForce GTX 1080 Xtreme | 755.00 | Crucial
+Portátil Yoga 520 | 559.00 | Lenovo
+Portátil Ideapd 320 | 444.00 | Lenovo
+Monitor 27 LED Full HD | 245.99 | Asus
+Monitor 24 LED Full HD | 202.00 | Asus
+GeForce GTX 1050Ti | 185.00 | Gigabyte
 Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 32: Incorrecto
```diff
--- 
+++ 
@@ -1,8 +1,8 @@
-nombre | precio | fabricante
-GeForce GTX 1080 Xtreme | 755.00 | Crucial
-Portátil Yoga 520 | 559.00 | Lenovo
-Portátil Ideapd 320 | 444.00 | Lenovo
-Monitor 27 LED Full HD | 245.99 | Asus
-Monitor 24 LED Full HD | 202.00 | Asus
-GeForce GTX 1050Ti | 185.00 | Gigabyte
-Impresora HP Laserjet Pro M26nw | 180.00 | Hewlett-Packard
+codigo | nombre
+1.00 | Asus
+2.00 | Lenovo
+3.00 | Hewlett-Packard
+4.00 | Samsung
+5.00 | Seagate
+6.00 | Crucial
+7.00 | Gigabyte
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

---

## ❌ Query 33: Incorrecto
```diff
--- 
+++ 
@@ -1,8 +1,14 @@
-codigo | nombre
-1.00 | Asus
-2.00 | Lenovo
-3.00 | Hewlett-Packard
-4.00 | Samsung
-5.00 | Seagate
-6.00 | Crucial
-7.00 | Gigabyte
+nombre_fabricante | nombre_producto
+Asus | Monitor 27 LED Full HD
+Asus | Monitor 24 LED Full HD
+Lenovo | Portátil Ideapd 320
+Lenovo | Portátil Yoga 520
+Hewlett-Packard | Impresora HP Laserjet Pro M26nw
+Hewlett-Packard | Impresora HP Deskjet 3720
+Samsung | Disco SSD 1 TB
+Seagate | Disco duro SATA3 1TB
+Crucial | GeForce GTX 1080 Xtreme
+Crucial | Memoria RAM DDR4 8GB
+Gigabyte | GeForce GTX 1050Ti
+Huawei | NULL
+Xiaomi | NULL
```

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ❌ Query 34: Incorrecto
```diff
--- 
+++ 
@@ -1,14 +1,3 @@
-fabricante | producto
-Asus | Monitor 27 LED Full HD
-Asus | Monitor 24 LED Full HD
-Lenovo | Portátil Ideapd 320
-Lenovo | Portátil Yoga 520
-Hewlett-Packard | Impresora HP Laserjet Pro M26nw
-Hewlett-Packard | Impresora HP Deskjet 3720
-Samsung | Disco SSD 1 TB
-Seagate | Disco duro SATA3 1TB
-Crucial | GeForce GTX 1080 Xtreme
-Crucial | Memoria RAM DDR4 8GB
-Gigabyte | GeForce GTX 1050Ti
-Huawei | NULL
-Xiaomi | NULL
+nombre_fabricante
+Huawei
+Xiaomi
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ❌ Query 35: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,3 @@
-fabricante
-Huawei
-Xiaomi
+codigo | nombre | precio | codigo_fabricante
+8.00 | Portátil Yoga 520 | 559.00 | 2.00
+9.00 | Portátil Ideapd 320 | 444.00 | 2.00
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ❌ Query 36: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,2 @@
 codigo | nombre | precio | codigo_fabricante
 8.00 | Portátil Yoga 520 | 559.00 | 2.00
-9.00 | Portátil Ideapd 320 | 444.00 | 2.00
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante, PRIMARY

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ❌ Query 37: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
-codigo | nombre | precio | codigo_fabricante
-8.00 | Portátil Yoga 520 | 559.00 | 2.00
+nombre_producto
+Portátil Yoga 520
```

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ❌ Query 38: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
-nombre
-Portátil Yoga 520
+nombre_producto
+Impresora HP Deskjet 3720
```

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---

## ❌ Query 39: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,3 @@
-nombre
-Impresora HP Deskjet 3720
+codigo | nombre | precio | codigo_fabricante
+5.00 | GeForce GTX 1080 Xtreme | 755.00 | 6.00
+8.00 | Portátil Yoga 520 | 559.00 | 2.00
```

⏱ Tiempo: 0.39 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ❌ Query 40: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,2 @@
 codigo | nombre | precio | codigo_fabricante
-5.00 | GeForce GTX 1080 Xtreme | 755.00 | 6.00
-8.00 | Portátil Yoga 520 | 559.00 | 2.00
+7.00 | Monitor 27 LED Full HD | 245.99 | 1.00
```

⏱ Tiempo: 0.40 ms
✅ Se usó índice(s) en la consulta: codigo_fabricante

---
