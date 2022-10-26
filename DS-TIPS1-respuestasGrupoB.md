# Bienvenidos a los TIP's. <br>
## Usa este espacio como un lugar de repaso. Esto servirá para tus entrevistas laborales asi que ¡actúa como si estuvieras en una! Comencemos.  
<br>

### **1) Explique la diferencia entre la cláusula WHERE y la cláusula HAVING.**
<br>
La cláusula WHERE es utilizada para aplicar condiciones/filtros ANTES de aplicar cualquier agregación (o cuando no se aplique ninguna)
La cláusula HAVING es usada para aplicar condiciones/filtros DESPUÉS de dar lugar a la agregación. 

<br>

### **2) ¿Para qué se usan break, continue y pass en python?**
<br>
Break: finaliza un bucle (loop), continuando con las sentencias que le siguen a éste.
Continue: finaliza la iteración en la que se encuentre dentro del bucle, omite lo que le sigue dentro de ésta iteración y continúa a la siguiente.
Pass: es una declaración nula, suele ser usada de forma momentánea en funciones y bucles vacíos. El programa no ignora esta declaración, pero no sucede nada cuando ésta se ejecuta.

<br>

### **3) En un estante hay 10 tazas: 5 rojas, 3 azules y 2 amarillas. Se realiza una selección al azar. ¿Cuál es la probabilidad de:**
**a) Elegir una taza amarilla**<br>

P(A) = exito_amarillas / Casos_posibles (2/10) = 0.2<br> 

**b) Elegir dos tazas rojas, si no hay reposición**<br>
P(2R) = 5/10 * 4/9 = 0.22

<br>

## Suponga tiene la tabla HITS compuesta de la siguiente forma:

| ID_Cancion | Año | Artista |
|--------|--------|----|
| valor | valor | valor |
|valor  | valor  | valor |

### **4) Cree una consulta SQL que obtenga de la tabla HITS, canciones cuyo AÑO de publicación esté entre  1970 y 1980 (ambos años incluídos).**
<br>
SELECT<br>
&emsp;ID_cancion,<br>
&emsp;Año<br>
FROM<br>
&emsp;HITS<br>    
WHERE<br>
&emsp;Año BETWEEN 1970 AND 1980;<br>
<br>    
### **5) Obtener los 5 artistas con mayor cantidad de canciones**  
<br>

SELECT<br> 
&emsp;Artista<br>
&emsp;COUNT(ID_Cancion) AS N_cancion,<br>
FROM<br> 
&emsp;HITS<br>
GROUP BY<br> 
&emsp;Artista<br>
ORDER BY<br> 
&emsp;COUNT(ID_Cancion) DESC<br>
LIMIT 5;<br>

<br>


# Recuerda que no deberías poder usar Google. 
![img](https://thumbs.gfycat.com/KaleidoscopicFaintHind-size_restricted.gif)
## ¡Exitos!
