# 📘 Assignment: Primeiros passos com testes automatizados em Python

## 🎯 Objective

Aprenda a verificar automaticamente o comportamento de funções Python usando `pytest`. Você escreverá testes simples, executará a suíte e ampliará a cobertura com casos-limite.

## 📝 Tasks

### 🛠️ Escreva e execute seu primeiro teste

#### Descrição
Instale o `pytest` com `python -m pip install pytest` e crie um arquivo chamado `test_starter_code.py`. Escreva um teste para confirmar que `add_two_numbers(2, 3)` retorna `5`.

#### Requisitos
O programa concluído deve:

- Usar o arquivo `starter-code.py` como módulo sob teste.
- Nomear o arquivo de teste `test_starter_code.py` para que o `pytest` o encontre.
- Usar `assert` para verificar o resultado de `add_two_numbers(2, 3)`.
- Executar o teste com `python -m pytest -q` e observar que ele passa.


### 🛠️ Teste resultados diferentes

#### Descrição
Adicione testes para a função `is_even`, verificando um número par e um número ímpar.

#### Requisitos
O programa concluído deve:

- Verificar que `is_even(4)` retorna `True`.
- Verificar que `is_even(5)` retorna `False`.
- Executar novamente todos os testes e confirmar que passam.


### 🛠️ Cubra casos-limite

#### Descrição
Amplie os testes de `is_even` para conferir como a função se comporta com zero e números negativos.

#### Requisitos
O programa concluído deve:

- Verificar que `is_even(0)` retorna `True`.
- Verificar que `is_even(-2)` retorna `True` e `is_even(-3)` retorna `False`.
- Executar a suíte completa com `python -m pytest -q` e confirmar que todos os testes passam.