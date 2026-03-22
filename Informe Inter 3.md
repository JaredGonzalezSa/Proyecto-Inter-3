# Informe Proyecto No. 1 Intermedia 3
**Universidad:** Universidad de San Carlos de Guatemala  <br>
**Facultad:** Facultad de Ingeniería  <br>
**Carrera:** Ingeniería en Ciencias y Sistemas  <br>

**Curso:** Matemática Intermedia 3  <br>

**Proyecto No.1** <br>


**Fecha:** 27/03/2026<br>
## Integrantes del equipo

| No | Nombre | Carné | Rol |
|---|---|---|---|
| 1 | Carlos Rolando Barrios Estrada | 202500432 | Coordinador |
| 2 | Nombre integrante | 2025XXXXX | Investigador |
| 3 | Nombre integrante | 2025XXXXX | Diseñador de material |


---
# Introducción
---
# Objetivos
## General:
>Colocar texto<br>

## Específicos:
> 1. Introducción
> 2. Objetivos
> 3. Descripción del tema


---
# Resolución de los problemas

## Problema No. 3
Problema: Con objeto de regular la pesca en los océanos, se han establecido
comisiones internacionales para implementar los controles. Para entender el
efecto de tales controles se han construido modelos matemáticos de poblaciones
de peces. Una etapa en este esfuerzo por crear nuevos modelos incluye la
predicción del crecimiento de un tipo de pez. El modelo de crecimiento de von
Bertalanffy se refleja en la ecuación de Bernoulli.
Dada la ecuación: 
$$\frac{dw}{dt}=\alpha W^{\frac{2}{3}}-\beta W $$
Convertimos esta ecuación diferencial en ecuación diferencial estándar de bernoulli la cual nos queda 
$$\frac{dw}{dt}+\beta W=\alpha W^{\frac{2}{3}} $$
1. Sustitucion
$x=W^{1-\frac{2}{3}} = W^{\frac{1}{3}}$
2. Derivamos 
$\frac{dx}{dt}=\frac{1}{3}W^{\frac{-2}{3}}\frac{dw}{dt}$
3. Despejamos $\frac{dw}{dt}$
$\frac{\frac{dx}{dt}}{\frac{1}{3}W^{\frac{-2}{3}}}=\frac{dw}{dt}$
4. Sustituimos
$\frac{\frac{dx}{dt}}{\frac{1}{3}W^{\frac{-2}{3}}}+\beta W=\alpha W^{\frac{2}{3}}$
5. Multiplicamos por $\frac{1}{3}W^{\frac{-2}{3}}$
6. Obtenemos la nueva ecuación
$\frac{dx}{dt}+\frac{\beta}{3} W^\frac{1}{3}=\frac{\alpha}{3}$
*Sabemos que $X=W^{\frac{1}{3}}$
7. Encontramos el factor de integración
$e^{\int \frac{\beta}{3}\,dt} = e^{\frac{\beta}{3}t}$
8. Multiplicamos por el factor de integracion
$d(e^{\frac{\beta}{3}t}X)=e^{\frac{\beta}{3}t}\frac{\alpha}{3}$
9. Integramos a ambos lados 
$\int d(e^{\frac{\beta}{3}t}X)\,dt$ $=$ $\int e^{\frac{\beta}{3}t}\frac{\alpha}{3}\,dt$
10. Obtenemos los resultados
$e^{\frac{\beta}{3}t}X = \frac{\alpha}{\beta} e^{\frac{\beta}{3}t} + C   $
11. Volvemos a nuestra variable principal
$e^{\frac{\beta}{3}t}W^{\frac{1}{3}} = \frac{\alpha}{\beta} e^{\frac{\beta}{3}t} + C   $

### Cuando $\lim_{t \to \infty} W(t)$
1. Depejamos W y obtenemos
$ W^{\frac{1}{3}} $ $=$  $\frac{\alpha}{\beta} + \frac{C}{e^{\frac{\beta}{3}t}}$
* Sabemos que $\frac{C}{\infty}=0$ por lo que tenemos que: 
$\lim_{t \to \infty} W(t)= (\frac{\alpha}{\beta})^3$
 ### Valores iniciales $W(0)=0$
1. Sabiendo que cualquier numero elevado a la 0 es 1, obtenemos 
$0=\frac{\alpha}{\beta} +C$
Al despejar obtenemos
$C=-\frac{\alpha}{\beta} $
### Depeje de la ecuación a graficar
1. Obtenemos la nueva ecuación
$W =$ $(\frac{\alpha}{\beta} -\frac{\alpha}{\beta} e^{-\frac{\beta}{3}t})^3$
Al graficar obtendremos lo siguiente
![alt text](Imagenes\Graficaproblema3.png)
---