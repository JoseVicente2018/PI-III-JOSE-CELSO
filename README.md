# PI-III-JOSECELSO

# Proposta de Tema de PI3
Título:
Desenvolvimento de um software usando óculos de realidade virtual

Aluno(s): José Celso Vicente do Nascimento

Orientador: Prof. Sérgio Augusto Bitencourt Petrovcic

# Objetivo geral
O objetivo deste trabalho é desenvolver um software ( uma intereção educacional da área da elétrica) usando óculos de realidade virtual no ambiente Unity, na linguagem C#. O óculos de realidade virtual será fornecido pelo IFSC.


# Objetivos específicos

Estudar o funcionamento do óculos de realidade virtual; Documentar todos os procedimentos (conexão, configuração, calibração, carregamento, cuidados necessários, limpeza, armazenamento).

Conectar o óculos de realidade virtual ao computador;

Realizar a integração do óculos de realidade virtual com o ambiente de desenvolvimento Unity;

Escolha de um procedimento de teste na área da elétrica para desenvolvê-lo de forma realidade virtual pelo software Unity;

Desenvolver um software no Unity usando o óculos de realidade virtual com a função hand tracking; (comunicação, codificação, bibliotecas necessária)



# Metodologia

Para realização do objetivo proposto faz-se necessário  primeiramente entender a tecnologia de realidade virtual (VR), o espaço virtual 3D através do software Unity e também o conteúdo da engenharia elétrica a ser desenvolvido nessa interação. Para isso, é importante a introdução desse novo tipo de tecnologia de realidade virtual. A fim de facilitar a execução do projeto, optou-se por seguir a sequência dos objetivos específicos, buscando assim a integração dos conhecimentos necessários para alcançar o objetivo geral do projeto no ambiente de Realidade Virtual, estabelecendo a conexão entre o Oculus e o Unity.

Para o bom entendimento inicial é importantissímo salientar a diferença de realidade virtual para a realidade aumentada. A realidade virtual (RV), utilizada nesse projeto, é uma tecnologia que cria um ambiente digital totalmente imersivo, onde os usuários podem interagir com esse ambiente como se estivessem fisicamente presentes nele. Isso geralmente é alcançado por meio do uso de dispositivos como óculos de realidade virtual, nesse projeto usa-se o Oculus Meta Quest 2, que bloqueiam a visão do mundo real e substituem por uma simulação digital. Já a realidade aumentada (RA) combina elementos do mundo real com elementos virtuais. Ao contrário da realidade virtual, a realidade aumentada não substitui completamente o ambiente real, mas sobrepoõe informações digitais sobre a visão do mundo real. Resumidamente, na realidade virtual, os usuários são totalmente imersos em um ambiente digital, enquanto na realidade aumentada, elementos virtuais são sobrepostos ao ambiente real.
O Unity é um programa para computador o qual proporciona ao seu usuário a possibilidade de criar modelos em 3D de objetos e 3D de ambientes e, além disso, possibilita criar ambientes de realidade virtual também possibilitando a interatividade com o Oculus Meta Quest 2.

