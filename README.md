#include <iostream>
#include <limits>

using namespace std;

int main() {
    int numero;

    cout << "Ingresa un número entero (1-12) para saber qué mes corresponde: ";

    if (!(cin >> numero)) {
        cout << "Error: Entrada inválida. Debes ingresar un número entero." << endl;
        return 1;
    }

    if (numero < 1 || numero > 12) {
        cout << "El número ingresado no corresponde a ningún mes válido." << endl;
    } else {
        switch (numero) {
            case 1:  cout << "Enero"; break;
            case 2:  cout << "Febrero"; break;
            case 3:  cout << "Marzo"; break;
            case 4:  cout << "Abril"; break;
            case 5:  cout << "Mayo"; break;
            case 6:  cout << "Junio"; break;
            case 7:  cout << "Julio"; break;
            case 8:  cout << "Agosto"; break;
            case 9:  cout << "Septiembre"; break;
            case 10: cout << "Octubre"; break;
            case 11: cout << "Noviembre"; break;
            case 12: cout << "Diciembre"; break;
        }
        cout << endl;
    }

    return 0;
}
