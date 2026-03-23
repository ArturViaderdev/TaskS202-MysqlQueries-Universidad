# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 7 correctas de 11 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.41 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.34 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 5: Incorrecto
```diff
--- 
+++ 
@@ -1,7 +1,7 @@
-id | nombre | cuatrimestre | curso | id_grado
-72.00 | Bases moleculares del desarrollo vegetal | 1.00 | 3.00 | 7.00
-73.00 | Fisiología animal | 1.00 | 3.00 | 7.00
-74.00 | Metabolismo y biosíntesis de biomoléculas | 1.00 | 3.00 | 7.00
-75.00 | Operaciones de separación | 1.00 | 3.00 | 7.00
-76.00 | Patología molecular de plantas | 1.00 | 3.00 | 7.00
-77.00 | Técnicas instrumentales básicas | 1.00 | 3.00 | 7.00
+nombre
+Bases moleculares del desarrollo vegetal
+Fisiología animal
+Metabolismo y biosíntesis de biomoléculas
+Operaciones de separación
+Patología molecular de plantas
+Técnicas instrumentales básicas
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.39 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_departamento

---

## ❌ Query 7: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,25 @@
-nombre | anyo_inicio | anyo_fin
-Álgegra lineal y matemática discreta | 2014.00 | 2015.00
-Cálculo | 2014.00 | 2015.00
-Física para informática | 2014.00 | 2015.00
+id | nif | nombre | apellido1 | apellido2 | ciudad | direccion | telefono | fecha_nacimiento | sexo | tipo
+1.00 | 26902806M | Salvador | Sánchez | Pérez | Almería | C/ Real del barrio alto | 950254837 | 1991-03-28 | H | alumno
+2.00 | 89542419S | Juan | Saez | Vega | Almería | C/ Mercurio | 618253876 | 1992-08-08 | H | alumno
+3.00 | 11105554G | Zoe | Ramirez | Gea | Almería | C/ Marte | 618223876 | 1979-08-19 | M | profesor
+4.00 | 17105885A | Pedro | Heller | Pagac | Almería | C/ Estrella fugaz | NULL | 2000-10-05 | H | alumno
+5.00 | 38223286T | David | Schmidt | Fisher | Almería | C/ Venus | 678516294 | 1978-01-19 | H | profesor
+6.00 | 04233869Y | José | Koss | Bayer | Almería | C/ Júpiter | 628349590 | 1998-01-28 | H | alumno
+7.00 | 97258166K | Ismael | Strosin | Turcotte | Almería | C/ Neptuno | NULL | 1999-05-24 | H | alumno
+8.00 | 79503962T | Cristina | Lemke | Rutherford | Almería | C/ Saturno | 669162534 | 1977-08-21 | M | profesor
+9.00 | 82842571K | Ramón | Herzog | Tremblay | Almería | C/ Urano | 626351429 | 1996-11-21 | H | alumno
+10.00 | 61142000L | Esther | Spencer | Lakin | Almería | C/ Plutón | NULL | 1977-05-19 | M | profesor
+11.00 | 46900725E | Daniel | Herman | Pacocha | Almería | C/ Andarax | 679837625 | 1997-04-26 | H | alumno
+12.00 | 85366986W | Carmen | Streich | Hirthe | Almería | C/ Almanzora | NULL | 1971-04-29 | M | profesor
+13.00 | 73571384L | Alfredo | Stiedemann | Morissette | Almería | C/ Guadalquivir | 950896725 | 1980-02-01 | H | profesor
+14.00 | 82937751G | Manolo | Hamill | Kozey | Almería | C/ Duero | 950263514 | 1977-01-02 | H | profesor
+15.00 | 80502866Z | Alejandro | Kohler | Schoen | Almería | C/ Tajo | 668726354 | 1980-03-14 | H | profesor
+16.00 | 10485008K | Antonio | Fahey | Considine | Almería | C/ Sierra de los Filabres | NULL | 1982-03-18 | H | profesor
+17.00 | 85869555K | Guillermo | Ruecker | Upton | Almería | C/ Sierra de Gádor | NULL | 1973-05-05 | H | profesor
+18.00 | 04326833G | Micaela | Monahan | Murray | Almería | C/ Veleta | 662765413 | 1976-02-25 | H | profesor
+19.00 | 11578526G | Inma | Lakin | Yundt | Almería | C/ Picos de Europa | 678652431 | 1998-09-01 | M | alumno
+20.00 | 79221403L | Francesca | Schowalter | Muller | Almería | C/ Quinto pino | NULL | 1980-10-31 | H | profesor
+21.00 | 79089577Y | Juan | Gutiérrez | López | Almería | C/ Los pinos | 678652431 | 1998-01-01 | H | alumno
+22.00 | 41491230N | Antonio | Domínguez | Guerrero | Almería | C/ Cabo de Gata | 626652498 | 1999-02-11 | H | alumno
+23.00 | 64753215G | Irene | Hernández | Martínez | Almería | C/ Zapillo | 628452384 | 1996-03-12 | M | alumno
+24.00 | 85135690V | Sonia | Gea | Ruiz | Almería | C/ Mercurio | 678812017 | 1995-04-13 | M | alumno
```

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.41 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_profesor,id_grado, PRIMARY,id_departamento

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.41 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_curso_escolar

---

## ❌ Query 10: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-departamento | apellido1 | apellido2 | nombre
+nombre | apellido1 | apellido2 | nombre
 Agronomía | Monahan | Murray | Micaela
 Economía y Empresa | Fahey | Considine | Antonio
 Economía y Empresa | Lemke | Rutherford | Cristina
```

⏱ Tiempo: 0.42 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 11: Error
- **Descripción**: 'NoneType' object is not iterable

