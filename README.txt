tecnologias utilizadas: codeblocks(para escrever e rodar a aplicação), linguagem c#/c++

bibliotecas: <stdio.h>, <time.h>, <cstdlib>

como rodar aplicação: tendo o codebloks devidamente instaldo e aberto na maquina (mas também pode ser lido em outros softwares de desenvolvimento como visual studio, etc.), 
aperte "ctrl+o" navegue até onde a pasta do desafio foi salva, e dentro, selecione e abra o projeto, e então aperte a tecla de atahlo "f9" para rodar o codigo.
ou entre na pasata do projeto e abra: "2campgeminidesafio.exe"

****************************************************************************************************************************
*esse é o codigo comentado caso não consiga abrir a aplicação**esse é o codigo comentado caso não consiga abrir a aplicação*
****************************************************************************************************************************


#include <stdio.h>
#include <time.h>
#include <cstdlib>
int main(){
int i, x, aux, v[5];                                                        //declarando variaveis

for(i=0; i<5; i++){
    printf("digite um valor %i:",i);
    scanf("%i", &v[i]);
                                                                            /*
                                                                            laço de repetição "for", esta lendo as entradas do usuario
                                                                             e aramazanando na variavel indice (i) e repentindo a perqunta enauqanto for menor que 5
                                                                             em seguida armazena o indice no vetor(v[i])
                                                                            */
}
                                                                            /*
                                                                            aqui o laço vai ler e interpretar as informações, para alocar nas ordens corretas
                                                                            contador para ordenar as posições em ordem crescente:
                                                                            */
for(i=0; i<5; i++){
    for(x=i;x<5;x++)                                                         // o X representa a lista de indices ja ordenada
        {
        if(v[i]>v[x])
                                                                             /* aqui o if esta comparando se: o indice no vetor de indices i é maior que os no vetor de indeces x
                                                                             indice é a posição do valor armazenado no vetor
                                                                             para inverter a ordem da lista bastaria inverter o sinal de maior, para menor*/
        {
            aux=v[i];
            v[i]=v[x];
            v[x]=aux;
                                                                            /*
                                                                            a variavel auxiliar(aux), tem a função de trocar de lugar nas posições dentro do vetor, logo:
                                                                            aux passa a valer os indices i (que até então são maiores que x),
                                                                            e os indices i passam a valer o inice x (que são menorres que i),
                                                                            e por fim o vetor de indices x assume os valores auxiliares, formando a lista
                                                                            */
        }
    }
}
printf("\nos valores ordenados em ordem crescente ficam:\n");               // o printf aqui é pra imprimir na tela o resultado
for (i=0; i<5; i++)
    {
        printf("\n %i", v[i]);                                              //printf esta imprimindo o vetor na tela
    }
    printf("\no valor mediano e: %i", v[2]);
                                                                            /*
                                                                            printf esta mostrando o mediano, que por se tratar de um grupo de sempre 5 numeros,
                                                                            estara sempre ocupando a terceira posições dps de ser processado pela maquina, vulgo V[2](ja que inicia do zero)
                                                                            */
}





***********************************************************************************************
**esse é o codigo sem comentarios, para só copiar e colar, caso não consiga abrir a aplicação**
***********************************************************************************************
#include <stdio.h>
#include <time.h>
#include <cstdlib>
int main(){
int i, x, aux, v[5];                                                        
for(i=0; i<5; i++){
    printf("digite um valor %i:",i);
    scanf("%i", &v[i]);                                                              
}                                                                       
for(i=0; i<5; i++){
    for(x=i;x<5;x++)                                                       
        {
        if(v[i]>v[x])                                                        
            aux=v[i];
            v[i]=v[x];
            v[x]=aux;                                                                     
        }
    }
}
printf("\nos valores ordenados em ordem crescente ficam:\n");               
for (i=0; i<5; i++)
    {
        printf("\n %i", v[i]);                                           
    }
    printf("\no valor mediano e: %i", v[2]);
                                                                            
}
