# 🖱️ Automação de Cadastro de Produtos com PyAutoGUI

Este projeto tem como objetivo demonstrar o uso da biblioteca `pyautogui` para automatizar o processo de cadastro de produtos em um formulário web (Google Forms). A automação inclui a abertura do navegador, carregamento do formulário e preenchimento automático dos campos com base em um arquivo CSV.

---

## 📦 Bibliotecas Utilizadas

- [`pyautogui`](https://pyautogui.readthedocs.io/en/latest/): Permite controlar o mouse e o teclado para automações visuais.
- [`time`](https://docs.python.org/3/library/time.html): Utilizado para controlar intervalos entre as ações.
- [`pandas`](https://pandas.pydata.org/): Manipulação de dados estruturados (CSV neste caso).

---

## 🧠 Funcionamento

### 1. Marcar Posição do Mouse

Antes de executar a automação, o ideal é mapear as posições do mouse nos elementos a serem clicados. Utilize o código abaixo para isso:

#### python
- import pyautogui
- import time

- time.sleep(5)  # Tempo para posicionar o mouse
- print(pyautogui.position())  # Retorna a posição atual do cursor
---
### ⚠️ Possíveis Erros e Soluções
- ❗ FailSafeException
- O erro abaixo ocorre quando o mouse é movido para algum dos cantos da tela (medida de segurança do PyAutoGUI):

- Solução:
- Evite mover o mouse para os cantos durante a execução. Se desejar desativar a proteção (não recomendado)
