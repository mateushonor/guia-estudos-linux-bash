
```md
# Execução de comandos — ;  &&  ||

Este módulo estuda como o Bash executa comandos em sequência
e como o comportamento muda conforme o operador utilizado.

O objetivo é compreender:

- execução simples
- execução condicional por sucesso/erro
- diferença entre `;`, `&&` e `||`
- interpretação de código de retorno `$?`
- uso prático em automação e scripts

---

## 🖥️ Como este material deve ser usado

Os comandos devem ser:

1) executados no terminal Linux  
2) analisados em diferentes cenários  
3) registrados neste arquivo como evidência de prática

📌 O GitHub guarda as anotações  
📌 o terminal é o laboratório

---

## 🔹 Operador `;` — executa sempre

Executa todos os comandos,
independentemente de sucesso ou erro.

Exemplo:

```bash
echo "primeiro" ; echo "segundo"
