# Problema-P236
## Pensando o Problema

É essencial entendermos o processo que o problema nos propõe. Nesse caso, o processo central que o problema nos propõe, é uma **conversão de valores**, de kcal/min, para kcal.

Ele nos pede para coletar a minutagem de um indivíduo em cada esporte; converter cada minutagem para kcal, de acordo com a relação estabelecida *(kcal/min)*; fazer a soma de calorias perdidas em todos os esportes; e por fim, imprimir o resultado na tela.

## Dividindo em Partes

Uma forma de facilitar a nossa capacidade de organizar o problema, é **dividindo** ele. Vamos dividi-lo na seguinte maneira:

- **Bloco 1 - Receber Valores:** nesse primeiro bloco, vamos receber todos os valores de entrada em minuto.
- **Bloco 2 - Conversão de Valores:** aqui está o processo principal do problema, em que vamos converter os valores da entrada para kcal.
- **Bloco 3 - Soma e Impressão:**  neste último bloco, somamos os valores processados, e imprimimos eles na tela.

## Código

No **Bloco 1**, primeiramente, vamos definir nossas variáveis:

	#include <iostream>

	using namespace std;
	int main(int argc, char** argv) {
	
	int m_bas, m_cic, m_fut, m_vol; //Minutos em cada Esporte
	int bas, cic, fut, vol; //Total de kcal em cada Esporte
	int soma; //Soma Total de kcal
	
		return 0;
	} 

Depois de definir as variáveis, vamos pedir para que o usuário **insira** os valores correspondentes a minutagem em cada esporte:

	#include <iostream>

	using namespace std;
	int main(int argc, char** argv) {
	
	//Definição
	int m_bas, m_cic, m_fut, m_vol; //Min em cada Esporte
	int bas, cic, fut, vol; //Total de kcal em cada Esporte
	int soma; //Soma Total de kcal
	
	//Minutos por cada esporte
	cin >> m_bas;
	cin >> m_cic;
	cin >> m_fut;
	cin >> m_vol;
	
		return 0;
	}

Agora, no **Bloco 2**, precisamos pegar essas variáveis coletadas em minuto, e converte-las para kilo caloria, utilizando a relação *kcal/min* e os dados que o problema apresentou:

	#include <iostream>

	using namespace std;
	int main(int argc, char** argv) {
	
	//Definição
	int m_bas, m_cic, m_fut, m_vol; //Min em cada Esporte
	int bas, cic, fut, vol; //Total de kcal em cada Esporte
	int soma; //Soma Total de kcal
	
	//Minutos por cada esporte
	cin >> m_bas;
	cin >> m_cic;
	cin >> m_fut;
	cin >> m_vol;
	
	//Gasto em kcal
	bas = m_bas * 10;
	cic = m_cic * 6;
	fut = m_fut * 9;
	vol = m_vol * 6;
	
		return 0;
	}
Por último, no **Bloco 3**, precisamos somar todos os valores de gasto em kcal em uma só variável, no caso, na variável `soma`:

	#include <iostream>

	using namespace std;
	int main(int argc, char** argv) {
	
	//Definição
	int m_bas, m_cic, m_fut, m_vol; //Min em cada Esporte
	int bas, cic, fut, vol; //Total de kcal em cada Esporte
	int soma; //Soma Total de kcal
	
	//Minutos por cada esporte
	cin >> m_bas;
	cin >> m_cic;
	cin >> m_fut;
	cin >> m_vol;
	
	//Gasto em kcal
	bas = m_bas * 10;
	cic = m_cic * 6;
	fut = m_fut * 9;
	vol = m_vol * 6;
	
	//Somando Gasto
	soma = bas + cic + fut + vol;
	
	//Imprimindo Soma Total
	cout << soma;	

		return 0;
	}
