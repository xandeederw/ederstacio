#include <iostream>
#include <math.h>
using namespace std;
int main()
{
	float larg,alt,rend,tamlata,prelata,tamparede,qtdlata,total,quantopinta;
	cout << "Digite a largura da parede em (m): ";
	cin >> larg;
	cout << "Digite a altura da parede em (m): ";
	cin >> alt;
	cout << "Informe o rendimento da tinta em (m2/litro): ";
	cin >> rend;
	cout << "Informe o tamanho da lata em (l): ";
	cin >> tamlata;
	cout << "Informe o preco da lata R$: ";
	cin >> prelata;
	tamparede = larg * alt;
	quantopinta = rend * tamlata;
	qtdlata = tamparede / quantopinta;
	total = qtdlata * prelata;
	cout << "Tamanho da parede: " << tamparede << " m2" << endl;
	cout << "Quantidade de latas: " << ceil (qtdlata) << " latas" << endl;
	cout << "Total gasto R$ " << total << endl;
}
