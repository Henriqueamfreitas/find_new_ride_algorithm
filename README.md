A aplicação é uma plataforma de viagens de carro compartilhadas, por aplicativo. O objetivo é desenvolver o algoritmo que encontra a corrida mais próxima para o motorista, fornecendo as coordenadas precisas do 
passageiro, e a distância até o ponto de encontro. Como a precisão é extremamente importante nessa funcionalidade, o time de requisitos conseguiu estipular 256 casos de teste, mapeando uma parte de um pequeno 
bairro e estipulando qual deveria ser a saída para todas as possibilidades de coordenadas do motorista.

O template para utilizar nesse projeto está neste repositório.

Utilizei um arquivo com esse mapa 2D simulado de 16x16 posições e estes testes já programados utilizando console.log() para ajudar a testar seu algoritmo. O principal requisito é funcionar perfeitamente para todos 
os 256 casos de teste. As posições com o valor 1 são onde existe uma solicitação de corrida por um passageiro. E a distância entre um valor e outro imediatamente ao seu lado é sempre de 1 km, em qualquer direção.

A assinatura da função a ser desenvolvida é: findNewRide(driverPositionX, driverPositionY) e o retorno é um array contendo na primeira posição outro array com as coordenadas do passageiro mais próximo [x,y] e na 
segunda posição uma string mostrando em km a distância até o passageiro, com duas casas decimais de precisão, conforme o exemplo abaixo:

O retorno do caso de teste ⁠⁠findNewRide(0,0) deverá ser: [[7,0],'7.00 km']

Caso os testes sejam aprovados, eles serão apresentados na cor verde precedidos da palavra PASS e enquanto não estiver satisfazendo as condições ideais, os testes serão apresentados na cor vermelha, precedidos da 
palavra FAIL. Em ambos os casos, indica quais as coordenadas do motorista foram testadas em cada caso.

A distância a ser calculada na primeira versão é a mais simples, em linha reta, também conhecida como distância euclidiana, que segue o mesmo princípio do teorema de pitágoras.

**Tecnologias**: Javacript e Shell
