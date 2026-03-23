# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 12 correctas de 22 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.48 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.34 ms
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

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.44 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, PRIMARY

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

⏱ Tiempo: 0.43 ms
✅ Se usó índice(s) en la consulta: id_profesor,id_grado, PRIMARY,id_departamento, PRIMARY

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.44 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_curso_escolar, PRIMARY

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

⏱ Tiempo: 0.41 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 11: Incorrecto
```diff
--- 
+++ 
@@ -1 +1,25 @@
-apellido1 | apellido2 | nombre
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

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 12: Correcto

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ❌ Query 13: Incorrecto
```diff
--- 
+++ 
@@ -1,11 +1,11 @@
 apellido1 | apellido2 | nombre
 Schmidt | Fisher | David
-Kohler | Schoen | Alejandro
 Lemke | Rutherford | Cristina
-Fahey | Considine | Antonio
 Spencer | Lakin | Esther
 Streich | Hirthe | Carmen
+Stiedemann | Morissette | Alfredo
+Kohler | Schoen | Alejandro
+Fahey | Considine | Antonio
 Ruecker | Upton | Guillermo
 Monahan | Murray | Micaela
-Stiedemann | Morissette | Alfredo
 Schowalter | Muller | Francesca
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: id_profesor

---

## ❌ Query 14: Incorrecto
```diff
--- 
+++ 
@@ -1,63 +1,25 @@
-id | nombre
-22.00 | Ingeniería de Requisitos
-23.00 | Integración de las Tecnologías de la Información en las Organizaciones
-24.00 | Modelado y Diseño del Software 1
-25.00 | Multiprocesadores
-26.00 | Seguridad y cumplimiento normativo
-27.00 | Sistema de Información para las Organizaciones
-28.00 | Tecnologías web
-29.00 | Teoría de códigos y criptografía
-30.00 | Administración de bases de datos
-31.00 | Herramientas y Métodos de Ingeniería del Software
-32.00 | Informática industrial y robótica
-33.00 | Ingeniería de Sistemas de Información
-34.00 | Modelado y Diseño del Software 2
-35.00 | Negocio Electrónico
-36.00 | Periféricos e interfaces
-37.00 | Sistemas de tiempo real
-38.00 | Tecnologías de acceso a red
-39.00 | Tratamiento digital de imágenes
-40.00 | Administración de redes y sistemas operativos
-41.00 | Almacenes de Datos
-42.00 | Fiabilidad y Gestión de Riesgos
-43.00 | Líneas de Productos Software
-44.00 | Procesos de Ingeniería del Software 1
-45.00 | Tecnologías multimedia
-46.00 | Análisis y planificación de las TI
-47.00 | Desarrollo Rápido de Aplicaciones
-48.00 | Gestión de la Calidad y de la Innovación Tecnológica
-49.00 | Inteligencia del Negocio
-50.00 | Procesos de Ingeniería del Software 2
-51.00 | Seguridad Informática
-52.00 | Biologia celular
-53.00 | Física
-54.00 | Matemáticas I
-55.00 | Química general
-56.00 | Química orgánica
-57.00 | Biología vegetal y animal
-58.00 | Bioquímica
-59.00 | Genética
-60.00 | Matemáticas II
-61.00 | Microbiología
-62.00 | Botánica agrícola
-63.00 | Fisiología vegetal
-64.00 | Genética molecular
-65.00 | Ingeniería bioquímica
-66.00 | Termodinámica y cinética química aplicada
-67.00 | Biorreactores
-68.00 | Biotecnología microbiana
-69.00 | Ingeniería genética
-70.00 | Inmunología
-71.00 | Virología
-72.00 | Bases moleculares del desarrollo vegetal
-73.00 | Fisiología animal
-74.00 | Metabolismo y biosíntesis de biomoléculas
-75.00 | Operaciones de separación
-76.00 | Patología molecular de plantas
-77.00 | Técnicas instrumentales básicas
-78.00 | Bioinformática
-79.00 | Biotecnología de los productos hortofrutículas
-80.00 | Biotecnología vegetal
-81.00 | Genómica y proteómica
-82.00 | Procesos biotecnológicos
-83.00 | Técnicas instrumentales avanzadas
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

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ❌ Query 15: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,25 @@
-nombre
-Informática
-Matemáticas
-Economía y Empresa
-Educación
-Agronomía
-Química y Física
-Filología
-Derecho
-Biología y Geología
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

⏱ Tiempo: 0.32 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 16: Correcto

⏱ Tiempo: 0.32 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 17: Correcto

⏱ Tiempo: 0.34 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 18: Correcto

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: id_departamento, PRIMARY

---

## ✅ Query 19: Correcto

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ❌ Query 20: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-grau | total
+nombre | total
 Grado en Ingeniería Informática (Plan 2015) | 51.00
 Grado en Biotecnología (Plan 2015) | 32.00
 Grado en Ingeniería Agrícola (Plan 2015) | 0.00
```

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 21: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '--pendent
SELECT g.nombre,COUNT(a.id) AS total FROM grado AS g LEFT JOIN asignat' at line 2


## ❌ Query 22: Error
- **Descripción**: 'NoneType' object is not iterable

