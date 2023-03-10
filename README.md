<h1 align="center">
    <a href="ufg.br"><img src="https://github.com/MilleniumSAT/wiki/blob/main/figures/milleniumlogo.png?raw=true" alt="MILLENIUMSAT" width="30%"></a>
    <br>
    MilleniumSAT (ST-OBSAT-01)
    <br>
</h1>

<h4 align="center">Repositório da documentação técnica e teórica da missão.</h4>

<p align="center">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in%20development-red?style=for-the-badge">
	</a>
    <a href="">
		<img src="https://img.shields.io/badge/spacelab%20members-8-blue?style=for-the-badge">
	</a>
	<a href="#license">
		<img src="https://img.shields.io/badge/open--source-project-lightgray?style=for-the-badge">
	</a>
	<a href="">
		<img src="https://img.shields.io/badge/sourced%20by-UFG-orange?style=for-the-badge">
	</a>
	<a href="">
		<img src="https://img.shields.io/badge/sourced%20by-OBSAT-red?style=for-the-badge">
	</a>
</p>

## Motivação

A MilleniumSAT é uma missão desenvolvida com o propósito de estudo da Anomalia Magnética do Atlântico Sul.

A Anomalia Magnética do Atlântico Sul (AMAS) é uma área localizada na região do Oceano Atlântico, próxima à costa do Brasil e da África, onde ocorre uma redução significativa na intensidade do campo magnético terrestre em relação a outras regiões do planeta. Essa anomalia foi descoberta em 1958, durante a missão militar americana "Operation Argus", que tinha como objetivo monitorar explosões nucleares atmosféricas.

A AMAS é um fenômeno que intriga cientistas de todo o mundo, já que não existe uma explicação clara para sua origem. Uma das teorias mais aceitas é que a anomalia é causada pela presença de um grande volume de material líquido na região, como o magma presente em vulcões submarinos. Outra possibilidade é que a AMAS seja uma consequência da dinâmica do núcleo terrestre, que é composto principalmente de ferro e níquel, e que gera o campo magnético do planeta.

A importância da AMAS se deve ao fato de que ela interfere na navegação de aviões e navios, uma vez que o campo magnético é utilizado como referência para a orientação. Além disso, a anomalia tem sido estudada por cientistas que buscam entender melhor o funcionamento do campo magnético terrestre e sua relação com os processos geológicos e geofísicos.

Recentemente, foi descoberto que a AMAS está se expandindo em direção à América do Sul, o que tem gerado preocupação entre os cientistas e autoridades. Acredita-se que essa expansão possa ter implicações em diversos aspectos, como a segurança das redes elétricas e de comunicações, além de impactar a navegação e a aviação na região.

Essa proposta foi trabalhada durante a 1º Olimpíada Brasileira de Satélites, e será efetivamente lançada em um lançamento orbital em meados de dezembro de 2023*.

<p align="center">
    <img width="65%" src="https://github.com/MilleniumSAT/wiki/blob/main/figures/pcb-01.png?raw=true" />
</p>

## Objetivo da missão

1. Coletar dados da magnetosfera a fim de ampliar os estudos em relação à Anomalia Magnética do Atlântico Sul.
2. Validar a utilização de um algoritmo de localização e mapeamento do campo magnético chamado Magnetic SLAM.
3. Validar a utilização do sensor magnético de baixo custo RM3100 para missões em cubesats 1U.
4. Analisar a influência de interferências eletromagnéticas no uso do sensor.
5. Enviar os dados adquridos através do subsistema de telemetria utilizando frequências radio-amadoras.
6. Servir como inspiração para futuras missões originárias do Núcleo de Pesquisas Aeroespaciais da Universidade Federal de Goiás.

## Requisitos da missão

