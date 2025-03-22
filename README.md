# 🧠 Servidor de Cálculo Distribuído com Sockets e Multithreading

Este projeto tem como objetivo demonstrar a criação de um servidor capaz de processar operações matemáticas enviadas por múltiplos clientes simultaneamente, utilizando **Sockets** e **Multithreading** em Python.

## 🗂️ Estrutura do Repositório

```
📁 calculadora-distribuida/
├── servidor.py              # Código do servidor com suporte a múltiplos clientes via threads
├── cliente_operacao.py      # Cliente interativo que permite envio de operações via terminal
├── cliente_testes.py        # Script que simula múltiplas conexões concorrentes ao servidor
├── README.md                # Documentação do projeto
```

## 🧩 Objetivo

Desenvolver um sistema cliente-servidor com as seguintes funcionalidades:

- O **servidor** escuta uma porta específica e aceita conexões de múltiplos clientes.
- Cada conexão de cliente é tratada em uma **thread separada**.
- Os clientes enviam **operações matemáticas** (como `2 + 3`, `10 / 2`, etc.).
- O servidor processa a operação e retorna o resultado.

## ⚙️ Tecnologias Utilizadas

- 🐍 Python 3.x
- 🧵 Módulo `threading`
- 🔌 Módulo `socket`
- 🪵 Módulo `logging` (para registrar atividades do servidor)

## 🚀 Como Executar

### 1. Inicie o servidor

```bash
python servidor.py
```

O servidor ficará ouvindo na porta `65432` do `localhost`.

---

### 2. Execute o cliente interativo

```bash
python cliente_operacao.py
```

Este cliente permite que você envie operações manualmente, uma de cada vez.

---

### 3. (Opcional) Teste múltiplas conexões simultâneas

```bash
python cliente_testes.py
```

Este script simula várias conexões concorrentes ao servidor, enviando operações matemáticas predefinidas.

## 🧪 Exemplos de Operações Suportadas

- `2 + 3`
- `10 / 2`
- `5 * 4`
- `2 ** 3`
- `15 % 4`
- `1 + 2 * 3`
- `(10 + 5) / 3`

## 💡 Considerações Finais
A implementação deste projeto serviu como uma valiosa experiência de aprendizagem, proporcionando uma compreensão prática dos conceitos de comunicação em rede com sockets, execução concorrente com threads e processamento de requisições cliente-servidor.

Foi uma excelente oportunidade para consolidar conhecimentos e exercitar a lógica de programação aplicada a sistemas distribuídos.
