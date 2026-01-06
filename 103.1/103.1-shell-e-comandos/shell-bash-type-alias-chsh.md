# Shell Bash — type, alias e chsh

Este módulo aborda conceitos fundamentais do shell Bash
e como o sistema interpreta comandos digitados no terminal.

O objetivo é compreender:

- como o Bash identifica um comando
- a diferença entre builtin, alias e executável
- quando usar `type`, `which` e `whereis`
- como alterar e identificar o shell padrão do usuário
- como testar os comandos na prática no terminal

---

## 🖥️ Como este material deve ser usado

Os comandos devem ser:

1) executados no terminal Linux  
2) observados e analisados  
3) registrados neste arquivo como evidência de prática

📌 O GitHub armazena as anotações  
📌 O terminal é o laboratório

Este repositório funciona como:

✔ guia de estudo  
✔ caderno técnico  
✔ registro de experiência prática

---

## 🔹 O que é o Shell Bash

O Bash é um **interpretador de comandos**.

Ele:

1. recebe o comando digitado  
2. interpreta o conteúdo  
3. decide o que executar  
4. envia a ação ao sistema

Exemplos básicos:

```bash
ls
pwd
whoami