## Funcionamento do Oculus Meta Quest 2 (VR)
O Oculus Meta Quest 2 proporciona uma experiência intuitiva desde o momento da sua conexão inicial. Ao ser conectado pela primeira vez, o dispositivo guia o usuário por ajustes básicos, como a seleção do idioma, e o introduz ao ambiente de realidade virtual por meio de uma animação imersiva. Durante esse processo inicial, o Oculus solicita a criação de uma conta no aplicativo Meta Quest, tendo o seu acesso via celular. Essa associação entre o dispositivo e o aplicativo disponibiliza um leque de opções, incluindo a capacidade de conectar o Oculus ao celular, permitindo comandos diretos do aplicativo para o dispositivo. Além disso, o aplicativo proporciona a primeira interação de espelhamento do Oculus para visualização no celular, tendo a sua primeira interação entre telas. Ainda na configuração inicial, o Oculus bloqueia o mundo real (como característica do VR) para introduzir o usuário em um ambiente totalmente imersivo, é necessário restringir o espaço de uso do dispositivo por motivos de segurança. O Oculus oferece dois modos para essa finalidade: a "Área Segura", onde você pode calibrar a altura do solo e o limite do espaço seguro usando o joystick, e o segundo modo, chamado de "Limite Estacionário", ideal para uso do Oculus enquanto sentado, sendo assim um ponto fixo. Após a definição da área, é possível escolher, nas configurações, entre o uso do joystick ou handtracking, permitindo a interação apenas com as mãos, sem a necessidade do joystick. Quanto ao carregamento, é importante observar que o  Oculus utiliza um conector de carregamento estadunidense, exigindo um adaptador para utilização em tomadas brasileiras para o seu carregamento. Para uma boa limpeza, a Meta Quest, disponibiliza em seu site orientações detalhadas sobre os passos a serem seguidos e os produtos recomendados de higienização, e uma obnservação interessante abordado no site é a a proteção para evitar a propagação de doenças contagiosas. Estando disponível no https://business.oculus.com/support/665720147270975/?locale=pt_BR. Dessa forma, manter sempre em dia a higienização do dispositivo e possuindo um lugar adequado para armazanemento.

## Conectar o óculos de realidade virtual ao computador/notebook
 
1ª opção (Casting)
	Conexão via casting. Para acessar essa função deve-se acessar o aplicativo câmera no próprio oculus e clicar na função de transmissão via casting, dessa forma consegue-se acessar em qualquer navegador de internet através de um endereço disponibilizado pelo próprio oculus.
 
2ª opção (Cabo link)
	Outra opção é via cabo link (cabo oficial disponibilizado pela meta quest, necessário realizar a compra a parte, pois não vem com o oculus), para essa função deve-se acessar a opção “configuração”, depois ir na função de “quest link” e selecionar o modo via cabo link no próprio oculus, e no dispositivo onde se deseja realizar o espelhamento, deve-se baixar o aplicativo do meta quest e selecionar o dispositivo e o modo de conexão para espelhamento, nesse caso, via cabo link.
 
3ª opção (Air link)
	Para realizar a opção de espelhamento via rede, para essa função deve-se acessar a opção “configuração”, depois ir na função de “quest link” e selecionar o modo via cabo link no próprio oculus, e no dispositivo onde se deseja realizar o espelhamento, deve-se baixar o aplicativo do meta quest e selecionar o dispositivo e o modo de conexão para espelhamento, nesse caso, via air link.

## Realizar a integração do óculos de realidade virtual com o ambiente de desenvolvimento Unity;

Para realizar a conexão do oculus ao Unity, o notebook ou pc devem possuir a porta de acesso para cabo USB- C. Dessa forma, o próprio modo de criação de ambiente VR do Unity reconhecerá o dispositivo de entrada, que é o Oculus. Existem 3 modos de acessar o arquivo gerado pelo Unity no Oculus:

1º modo (cabo link)

Para acessar o Unity e ter sua interação basta ter o cabolink onde no próprio Unity você seleciona o dispositivo de entrada, após isso, no oculus, você realiza a primeira opção de espelhamento, dessa forma, todas as alterações feitas no Unity, e após a sua compilação, ao dar play. No próprio oculus você poderá interagir com o ambiente desenvolvido no software Unity.

2º modo (cabo USB-C)

Conexão via USB-C, a diferença para o anterior é a seguinte, para poder interagir no oculus deve-se acessar a opção (file>build and run) dessa forma, gerando dentro do oculus um arquivo (app) apk para acesso. Ou seja, toda vez que fizer alteração terá que fazer esse procedimento, diferentemente do primeiro modo, o qual bastava apertar play.
3ª modo (SIDE QUEST)
Para ter acesso ao arquivo deverá realizar a criação de um apk gerado no próprio ambiente unity em (file> build), depois transferir esse arquivo para o aplicativo sidequest dessa forma gerando o arquivo de acesso no oculus.

## Escolha de um procedimento de teste na área da elétrica para desenvolvê-lo de forma realidade virtual pelo software Unity;

