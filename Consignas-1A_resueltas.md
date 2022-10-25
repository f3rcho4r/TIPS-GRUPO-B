# Bienvenidos a los TIP's. Usa este espacio como un lugar de repaso. Esto servirá para tus entrevistas laborales asi que ¡actúa como que estuvieras en una!.  

<br>

### **1) Especificar la diferencia entre variables locales y globales en python.**  
<br>
Respuesta Esperdada : Las VARIABLES GLOBALES son las declaradas fuera de una función. Todas las funciones del código pueden acceder a dicha variables.
<br>
                     En cambio, las VARIABLES LOCALES son aquellas creadas dentro de las funciones. Intentar acceder a ellas fuera de la función devolverá una falla del sistema. 

<br>


### **2) ¿Cuál es la diferencia entre la funcion .loc y .iloc de pandas?.**
<br>
Respuesta Esperada: Ambas funciones sirver para acceder a filas y columnas de un DataFrame pero la funcion .loc puede recibir como parametro los nombres de las columnas
<br>
                    En cambio la funcion .iloc recibe unicamente numeros

<br>


### **3) Suponiendo que A y B son dos sucesos independientes con P(A) = 0,2 y P(B) = 0,3, ¿cuál es la probabilidad de que:**  

<br>

a)  ambos ocurran? 

<br>

b) al menos uno ocurra?   

<br>

c) exactamente uno ocurra?   

<br>

Respuesta Esperada: a) P(AyB) = P(A) * P(B) = 0.2 * 0.3
                                            = 0.06

<br>
                    b) P(AUB) = P(A) + P(B) - P(AyB) = 0.2 + 0.3 - 0.06
                                                     = 0.44

<br>
                    c) P(AUB) = P(A) + P(B) - 2 * P(AyB) = 0.2 + 0.3 - 0.12
                                                         = 0.38

<br>


## Suponga tiene la tabla CIUDADES compuesta de la siguiente forma:

| IDCiudad | Ciudad | Estado |
|--------|--------|--------|
| valor | valor | valor |
|valor  | valor  | valor |

### **4) Cree una consulta SQL que obtenga los estados sin repeticiones**
<br>
Respuesta Esperada : SELECT DISTINCT estado 
                     FROM ciudades;

<br>

### **5) Obtener todos los datos de las ciudades pertenecientes a los estados "CABA" y "Córdoba"**
<br>
Respuesta Esperada: SELECT *
                    FROM ciudades
                    WHERE estado == "CABA" or estado == "Córdoba";   

<br>
Utilizando IN:         
                    SELECT * 
                    FROM ciudades
                    WHERE estado IN("CABA","CÓRDOBA");

<br>

### **6) Obtener todos los datos de las ciudades que empiecen con la letra "L"**
<br>
Respuesta Esperada: SELECT * 
                    FROM ciudades
                    WHERE ciudad LIKE "L%";



<br>
