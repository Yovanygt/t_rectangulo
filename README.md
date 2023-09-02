# TRIANGULO RECTANGULO EN PSEINT
Algoritmo TriangulosRectangulos
    Definir numero, opcion como Entero
    
    Escribir "Ingrese un numero entero positivo: "
    Leer numero
    Escribir "\n\n"

    Si numero <= 0 Entonces
        Escribir "El numero debe ser positivo."
        Escribir "\n\n"
    Sino
        Escribir "Elija el tipo de triangulo rectangulo (1-4):"
        Escribir "\n\n"
        Escribir "1. Triangulo rectangulo hacia arriba"
        Escribir "2. Triangulo rectangulo hacia abajo"
        Escribir "3. Triangulo rectangulo hacia la izquierda"
        Escribir "4. Triangulo rectangulo hacia la derecha"
        Leer opcion

        Si opcion >= 1 Y opcion <= 4 Entonces
            Segun opcion Hacer
                Caso 1:
                    Para i desde 1 hasta numero hacer
                        Para j desde 1 hasta i hacer
                            Escribir "* "
                        Fin Para
                        Escribir ""
                    Fin Para
                Caso 2:
                    Para i desde numero hasta 1 con paso -1 hacer
                        Para j desde 1 hasta i hacer
                            Escribir "* "
                        Fin Para
                        Escribir ""
                    Fin Para
                Caso 3:
                    Para i desde 1 hasta numero hacer
                        Para j desde numero hasta i + 1 paso -1 hacer
                            Escribir "  "
                        Fin Para
                        Para k desde 1 hasta i hacer
                            Escribir "* "
                        Fin Para
                        Escribir ""
                    Fin Para
                Caso 4:
                    Para i desde 1 hasta numero hacer
                        Para j desde 1 hasta i - 1 hacer
                            Escribir "  "
                        Fin Para
                        Para k desde i hasta numero hacer
                            Escribir "* "
                        Fin Para
                        Escribir ""
                    Fin Para
            Fin Segun
        Sino
            Escribir "Opción no válida. Por favor, elija un número del 1 al 4."
        Fin Si
    Fin Si
Fin Algoritmo

# TRIANGULO RECTANGULO EN C++
#include <iostream>

int main() {
    int numero;
    
    std::cout << "Ingrese un numero entero positivo: "; 
    std::cin >> numero;
	std::cout << std::endl << std::endl;

    if (numero <= 0) {
        std::cout << "El numero debe ser positivo." << std::endl << std::endl;
    } else {
        int opcion;
        std::cout << "Elija el tipo de triangulo rectangulo (1-4):" << std::endl << std::endl;
        std::cout << "1. Triangulo rectangulo hacia arriba" << std::endl;
        std::cout << "2. Triangulo rectangulo hacia abajo" << std::endl;
        std::cout << "3. Triangulo rectangulo hacia la izquierda" << std::endl;
        std::cout << "4. Triangulo rectangulo hacia la derecha" << std::endl;
        std::cin >> opcion;

        if (opcion >= 1 && opcion <= 4) {
            switch (opcion) {
                case 1:
                    for (int i = 1; i <= numero; i++) {
                        for (int j = 1; j <= i; j++) {
                            std::cout << "* ";
                        }
                        std::cout << std::endl;
                    }
                    break;
                case 2:
                    for (int i = numero; i >= 1; i--) {
                        for (int j = 1; j <= i; j++) {
                            std::cout << "* ";
                        }
                        std::cout << std::endl;
                    }
                    break;
                case 3:
                    for (int i = 1; i <= numero; i++) {
                        for (int j = numero; j > i; j--) {
                            std::cout << "  ";
                        }
                        for (int k = 1; k <= i; k++) {
                            std::cout << "* ";
                        }
                        std::cout << std::endl;
                    }
                    break;
                case 4:
                    for (int i = 1; i <= numero; i++) {
                        for (int j = 1; j < i; j++) {
                            std::cout << "  ";
                        }
                        for (int k = i; k <= numero; k++) {
                            std::cout << "* ";
                        }
                        std::cout << std::endl;
                    }
                    break;
            }
        } else {
            std::cout << "Opción no válida. Por favor, elija un número del 1 al 4." << std::endl;
        }
    }

    return 0;
}
# TRIANGULO RECTANGULO EN PHYTON

numero = int(input("Ingrese un número entero positivo: "))

print("\n\n")

if numero <= 0:

    print("El número debe ser positivo.\n\n")


else:


    opcion = int(input("Elija el tipo de triángulo rectángulo (1-4):\n"
                       "1. Triángulo rectángulo hacia arriba\n"
                       "2. Triángulo rectángulo hacia abajo\n"
                       "3. Triángulo rectángulo hacia la izquierda\n"
                       "4. Triángulo rectángulo hacia la derecha\n"))

    if opcion >= 1 and opcion <= 4:
        if opcion == 1:
            for i in range(1, numero + 1):
                for j in range(1, i + 1):
                    print("* ", end="")
                print()
        elif opcion == 2:
            for i in range(numero, 0, -1):
                for j in range(1, i + 1):
                    print("* ", end="")
                print()
        elif opcion == 3:
            for i in range(1, numero + 1):
                for j in range(numero, i, -1):
                    print("  ", end="")
                for k in range(1, i + 1):
                    print("* ", end="")
                print()
        elif opcion == 4:
            for i in range(1, numero + 1):
                for j in range(1, i):
                    print("  ", end="")
                for k in range(i, numero + 1):
                    print("* ", end="")
                print()
    else:
        print("Opción no válida. Por favor, elija un número del 1 al 4.\n")
#   t _ r e c t a n g u l o  
 