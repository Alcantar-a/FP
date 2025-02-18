# Titulo 1 
## Titulo 2 
### Titulo 3 
#### Titulo 4 
##### Titulo 5
###### Titulo 6 

* bullet 1
* bullet 2
* bullet 3

1. Uno
2. Dos
3. Tres

**Texto Negritas**
_Texto Italica_ 
***Negritas Italicas***

![Descripción de la imagen](https://dropinblog.net/34249715/files/portada-post/el_lenguaje_de_programacion_kotlin_fundamentos_y_caracteristicas.png)
Curso de Fundamentos de Programación


Practica C 
#include <iostream>
#include <string>
using namespace std;
int main() {
       
    // 1.10 
    // Declarar una variable para almacenar el número
        float numero;
        // Solicitar un número al usuario
        cout << "Por favor, ingresa un número: ";
        cin >> numero;
        // Verificar si el número es mayor a 100
        if (numero > 100) {
            cout << "El número es mayor a 100" << endl;
        }
        else {
            cout << "El número es menor o igual que 100" << endl;
        }

       //1.11
       // Declarar una variable para almacenar el número
        float numero1;

        // Solicitar un número al usuario
        cout << "Por favor, ingresa un número: ";
        cin >> numero1;

        // Verificar si el número es negativo
        if (numero1 < 0) {
            cout << "El número es negativo" << endl;
        }
        else {
            cout << "El número es positivo" << endl;
        }

        // 1.12
        // Declarar las variables para almacenar el correo electrónico y la contraseña
        string Miemail, Password_Ingresado;

        // Solicitar el correo electrónico al usuario
        cout << "Por favor, ingresa tu correo electrónico: ";
        cin >> Miemail;

        // Solicitar la contraseña al usuario
        cout << "Por favor, ingresa tu contraseña: ";
        cin >> Password_Ingresado;

        // Validar si la contraseña es correcta
        if (Password_Ingresado == "12345") {
            cout << "Felicidades, password correcto" << endl;
        }
        else {
            cout << "Su password es incorrecto" << endl;
        }

        //1.13
        // Declarar una variable para almacenar los grados Fahrenheit
        float Fahrenheit;

        // Solicitar al usuario ingresar los grados Fahrenheit
        cout << "Por favor, ingresa los grados Fahrenheit: ";
        cin >> Fahrenheit;

        // Calcular los grados Centígrados usando la fórmula
        float Centigrados = (Fahrenheit - 32) * 5 / 9;

        // Verificar si el valor de Fahrenheit es igual a 32
        if (Fahrenheit == 32) {
            cout << "0 grados Centígrados (cero grados)" << endl;
        }
        else {
            // Imprimir el valor de los grados Centígrados en número y en letra
            cout << "Los grados Centígrados son: " << Centigrados << " grados ";

            // Convertir el valor de Centígrados a texto (en letra)
            if (Centigrados == 0) {
                cout << "(cero grados)" << endl;
            }
            else if (Centigrados > 0) {
                cout << "(positivos)" << endl;
            }
            else {
                cout << "(negativos)" << endl;
            }
        }

        //1.14
        // Declarar las variables para almacenar el peso y la estatura
            float peso, estatura, masaCorporal;

            // Solicitar el peso al usuario
            cout << "Por favor, ingresa tu peso en kilogramos: ";
            cin >> peso;

            // Solicitar la estatura al usuario
            cout << "Por favor, ingresa tu estatura en metros: ";
            cin >> estatura;

            // Calcular la masa corporal (IMC) usando la fórmula
            masaCorporal = peso / (estatura * estatura);

            // Mostrar el valor de la masa corporal
            cout << "Tu masa corporal (IMC) es: " << masaCorporal << endl;

            // Verificar en qué categoría entra el IMC y mostrar el mensaje adecuado
            if (masaCorporal < 18.5) {
                cout << "Abajo del peso normal" << endl;
            }
            else if (masaCorporal >= 18.5 && masaCorporal < 25) {
                cout << "Peso normal" << endl;
            }
            else if (masaCorporal >= 25 && masaCorporal < 30) {
                cout << "Sobrepeso" << endl;
            }
            else if (masaCorporal >= 30 && masaCorporal < 35) {
                cout << "Obeso Clase 1" << endl;
            }
            else if (masaCorporal >= 35 && masaCorporal < 40) {
                cout << "Obeso Clase 2" << endl;
            }
            else {
                cout << "Obeso Clase 3" << endl;
            }

            //1.16
             // Declarar tres variables para los números A, B, y C
            float A, B, C;

            // Solicitar los tres números al usuario
            cout << "Por favor, ingresa el primer número (A): ";
            cin >> A;
            cout << "Por favor, ingresa el segundo número (B): ";
            cin >> B;
            cout << "Por favor, ingresa el tercer número (C): ";
            cin >> C;

            // Determinar cuál es el número más grande
            if (A >= B && A >= C) {
                cout << "El número más grande es: " << A << endl;
            }
            else if (B >= A && B >= C) {
                cout << "El número más grande es: " << B << endl;
            }
            else {
                cout << "El número más grande es: " << C << endl;
            }

            //1.18
            // Declarar las variables para la hora, minutos y segundos
            int hora, minutos, segundos;

            // Solicitar al usuario ingresar la hora, minutos y segundos
            cout << "Ingresa la hora (HH): ";
            cin >> hora;
            cout << "Ingresa los minutos (MM): ";
            cin >> minutos;
            cout << "Ingresa los segundos (SS): ";
            cin >> segundos;

            // Incrementar los segundos por 1
            segundos++;

            // Comprobar si los segundos alcanzan 60
            if (segundos == 60) {
                segundos = 0;
                minutos++;
            }

            // Comprobar si los minutos alcanzan 60
            if (minutos == 60) {
                minutos = 0;
                hora++;
            }

            // Comprobar si las horas alcanzan 24 (es un reloj de 24 horas)
            if (hora == 24) {
                hora = 0;
            }

            // Mostrar el nuevo tiempo
            cout << "La hora después de un segundo será: ";
            cout << (hora < 10 ? "0" : "") << hora << ":"; // Asegurar el formato 2 dígitos para la hora
            cout << (minutos < 10 ? "0" : "") << minutos << ":"; // Asegurar el formato 2 dígitos para los minutos
            cout << (segundos < 10 ? "0" : "") << segundos << endl; // Asegurar el formato 2 dígitos para los segundos
