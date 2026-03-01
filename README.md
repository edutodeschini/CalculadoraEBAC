# 🧮 Calculadora

Uma calculadora simples de linha de comando feita em Python.

## Funcionalidades

- Soma, subtração, multiplicação e divisão
- Loop contínuo: realize várias operações sem reiniciar o programa

## Requisitos

- Python 3

## Como usar

**Via Python diretamente:**
```bash
python3 calculadora.py
```

**Via script Shell:**
```bash
chmod +x calculadora.sh
./calculadora.sh
```

## Como funciona o código

O código é estruturado em torno de um loop principal que mantém a calculadora rodando até o usuário decidir sair.

**1. Variável de controle**

A variável `ligada = True` controla o loop. Enquanto for `True`, a calculadora continua funcionando.

**2. Entrada de dados**

A cada rodada, o programa solicita dois números (convertidos para `int`) e a operação desejada.

**3. Execução da operação**

Um bloco `if/elif` verifica qual operação foi digitada (`+`, `-`, `*`, `/`) e exibe o resultado. Caso o usuário digite algo inválido, exibe "Operacao invalida".

**4. Continuar ou sair**

Ao final de cada cálculo, o programa pergunta se o usuário quer realizar outra operação:
- `s` → continua o loop
- `n` → define `ligada = False`, encerrando o programa
- qualquer outra coisa → exibe "Opcao invalida" e pergunta novamente na próxima iteração

---

## Exemplo de uso

```
Digite um numero: 10
Digite outro numero: 5
Digite a operacao(+, -, *, /): *
10 * 5 =
50
Deseja realizar outra operação?(s/n): n
Obrigado por usar a calculadora!
```
