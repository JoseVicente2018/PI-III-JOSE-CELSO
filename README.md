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

Como pode-se observar o megometro mediu 0,2Mohms, dessa forma, conluimos que o motor doado ao IFSC não está em condições de uso e que precisa de manutenções. De forma semelhante, o intuíto dessa visita na prática é de reproduzir esse procedimento via software unity integrando com o oculus metaquest 2.

## Desenvolver um software no Unity usando o óculos de realidade virtual com a função hand tracking;

Antes de realizar o desenvolvimento do projeto no Unity primeiramente foi criado um procedimento de como deve ser feito o teste no ambiente de realidade virtual e quais materiais que devem nesse ambiente de realidade virtual. Segue o procedimento para o desenvolvimento no unity:
 
 1º passo:
 
Procedimento de segurança:
- Colocar o EPI (luva);
- Desligar o motor no quadro elétrico (on/off) (pode ser 1 led demostrando o status do motor).
Resultado das decisões:
Se o usuário não colocar a luva e for direto ao quadro, ao tentar abrir o quadro, o quadro não se abrirá e aparecerá uma mensagem dizendo que o usuário deverá colocar a luva primerio.
Se o usuário for direto mexer no motor, aparecerá uma mensagem dizendo que ele morreu, e automaticamente voltará pro respawn. 
Se o usuário for direto no megometro e tentar colocar no motor, acontecerá o mesmo que o caso acima.
Se o usuário pegar a luva e tentar e depois tentar mexer no motor ou no megometro (aparecerá uma mensagem, “para sua maior segurança, desligue o disjuntor do motor quadro elétrico)

2º Passo

Disponibilizar para o usuário um quadro ou um informativo da tensão do motor para adequar o megometro à tensão correta; nesse informativo deverá conter a tensão do motor e o quadro segundo a norma de qual tensão ele deverá utilizar no megometro para realizar o teste do motor. 
- Selecionar a tensão no megometro;
- Conectar os jacarés no motor. - Escolher forma de medição:
1ª forma: bobina – chassi :curto circuitar 3 bobinas e conectar o positivo e depois negativo na carcaça (chassi). - 2ª forma: entre bobinas;
- Voltar no megometro e colocar start.
- megometro poderá ter 2 valores diferentes (%) nos dois métodos de ligação do megometro. Um valor muito baixo 1Mohm e o outro valor alto 6Mohms. Nos dois tipos de ligação deverá dar o mesmo valor.

3ª passo retirada do equipamento

Quando o usuário decidir desligar o megometro. Aparecerá, de acordo com os valores medidos, um menu perguntando se o motor está ok ou não.
Se o parâmetro estiver ok. E a pessoa responder ok. Está correto. (Justificar na resposta o do porquê que está certo)
Caso a pessoa colocar ok, e não tiver, aparecerá uma mensagem justificando o porquê que não.
Fim.

O software tem uma comunicação interativa com seu usuário de forma virtual disponibilizando uma infinidade de funções figura 4, no qual, para um iniciante o uso pode parece dificil. Nesse caso, como teve-se o primeiro contato o software unity demandou um certo esforço para entender a demanda basica. 

Figura 4: interface unity.

![image](https://github.com/JoseVicente2018/PI-III-JOSE-CELSO/assets/141693494/bf507e36-5c9b-4681-813a-a9240eba36ac)

O Unity disponibiliza opções de desenvolvimento para criação de projetos, podendo eles serem 2D, 3D, VR, etc. Como nosso caso é para realidade virtual, foi criado no espaço de projeto para VR. 

Para criar o ambiente utilizou-se a ferramente disponível chamada Assets, "Assets" refere-se a todos os recursos que são utilizados em um projeto, como modelos 3D, texturas, scripts, áudio, animações, entre outros. Sendo esses recursos fundamentais para a criação de jogos e aplicações interativas. Utilizando a ferramenta, montou-se o ambiente para teste de verificação de resistência de isolamento de um motor trifasico 

Figura 5 : ambiente para teste de resistência de isolamento do motor

![image](https://github.com/JoseVicente2018/PI-III-JOSE-CELSO/assets/141693494/47549c3a-5c0c-4634-be1d-6db018e3a1ca)

Após montar o ambiente em 3D chegou a hora de realizar de forma interativa com a linguagem de programação C#. Com a programação pode-se realizar uma infinidade de interações com o ambiente de realidade virtual, como exemplo, segurar objetos, cortar, vestir, apertar, gerar numeros, etc. A programação é feita a partir do software visualstudio, o qual no unity é agregado ao objeto. Então, para continuidade do projeto seguiu-se em codigo c# essas intereções. Essas interações e códigos encontra-se no repositório e o programa disponível em APK na área Releases> assets (podendo realizar a trasferencia para o Oculus através do aplicativo sidequest e testar o software criado ( teste de medição de resistência de isolamento do motor trifásico).

 

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
  

