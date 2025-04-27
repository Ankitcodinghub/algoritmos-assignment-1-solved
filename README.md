# algoritmos-assignment-1-solved
**TO GET THIS SOLUTION VISIT:** [Algoritmos Assignment 1 Solved](https://www.ankitcodinghub.com/product/algoritmos-grado-en-ingenieria-informatica-solved-3/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117860&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Algoritmos Assignment 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
Práctica 1

Suma de la subsecuencia máxima: Dados n números enteros a1,a2,…,an, encontrar el valor máximo de ∑kj=i ak con 1 ≤ i ≤ j ≤ n (por conveniencia, la suma de la subsecuencia máxima es 0 si todos los enteros son negativos).

Se proponen dos algoritmos para resolver este problema:

Algoritmo 1: O(n2)

función sumaSubMax1 (v[1..n]) sumaMax := 0 ; para i := 1 hasta n hacer estaSuma := 0 ; para j := i hasta n hacer estaSuma := estaSuma + v[j] ; si estaSuma &gt; sumaMax entonces sumaMax := estaSuma fin si

fin para

fin para ;

devolver sumaMax

fin función

Algoritmo 2: O(n)

función sumaSubMax2 (v[1..n]) estaSuma := 0 ; sumaMax :=0 ; para j := 1 hasta n hacer estaSuma := estaSuma + v[j] ; si estaSuma &gt; sumaMax entonces sumaMax := estaSuma

sino si estaSuma &lt; 0 entonces estaSuma := 0

fin si

fin para ;

devolver sumaMax

fin función

Se pide:

1. Implemente en C los algoritmos propuestos (véase la figura 5).

2. Valide que los algoritmos funcionan correctamente. Chequee las siguientes secuencias:

secuencia resultado

-9, 2, -5, -4, 6 6

4, 0, 9, 2, 5 20

-2, -1, -9, -7, -1 0

9, -2, 1, -7, -8 9

15, -2, -5, -4, 16 20

7, -5, 6, 7, -7 15

Así mismo realice una segunda comprobación con vectores generados de forma aleatoria (figura 1) comprobando que ambos algoritmos devuelven el mismo resultado (figura 2).

void inicializar_semilla() {

srand(time(NULL));

/* se establece la semilla de una nueva serie de enteros pseudo-aleatorios */

} void aleatorio(int v [], int n) {

int i, m=2*n+1; for (i=0; i &lt; n; i++)

v[i] = (rand() % m) – n;

/* se generan números pseudoaleatorio entre -n y +n */

}

Figura 1: Inicialización de un vector con números pseudoaleatorios en el rango [−n,…,+n]

sumaSubMax1 sumaSubMax2

[ 7 0 -3 3 -1 1 -5 5 -8 ] 7 7

[ -8 8 1 -1 7 6 -5 -4 -7 ] 21 21

[ -1 -7 -8 -6 7 -2 1 -2 -7 ] 7 7

[ 8 -3 8 9 -9 -5 -4 3 1 ] 22 22

[ 3 8 -4 5 6 -9 -4 -8 7 ] 18 18

[ 9 -6 -6 8 2 -7 -9 5 9 ] 14 14

[ -5 -7 -6 -3 -8 -3 -5 -9 -3 ] 0 0

[ -3 -7 -9 7 6 5 -7 -2 -2 ] 18 18

[ -7 0 0 7 -1 3 -9 -5 -8 ] 9 9

[ 9 -5 3 8 -1 6 9 3 4 ] 36 36

Figura 2: Aplicadas sobre distintos vectores aleatorios, ambas funciones devuelven el mismo resultados.

3. Para cada uno de los dos algoritmos, determine los tiempos de ejecución con vectores aleatoriosde tamaño n igual a 500,1000,2000,4000,8000,16000 y 32000. Use el código de la figura 3 para obtener la hora del sistema. Para generar los datos de prueba utilice el código de la figura 1 que genera vectores de números pseudoaleatorios en el rango [−n,…,n].

#include &lt;sys/time.h&gt; double microsegundos() { /* obtiene la hora del sistema en microsegundos */

struct timeval t; if (gettimeofday(&amp;t, NULL) &lt; 0 )

return 0.0;

return (t.tv_usec + t.tv_sec * 1000000.0);

}

Figura 3: Obtención de la hora del sistema

4. Analice los resultados obtenidos realizando una comprobación empírica de la complejidad teórica (figura 4). Igualmente se realizará una comprobación empírica utilizando una cota subestimada y otra sobre-estimada para cada algoritmo.

$ ./p1

SumaSubMax 1

n t(n) t(n)/n^1.8 t(n)/n^2 t(n)/n^2.2

(*) 500 341.666 0.004736 0.001367 0.000394

1000 1200.000 0.004777 0.001200 0.000301

2000 4819.000 0.005509 0.001205 0.000263

4000 19178.000 0.006296 0.001199 0.000228

8000 85178.000 0.008031 0.001331 0.000221

16000 332606.000 0.009006 0.001299 0.000187

32000 1270463.000 0.009879 0.001241 0.000156

Figura 4: Parte de la posible salida por pantalla del programa que mide los tiempos de ejecución del primer algoritmo.

5. Entregue los ficheros con el código C y el fichero .txt con el informe por medio de la tarea

Entrega Práctica 1 en la página de Algoritmos en https://campusvirtual.udc.gal. Se recuerda que el límite para completar la tarea es el sábado 25 de septiembre a las 23:59, y una vez subidos los archivos no se podrán cambiar. Todos los compañeros que forman un equipo tienen que entregar el trabajo.

#include &lt;stdio.h&gt; int sumaSubMax1(int v[], int n) {

int i, j; int estaSuma, sumaMax = 0; for (i = 0; i &lt; n; i++) { estaSuma = 0; for (j = i; j &lt; n; j++) { estaSuma += v[j]; if (estaSuma &gt; sumaMax) {

sumaMax = estaSuma;

}

} } return sumaMax;

} int sumaSubMax2(int v[], int n) {

/* … */

} void listar_vector(int v[], int n){

/* … */

} void test1() {

/* … */

} void test2() { int i, a, b; int v[9]; printf(“test “); printf(“%33s%15s%15s “, “”, “sumaSubMax1”, “sumaSubMax2”); for (i=0; i&lt;10; i++) { aleatorio(v, 9); listar_vector(v, 9); a = sumaSubMax1(v, 9); b = sumaSubMax2(v, 9); printf(“%15d%15d “, a, b);

}

} int main() { inicializar_semilla(); test1(); test2(); return 0;

}

Figura 5: Código con la función sumaSubMax1 y el segundo test
