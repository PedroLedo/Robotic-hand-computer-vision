# 🤖 Mão Robótica Controlada por Visão Computacional

> Projeto educacional de uma mão robótica controlada por **visão computacional**, desenvolvido com foco em **baixo custo, acessibilidade e reprodução por estudantes**.

Este repositório tem como objetivo documentar o desenvolvimento de uma mão robótica capaz de interpretar movimentos realizados pelo usuário por meio de uma câmera e transformar essas informações em movimentos correspondentes da mão robótica.

O projeto foi desenvolvido com uma abordagem **open source**, permitindo que estudantes, professores, pesquisadores e entusiastas possam reproduzir o projeto, compreender seu funcionamento e desenvolver suas próprias versões.

---

## 📌 Sobre o projeto

A proposta consiste em utilizar **visão computacional** para identificar a posição e/ou os movimentos da mão humana.

As informações capturadas pela câmera são processadas por um software responsável por interpretar os movimentos e gerar os comandos necessários para controlar os atuadores da mão robótica.

De forma simplificada:

```text
┌──────────────┐
│    Câmera    │
└──────┬───────┘
       │
       ▼
┌─────────────────────┐
│ Visão Computacional │
│  Detecção da mão    │
└─────────┬───────────┘
          │
          ▼
┌─────────────────────┐
│ Interpretação dos   │
│     movimentos      │
└─────────┬───────────┘
          │
          ▼
┌─────────────────────┐
│ Controlador / MCU   │
└─────────┬───────────┘
          │
          ▼
┌─────────────────────┐
│     Atuadores       │
│ Servos / Motores    │
└─────────┬───────────┘
          │
          ▼
┌─────────────────────┐
│    Mão Robótica     │
└─────────────────────┘
```

---

## 🎯 Objetivos

### Objetivo principal

Desenvolver uma mão robótica controlada por visão computacional, utilizando tecnologias acessíveis e uma documentação que permita a reprodução do projeto por outros estudantes.

### Objetivos específicos

* Desenvolver a estrutura mecânica da mão robótica;
* Implementar o sistema de acionamento dos dedos;
* Desenvolver o sistema de visão computacional;
* Identificar os movimentos da mão humana;
* Converter os movimentos identificados em comandos para os atuadores;
* Integrar hardware e software;
* Desenvolver uma interface de comunicação entre o computador e o sistema embarcado;
* Documentar o projeto de forma didática;
* Possibilitar que outros estudantes reproduzam e aprimorem o projeto.

---

## 🧠 Como funciona?

O sistema utiliza uma câmera para capturar os movimentos realizados pela mão do usuário.

O software de visão computacional analisa a imagem capturada e identifica características da mão, como a posição dos dedos e suas articulações.

A partir dessas informações, o sistema determina quais movimentos devem ser realizados pela mão robótica.

O controlador recebe os comandos e aciona os atuadores responsáveis pelo movimento dos dedos.

### Fluxo de funcionamento

```text
Mão humana
    ↓
Câmera
    ↓
Processamento da imagem
    ↓
Detecção da mão
    ↓
Identificação dos dedos
    ↓
Cálculo dos movimentos
    ↓
Comandos de controle
    ↓
Microcontrolador
    ↓
Atuadores
    ↓
Mão robótica
```

---

## 🛠️ Tecnologias utilizadas

O projeto pode utilizar diferentes tecnologias dependendo da versão desenvolvida.

### Software

* Python
* OpenCV
* Bibliotecas de visão computacional
* Algoritmos de detecção e rastreamento da mão

### Hardware

* Microcontrolador
* Servomotores e/ou outros atuadores
* Câmera
* Fonte de alimentação
* Estrutura mecânica
* Componentes eletrônicos

> ⚠️ A lista definitiva de componentes e suas especificações será apresentada na documentação de montagem.

---

## 📦 Componentes

A quantidade e o modelo dos componentes podem variar de acordo com a versão da mão robótica.

| Componente           | Quantidade | Função                 |
| -------------------- | ---------: | ---------------------- |
| Microcontrolador     |          1 | Controle dos atuadores |
| Câmera               |          1 | Captura dos movimentos |
| Servomotores         |  A definir | Movimentação dos dedos |
| Fonte de alimentação |          1 | Alimentação do sistema |
| Estrutura da mão     |          1 | Estrutura mecânica     |
| Cabos                |          — | Conexões elétricas     |
| Outros componentes   |          — | Dependendo da versão   |

---

## 🔧 Montagem

A montagem do projeto será dividida em etapas para facilitar a reprodução.

### 1. Estrutura mecânica

Montagem da estrutura responsável por representar os dedos, palma e demais componentes mecânicos.

### 2. Instalação dos atuadores

Os servomotores ou outros atuadores devem ser instalados de forma que seus movimentos sejam transmitidos aos dedos da mão robótica.