1. Deverá haver disponibilidade de um barramento CAN e USART para comunicação do microcontrolador sampler com o OBC
2. Necessidade de uma alimentação 3.3V e 5V
3. Deverá haver um barramento através de conectores header (PC104)
4. Deverá haver previsão de fornecimento de potencia para (580mW) em atividade
5. Deverá haver disponibilidade um andar inteiro para o payload
6. A comunicação entre o computador de bordo e payload deverá seguir o protocolo desenvolvido
7. A órbita deverá estar entre 500~600km de altitude, preferenciamente
8. A inclinação orbital deverá ser 35º e 60º

## Mission Schedule

| Início  | Fim | Fase                                                                                          |
|------------------|------------------|-----------------------------------------------------------------------------------------------------------|
| T-304d             | T-265d             | Início do desenvolvimento do payload Millenium                   |
| T-264d               | T-243d           | Data de entrega da lista de componentes/sensores/PCB necessários para o desenvolvimento do payload.   |
| T-242d                | T-157d           | Data de entrega do firmware para integração com o computador de bordo.                               |
| T-156d                | T-150d            | Data limite para integração do satélite

> T = Dezembro de 2023*

## Desenvolvimento 

As seções a seguir descrevem os subsistemas de missão. 

<p align="center">
  <img width="65%" src="https://github.com/MilleniumSAT/wiki/blob/main/figures/diagrama1.png?raw=true" />
</p>

<br><br>

<a href="https://github.com/MilleniumSAT/stmillenium-32-firmware/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=MilleniumSAT/stmillenium-32-firmware" />
</a>

## Payload Millenium (AMAS)

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in%20development-red?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/obdh2/releases">
		<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/MilleniumSAT/stmillenium-32-firmware?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/obdh2/commits/master">
		<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/MilleniumSAT/stmillenium-32-firmware?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/obdh2/issues">
		<img alt="GitHub issues" src="https://img.shields.io/github/issues/MilleniumSAT/stmillenium-32-firmware?style=for-the-badge">
	</a>
</p>

<a href="https://github.com/spacelab-ufsc/obdh2">
<img align="right" width="25%" src="https://github.com/MilleniumSAT/wiki/blob/main/figures/pcb-02.png?raw=true">
</a>

O payload Millenium é um das duas cargas úteis da missão ST-OBSAT-01. Seu principal objetivo consiste em obter dados sensoriais de um magnetômetro de baixo custo para analisar o comportamento da Anomalia Magnética do Atlântico Sul e implementar o algoritmo Magnetic SLAM em seu processamento. Composto por um microcontrolador STM32L0 e contando com protocolos de comunicação SPI, I2C, CAN e USART, o payload também é capaz de armazenar seus dados adquiridos em uma memória EEPROM de 512kB.
Além disso, a placa possui um sensor magnetômetro RM3100 e um sensor de temperatura TMP100.

<br><br>

## Parceiros

#### CEIA (Centro de Excelência em Inteligência Artificial)

<p float="left">
  	<a href="">
  		<img src="https://github.com/MilleniumSAT/wiki/blob/main/figures/logo.5b8ba38120642953aba9.png?raw=true" width="37%" />
  	</a>
</p>

#### UFG (Universidade Federal de Goiás)

<p float="left">
    <a href="">
        <img src="https://github.com/MilleniumSAT/wiki/blob/main/figures/Marca_UFG_cor_vertical-03.png?raw=true" width="30%" />
    </a>
</p>

#### EMC (Escola de Engenharia Elétrica, Mecânica e Computação)/UFG 

<p float="left">
  	<a href="">
  		<img src="https://github.com/MilleniumSAT/wiki/blob/main/figures/Screenshot_from_2023-03-07_22-54-49-removebg-preview.png?raw=true" width="23%" />
  	</a> 
</p>

#### INF (Instituto de Informática)/UFG

<p float="left">
  	<a href="">
  		<img src="https://github.com/MilleniumSAT/wiki/blob/main/figures/banner-wiki-transparent.png?raw=true"/>
  	</a>
</p>
