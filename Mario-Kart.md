# 🏁 Mario Kart.JS — Simulador de Corrida

<p align="center">
  <img src="./docs/header.gif" alt="Mario Kart Banner" width="300"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-CommonJS-339933?style=for-the-badge&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-ES2022-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/status-concluído-brightgreen?style=for-the-badge" />
</p>

---

## 📖 Sobre o Projeto

**Mario Kart.JS** é uma simulação de corrida inspirada na famosa série da Nintendo, desenvolvida em JavaScript puro com Node.js. O projeto implementa mecânicas de dado, atributos de personagens e blocos de pista aleatórios para simular uma corrida completa de 5 rodadas no terminal.

> Desafio de projeto proposto pelo **Felipão** 🎮

---

## 🎮 Personagens

| Personagem | Imagem | Velocidade | Manobrabilidade | Poder |
|:----------:|:------:|:----------:|:---------------:|:-----:|
| **Mario** | <img src="./docs/mario.gif" width="50"/> | 4 | 3 | 3 |
| **Peach** | <img src="./docs/peach.gif" width="50"/> | 3 | 4 | 2 |
| **Yoshi** | <img src="./docs/yoshi.gif" width="50"/> | 2 | 4 | 3 |
| **Bowser** | <img src="./docs/bowser.gif" width="50"/> | 5 | 2 | 5 |
| **Luigi** | <img src="./docs/luigi.gif" width="50"/> | 3 | 4 | 4 |
| **Donkey Kong** | <img src="./docs/dk.gif" width="50"/> | 2 | 2 | 5 |

---

## 🕹️ Regras & Mecânicas

### Estrutura da Corrida
- A corrida é disputada entre **2 personagens** ao longo de **5 rodadas**
- A cada rodada, um **bloco de pista** é sorteado aleatoriamente

### Tipos de Bloco

| Bloco | Atributo Usado | Resultado |
|:-----:|:--------------:|:---------:|
| 🛣️ **Reta** | Velocidade + Dado (d6) | Quem somar mais ganha **+1 ponto** |
| 🔄 **Curva** | Manobrabilidade + Dado (d6) | Quem somar mais ganha **+1 ponto** |
| 🥊 **Confronto** | Poder + Dado (d6) | Quem perder, perde **-1 ponto** |

### Regras Gerais
- 🎲 O dado utilizado é de **6 lados**
- 🚫 Nenhum jogador pode ter **pontuação negativa** (mínimo: 0)
- 🏆 Vence quem acumular **mais pontos** ao final das 5 rodadas

---

## 🚀 Como Executar

### Pré-requisitos

- [Node.js](https://nodejs.org/) instalado (v14+)

### Instalação

```bash
# Clone o repositório
git clone https://github.com/Markin11-Dev/simulador-mario-kart.git

# Acesse a pasta do projeto
cd simulador-mario-kart

# Não há dependências externas — basta rodar!
node index.js
```

### Exemplo de Saída

```
🏁🚨 Corrida entre MARIO e LUIGI começando...

🏁 Rodada 1
Bloco: RETA
MARIO 🎲 rolou um dado de velocidade 5 + 4 = 9
LUIGI 🎲 rolou um dado de velocidade 3 + 3 = 6
MARIO marcou um ponto!
-----------------------------
🏁 Rodada 2
Bloco: CONFRONTO
MARIO confrontou com LUIGI! 🥊
...
-----------------------------
Resultado final:
MARIO: 3 ponto(s)
LUIGI: 2 ponto(s)

MARIO venceu a corrida! Parabéns! 🏆
```

---

## 📁 Estrutura do Projeto

```
simulador-mario-kart/
├── index.js          # Lógica principal do jogo
├── package.json      # Configurações do projeto
├── docs/
│   ├── header.gif
│   ├── mario.gif
│   ├── luigi.gif
│   ├── bowser.gif
│   ├── peach.gif
│   ├── yoshi.gif
│   ├── dk.gif
│   └── toad.gif
└── README.md
```

---

## 🛠️ Tecnologias Utilizadas

- **JavaScript** (ES2022)
- **Node.js** (CommonJS)
- Programação **assíncrona** com `async/await`
- Lógica de **aleatoriedade** com `Math.random()`

---

## ✅ Funcionalidades Implementadas

- [x] Dois personagens competindo com atributos distintos
- [x] Sorteio aleatório de blocos de pista (Reta, Curva, Confronto)
- [x] Sistema de pontuação com proteção contra pontos negativos
- [x] Log detalhado de cada rodada no terminal
- [x] Declaração do vencedor ao final da corrida

---

## 🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-mecanica`)
3. Commit suas alterações (`git commit -m 'feat: adiciona nova mecânica'`)
4. Push para a branch (`git push origin feature/nova-mecanica`)
5. Abra um Pull Request

---

## 📄 Licença

Este projeto está sob a licença **ISC**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---