Antes de desenvolver o software no unity, buscou-se na área da elétrica possíveis procedimentos, testes de funcionamentos que seriam viáveis para desenvolvimento do software. E com isso, através da sugestão do orientador, decidiu-se ir em busca de testes em motores elétricos trifásicos. No livro “Motores elétricos e acionamentos’’ do PETRUZELLA, Frank D. No capítulo 5 e na 8º parte ele trás diversos tipos de testes (ex: testes de isolamento dos enrolamentos) e possíveis problemas em motores elétricos, alguns exemplos: resistência de isolamento baixa, fusível queimado ou disjuntor desarmado, defeitos nos enrolamentos do motor.
	O procedimento decidido a se fazer foi o teste de medição de resistência de isolamento do motor através de um megometro. Para isso buscou-se a respectiva norma que disponibiliza o que deve ser levado em consideração para a realização do teste, a norma designada é a norma ABNT NBR 17094-3:2018  (Máquinas elétricas girantes Parte 3: Motores de indução trifásicos ― Métodos de ensaio). Para o teste a norma possibilita dois tipos de medições, de cada fase, ou do curto circuito das fases com o sistema de aterramento do motor. Para um bom entendimento do processo de teste, o Professor Tiago Drummond juntamente a sua turma de conversão eletromecânica de energia 1, proporcionou na fábrica o teste prático de um motor trifásico que foi doado para a instituição de forma a averiguar se o mesmo estava em condições de uso. Como pode ser visto nas seguintes figuras 1 e a figura 2:
 Figura 1: realização do teste prático.
 ![image](https://github.com/JoseVicente2018/PI-III-JOSE-CELSO/assets/141693494/273b406c-d67a-4670-bb07-4004e9c7d48a)
Fonte: o autor.
 Figura 2: realização do teste prático.
![image](https://github.com/JoseVicente2018/PI-III-JOSE-CELSO/assets/141693494/4a4476b6-ca83-4c38-a2f3-a82d161f2488)
Fonte: o autor.

A norma recomenda no minimo uma resistência confiável de operação de 5 Mohms. Como mostra a tabela.
![image](https://github.com/JoseVicente2018/PI-III-JOSE-CELSO/assets/141693494/352c1225-0b54-45a6-8ac1-b8a7f77bca82)
Fonte: ABNT NBR 17094-3:2018.

E para calibração do megometro, segundo a norma:
![image](https://github.com/JoseVicente2018/PI-III-JOSE-CELSO/assets/141693494/d8c4404e-3655-486f-97c9-648435f677a0)
Fonte: ABNT NBR 17094-3:2018.

Para a análise do resultado encontrado no megometro (aplicado uma tensão de 500V, sendo o motor de 500V), de acordo com a norma citada anteriormente a resistência de isolamento deve ser maior que 5Mohms. Figura 3 mostra o resultado da teste.
![image](https://github.com/JoseVicente2018/PI-III-JOSE-CELSO/assets/141693494/2379a9cb-a84a-4b2e-aa1e-56af05db92b9)
Fonte: o autor
Como pode-se observar o megometro mediu 0,2Mohms, dessa forma, conluimos que o motor doado ao IFSC não está em condições de uso e que precisa de manutenções. De forma semelhante, o intuíto dessa visita na prática é de reproduzir esse procedimento via software unity.



## Desenvolver um software no Unity usando o óculos de realidade virtual com a função hand tracking;


# Cronograma
De acordo com os objetivos apresentados, é necessário criar um cronograma com os períodos de estudo e implementação do projeto. Tendo a consciencia da possibilidade de algumas datas serem alteradas de acordo com o desenvolvimento do projeto.

Clique [aqui](https://github.com/users/JoseVicente2018/projects/1) para acessar o cronograma.

# Lista de materiais

| Item | Descrição | Unidade | Valor Unitário | Quantidade | Total |
| ---- | ------------- | --- | ------------- | ------------- | ------------- |
|  01  | oculus headset quest 2 advanced all-in-one de realidade virtual gmaing vr headset 128 gb branco| 1 | R$ 2.563,00 | 1 | R$ 2.563,00 |

# Unidades curriculares envolvidas

- Progamação I e II;
- Computação cientifica;
- Conversão eletromecanica de energia 1.
  

