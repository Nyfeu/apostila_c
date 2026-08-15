## 1. Histórico

Desenvolver um novo circuito a cada novo projeto consome muito tempo e recursos. Visto isso, o engenheiro [[Frederico Faggin]], da [[Intel]], desenvolveu um circuito com um conjunto de operações que podem ser executadas numa sequência definida e armazenada numa memória. Essa mudança de perspectiva muda a abordagem através de circuitos eletrônicos digitais (como [[Circuitos Combinacionais]] e [[Circuitos Sequenciais]]) para a utilização de processadores.

O primeiro produto comercial desse tipo desenvolvido  foi o chip [[Intel 4004]], para integrar a calculadora BUSICOM 141-PF. 

![[intel_4004.png|313]]

Ele foi lançado em 1971, possuindo uma arquitetura de 4 bits e 45 instruções diferentes. Sua frequência de operação (_clock_) máxima era de 740 kHz.

O uso apenas de microprocessadores não é suficiente para desenvolver um circuito integrado completo para aplicações em sistemas embarcados por si só. Portanto, foram criados os microcontroladores. Esse novo tipo de circuito foi projetado para integrar no mesmo substrato a ROM (_Ready-Only Memory_ - associada às instruções); a RAM (_Random-Access Memory_ - associada aos dados) e registradores digitais para interface com dispositivos externos.

## 2. Unidade de Processamento

A unidade de processamento, ou simplesmente processador, é o centro de um microcontrolador. É ela quem coordena, executa e gerencia todos os recursos disponíveis. Essa unidade, por sua vez, é um circuito digital sequencial - ou seja, o estado atual e os dados definem qual será o próximo estado que o circuito assumirá. 

Essas mudanças de estados são realizadas de forma síncrona de acordo com um sinal periódico chamado _clock_. O tempo entre dois estados é chamado de ciclo. 

![[estado_microcontrolador.png|470]]

Mais sobre o projeto e detalhamento sobre processadores é visto em [[Arquitetura de Computadores]]. 