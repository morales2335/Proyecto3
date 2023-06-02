
# **Documentación Proyecto número 3** 
 ___
**Datos principales:**

Universidad Mariano Galvéz de Guatemala, Sede Boca del Monte.

Introducción a los Sistemas de Computo.

Ingeniero: Melvin Cali.

**Integrantes:**

1. Carlos Enrique Ruiz Illescas. **No Carnet:** 7690-14-10690.    
2. Isaías Morales Illescas. **No Carnet:** 7690-23-705.

**Link del video**
[Proyecto3](https://youtu.be/1iZhTtxVUYM)

## **Explicación de lo realizado**

Para la realización de esté proyecto número 3, se tuvo que poner en práctica cierto conocimientos acerca de Pseudocódigo, también se realizaron busquedas e investigaciones para poder solventar algunas dudas, y así poder resolver los diferentes problemas dados en el proyecto. 

## **Proceso para llevar a cabo el algoritmo** 

1. Encabezado: es la primer parte del algoritmo donde se indica el nombre del mismo.
2. Definir variables: Se declara la variable con el tipo de dato que va a almacenar. 
3. Cuerpo: donde se especifican las acciones que se van a realizar.
   

___
## **Código fuente del programa**

___
```psc
 Algoritmo calculadora
	//VARIABLES
	Definir numero1,numero2 como entero;	
	Definir numf, numc, filas, columnas, sum, rest Como Entero;
	Dimension matriz[99,99];
	Dimension matriz1[99,99];
	Dimension matriz2[99,99];
	Dimension matriz3[99,99];
	Definir numero, i, j, a como entero;
	//MENU DE OPCIONES 
	Repetir
		Escribir "     CALCULADORA --> MENU DE OPCIONES <--   ";
		Escribir " ========================================== ";
		Escribir "| 1. Suma                                  |";
		Escribir "| 2. Resta                                 |";
		Escribir "| 3. Multiplicacion                        |";
		Escribir "| 4. Division                              |";
		Escribir "| 5. Sumar todos los valores de la matriz  |";
		Escribir "| 6. Restar todos los valores de la matriz |";
		Escribir "| 7. Suma de matrices                      |";
		Escribir "| 8. Resta de matrices                     |";
		Escribir "| 9. Triangulo con numeros                 |";
		Escribir "| 10. Rectangulo con asteriscos            |";
		Escribir "| 11. Salir                                |";
		Escribir " ========================================== ";
		Escribir Sinsaltar"Selecciona una opcion : ";
		Leer opcion;
		//ACCIONES SEGUN EL MENU 
		Segun opcion Hacer
			1: 
				Repetir
					Escribir Sinsaltar "Ingrese primer numero: ";
					Leer numero1;
					Escribir Sinsaltar"Ingrese segundo numero: ";
					Leer numero2;
					suma<-numero1+numero2;
					Escribir numero1," + ",numero2," = ",suma;
					Escribir Sinsaltar"Desea realizar otra suma? si/no ";
					leer respuesta;
				Mientras Que respuesta = "si";
				Limpiar Pantalla;
				
			2:
				Repetir
			     	Escribir Sinsaltar"Ingrese primer numero: ";
				    Leer numero1;
					Escribir Sinsaltar"Ingrese segundo numero: ";
					Leer numero2;
					resta<-numero1-numero2;
					Escribir numero1," - ",numero2," = ",resta;
					Escribir Sinsaltar"Desea realizar otra resta? si/no ";
					leer respuesta;
				Mientras Que respuesta = "si";
				Limpiar Pantalla;
				
			3:
				Repetir
					Escribir Sinsaltar"Ingrese primer numero: ";
					Leer numero1;
					Escribir Sinsaltar"Ingrese segundo numero: ";
					Leer numero2;
					multiplicacion<-numero1*numero2;
					Escribir numero1," * ",numero2," = ",multiplicacion;
					Escribir Sinsaltar"Desea realizar otra multiplicacion? si/no ";
					leer respuesta;
				Mientras Que respuesta = "si";
				Limpiar Pantalla;
				
			4:
				Repetir
					Escribir Sinsaltar"Ingrese primer numero: ";
					Leer numero1;
					Escribir Sinsaltar"Ingrese segundo numero: ";
					Leer numero2;
					division<-numero1/numero2;
					Escribir numero1," / ",numero2," = ",division;
					Escribir Sinsaltar"Desea realizar otra division? si/no ";
					leer respuesta;
				Mientras Que respuesta = "si";
				Limpiar Pantalla;
				
			5:
				Repetir
					sum<-0;
					Escribir Sinsaltar"Ingrese el numero de filas: ";
					Leer numf;
					Escribir Sinsaltar"Ingrese el numero de columnas: ";
					Leer numc;
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
						Escribir Sinsaltar "Ingrese dato en la posicion:[" filas ",",columnas "]";
					Leer matriz[filas,columnas];
					Fin Para
					Fin Para
					
					Escribir "La matriz quedaria de la siguiente manera:";
					
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
						Escribir Sin Saltar "  " matriz[filas,columnas],"  ";
						Fin Para
						Escribir " ";
					Fin Para
					
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
							sum<-sum + matriz[filas,columnas];
						Fin Para
					Fin Para
					
					Escribir "El resultado de la suma de todas las posiciones de la matriz es: " sum;
					Escribir Sinsaltar"Desea seguir generando matrices? si/no ";
					leer respuesta;
				Mientras Que respuesta = "si";
				Limpiar Pantalla;
				
			6:
				Repetir
					rest<-0;
					Escribir Sinsaltar"Ingrese el numero de filas: ";
					Leer numf;
					Escribir Sinsaltar"Ingrese el numero de columnas: ";
					Leer numc;
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
							Escribir Sinsaltar"Ingrese dato en la posicion:[" filas ",",columnas "]";
							Leer matriz[filas,columnas];
						Fin Para
					Fin Para
					
					Escribir "La matriz quedaria de la siguiente manera:";
					
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
							Escribir Sin Saltar "  " matriz[filas,columnas],"  ";
						Fin Para
					Escribir " ";
					Fin Para
					
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta  numc-1 Con Paso 1 Hacer
						si rest = 0 entonces 
							rest <- matriz[filas,columnas] - rest; 
						SiNo
							rest <- rest - matriz[filas,columnas]; 
						FinSi
						Fin Para
					Fin Para
					
					Escribir "El resultado de la resta de todas las posiciones de la matriz es: " rest;
					Escribir Sinsaltar"Desea seguir generando matrices? si/no ";
					leer respuesta;
				Mientras Que respuesta = "si";
				Limpiar Pantalla;
				
			7:
				Repetir
					Escribir Sinsaltar"Ingrese el numero de filas: ";
					Leer numf;
					Escribir Sinsaltar"Ingrese el numero de columnas: ";
					Leer numc;
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
						Escribir Sinsaltar"Ingrese datos en las posiciones para la primera matriz [" filas ",",columnas "]: ";
						Leer matriz1[filas,columnas];
					Fin Para
					Fin Para
				
					Escribir "La primera matriz quedaria de la siguiente manera:";
				
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
						Escribir Sin Saltar " " matriz1[filas,columnas]," ";
					Fin Para
					Escribir " ";
					Fin Para
					Escribir "";
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
						Escribir Sinsaltar"Ingrese datos en las posiciones para la segunda matriz [" filas ",",columnas "]: ";
						Leer matriz2[filas,columnas];
					Fin Para
					Fin Para
				
					Escribir "La segunda matriz quedaria de la siguiente manera:";
				
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
						Escribir Sin Saltar " " matriz2[filas,columnas]," ";
					Fin Para
					Escribir " ";
					Fin Para
				
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
					matriz3[filas,columnas] <- matriz1[filas,columnas] + matriz2[filas,columnas];
					Fin Para
					Fin Para
				
					Escribir "";
					Escribir "La suma de ambas matrices quedaria de la siguiente manera: ";
				
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
					Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
					Escribir Sin Saltar " " matriz3[filas,columnas]," ";
					Fin Para
					Escribir " ";
				    Fin Para
				Escribir Sinsaltar"Desea seguir sumando matrices? si/no ";
				leer respuesta;
			Mientras Que respuesta = "si";
			Limpiar Pantalla;
				
			8:
				Repetir
					Escribir Sinsaltar"Ingrese el numero de filas: ";
					Leer numf;
					Escribir Sinsaltar"Ingrese el numero de columnas: ";
					Leer numc;
					
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
						Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
							Escribir Sinsaltar"Ingrese datos en las posiciones para la primera matriz [" filas ",",columnas "]: ";
							Leer matriz1[filas,columnas];
						Fin Para
					Fin Para
					
					Escribir "La primera matriz quedaria de la siguiente manera:";
					
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
						Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
							Escribir Sin Saltar " " matriz1[filas,columnas]," ";
						Fin Para
						Escribir " ";
					Fin Para
					Escribir "";
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
						Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
							Escribir Sinsaltar"Ingrese datos en las posiciones para la segunda matriz [" filas ",",columnas "]: ";
							Leer matriz2[filas,columnas];
						Fin Para
					Fin Para
					
					Escribir "La segunda matriz quedaria de la siguiente manera:";
					
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
						Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
							Escribir Sin Saltar " " matriz2[filas,columnas]," ";
						Fin Para
						Escribir " ";
					Fin Para
					
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
						Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
							matriz3[filas,columnas] <- matriz1[filas,columnas] - matriz2[filas,columnas];
						Fin Para
					Fin Para
					
					Escribir "";
					Escribir "La resta de ambas matrices quedaria de la siguiente manera: ";
					
					Para filas<-0 Hasta numf-1 Con Paso 1 Hacer
						Para columnas<-0 Hasta numc-1 Con Paso 1 Hacer
							Escribir Sin Saltar " " matriz3[filas,columnas]," ";
						Fin Para
						Escribir " ";
				    Fin Para
					Escribir Sinsaltar"Desea seguir restando matrices? si/no ";
					leer respuesta;
				Mientras Que respuesta = "si";
				Limpiar Pantalla;
				
			9:
				Repetir
	
					Escribir sin saltar "Ingresa un numero para definir el tamanio del triangulo";
					leer numero;
					j <- 1; 
					i <- 0; 
					Mientras i < numero Hacer	
						si j mod 2 = 1 Entonces
							para a <- j Hasta 1 Con Paso -1 Hacer;
								si a mod 2 = 1 Entonces
									Escribir Sin Saltar " ", a;
								FinSi
							FinPara
							Escribir "";
							i <- i + 1;
						FinSi	
						j <- j + 1;
					FinMientras					
					Escribir Sinsaltar"Desea seguir generando triangulos? si/no ";
					leer respuesta;
				Mientras Que respuesta = "si"; 
				Limpiar Pantalla;
			10:
				Repetir
					Escribir Sinsaltar"Escribe un numero para generar cuadro de asteriscos: ";
					leer numero;
					para i <- 1 hasta numero Hacer
						para j <- 1 hasta numero Hacer
							Si i > 1 y i < numero y j > 1 y j < numero entonces
								Escribir Sin Saltar "  ";
							SiNo
								Escribir Sin Saltar "* ";
							FinSi
						FinPara
						Escribir " ";
					FinPara
					Escribir Sinsaltar"Desea seguir generando cuadros con asteriscos? si/no ";
					leer respuesta;
				Mientras Que respuesta = "si";
				Limpiar Pantalla;
				
			11:
				Escribir "GRACIAS!";
			De Otro Modo:
				Escribir "OPCION INCORRECTA!";
				Escribir Sinsaltar"Presiona tecla ENTER para volver al menu";
				leer respuesta;
				Limpiar Pantalla;
		FinSegun
	Hasta Que opcion = 11;
FinAlgoritmo


```