### 3. Circuito eletrônico

Realização das conexões entre o microcontrolador, atuadores e fonte de alimentação.

### 4. Programação

Configuração do firmware responsável pelo controle dos atuadores.

### 5. Sistema de visão computacional

Instalação das bibliotecas necessárias e configuração do software responsável pela identificação dos movimentos da mão.

### 6. Integração

Por fim, o sistema de visão computacional será conectado ao sistema embarcado para permitir o controle da mão robótica.

---

## 💻 Instalação

Clone este repositório:

```bash
git clone https://github.com/SEU-USUARIO/mao-robotica-visao-computacional.git
```

Entre na pasta:

```bash
cd mao-robotica-visao-computacional
```

Instale as dependências necessárias:

```bash
pip install -r requirements.txt
```

Execute o programa:

```bash
python main.py
```

> Os comandos acima serão atualizados conforme a estrutura definitiva do projeto.

---

## 🎮 Controle

Após iniciar o sistema, a câmera deverá ser posicionada de maneira que a mão do usuário esteja visível.

O software realizará a detecção da mão e utilizará as informações obtidas para gerar os comandos destinados à mão robótica.

A calibração inicial poderá ser necessária para ajustar os limites de movimento de cada dedo.

---

## 📁 Estrutura do repositório

```text
mao-robotica-visao-computacional/
│
├── README.md
│
├── software/
│   ├── main.py
│   ├── vision/
│   └── control/
│
├── hardware/
│   ├── circuitos/
│   ├── esquemas/
│   └── componentes/
│
├── mechanical/
│   ├── modelos-3d/
│   └── desenhos/
│
├── docs/
│   ├── montagem/
│   ├── configuracao/
│   └── testes/
│
└── requirements.txt
```

---

## 🧪 Testes

Durante o desenvolvimento serão realizados testes para avaliar:

* Detecção da mão;
* Identificação dos dedos;
* Precisão dos movimentos;
* Tempo de resposta;
* Comunicação entre computador e microcontrolador;
* Movimento dos atuadores;
* Sincronização entre mão humana e mão robótica;
* Confiabilidade do sistema.

Os resultados dos testes serão documentados neste repositório.

---

## 🚧 Status do projeto

**Em desenvolvimento 🚧**

O projeto está sendo desenvolvido e documentado progressivamente.

Novas informações, códigos, esquemas elétricos, modelos mecânicos e procedimentos de montagem serão adicionados conforme o desenvolvimento avançar.

---

## 📚 Documentação

A documentação será organizada para permitir que uma pessoa com conhecimentos básicos de eletrônica, programação e robótica consiga acompanhar o projeto desde o início.

Em breve:

* [ ] Guia de componentes
* [ ] Esquema elétrico
* [ ] Montagem mecânica
* [ ] Arquivos 3D
* [ ] Configuração do microcontrolador
* [ ] Instalação do software
* [ ] Configuração da visão computacional
* [ ] Calibração
* [ ] Testes
* [ ] Solução de problemas

---

## 🎓 Projeto educacional

Este projeto foi desenvolvido com o propósito de servir também como **material educacional**.

A documentação busca possibilitar que estudantes de diferentes níveis possam:

* compreender os princípios de visão computacional;
* aprender conceitos de robótica;
* desenvolver sistemas embarcados;
* estudar eletrônica;
* trabalhar com programação;
* integrar diferentes áreas da engenharia;
* reproduzir o projeto;
* modificar e melhorar o sistema.

A ideia não é apenas disponibilizar o resultado final, mas também **documentar o processo de desenvolvimento**, incluindo decisões, testes, erros e melhorias.

---

## 🤝 Contribuições

Contribuições são bem-vindas!

Você pode contribuir através de:

* Correções;
* Melhorias no código;
* Melhorias mecânicas;
* Otimizações;
* Novas funcionalidades;
* Documentação;
* Sugestões;
* Relatos de problemas.

Para contribuir, faça um *fork* do projeto, realize suas alterações e envie um *pull request*.

---

## ⚠️ Aviso

Este projeto possui finalidade **educacional e experimental**.

A reprodução do projeto deve considerar as características dos componentes utilizados, principalmente em relação à alimentação elétrica, corrente dos atuadores e limites mecânicos da estrutura.

Sempre verifique as especificações dos componentes antes de realizar a montagem.

---

## 📜 Licença

Este projeto será disponibilizado sob uma licença open source.

> A licença será definida conforme a versão final do projeto.

---

## 👨‍💻 Autor

**Pedro Ledo**

Projeto desenvolvido no contexto de estudos e desenvolvimento tecnológico em **Automação, Robótica e Visão Computacional**.

---

⭐ Se este projeto for útil para você, considere deixar uma estrela no repositório e compartilhar com outros estudantes.

**Construa. Teste. Erre. Melhore. Compartilhe.**
