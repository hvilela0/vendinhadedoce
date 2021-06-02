# vendinhadedoce

```
#include <stdlib.h>
#include <stdio.h>


	struct CLIENTE {
		int 	prod[25];
		float 	qtde[25];
	} cliente[25];
	


void novoCliente(CLIENTE cliente);
void gerarRelatorio();

int main() {
	
	int opcao = -1;
	int j = 0;
	
	while(opcao != 0){
		printf("Selecione a opcao: \n");
		printf("1 - Novo Cliente\n");
		printf("2 - Gerar relatorio\n");
		printf("-----------\n");
		printf("Digite 0 para finalizar\n");	
		scanf("%i", &opcao);
	
		switch(opcao){
			case 1:
				novoCliente(cliente[j]);
				j++;
				break;
			case 2:
				gerarRelatorio();
				break;
			default:
				printf("Fim de programa");
				break;
		}
	}
	printf("\n");
	system("pause");
	return 0;
}
void novoCliente(CLIENTE cliente){
	system("cls");
	int prod = -1;
	float qtde = 0.0;
	int i = 0;
// mostra o menu de compras para o cliente
	while(prod != 0) {
		printf("Selecione o produto: \n");
		printf("1 - Trufa\n");
		printf("2 - Torta\n");
		printf("3 - Bolo\n");
		printf("-----------\n");
		printf("Digite 0 para finalizar\n");
		
		printf("Digite a opcao: ");
		scanf(" %i",&prod);
		system("cls");
		if(prod == 0) return; //break;
		
		// produto selecionado: xxx
		printf("Digite a quantidade em (kg): ");
		scanf(" %f",&qtde);		
		//salvar o pedido para o cliente (...)
		system("cls");
		
		cliente.prod[i] = prod;
		cliente.qtde[i] = qtde;
		i++;
	}
}

void gerarRelatorio(){
	printf("\n-------- Relatorio --------\n");
	for(int j=0;j<25;j++){
		printf("O Cliente %d comprou: \n", j);
		for(int i=0;i<25;i++){
			// continaur daqui...
	}
	
	
}
```
