# Comando `alias`

O comando `alias` permite criar **atalhos para comandos no Bash**.

Isso é útil para simplificar comandos longos ou usados com frequência.

Quando um alias é criado, o Bash substitui o alias pelo comando correspondente antes de executá-lo.

---

# Criando um alias

Podemos criar um alias usando a seguinte sintaxe:

```bash
alias nome_do_alias="comando"
```

Exemplo
```bash
alias ll="ls -l"
```
Agora, quando digitarmos:
```bash
ll
```

O Bash executará automaticamente:
```bash
ls -l
```
---

# Criando alias mais completos

Também podemos incluir opções adicionais.

alias la="ls -la"

Agora ao executar:
```bash
la
```

O Bash executará:
```bash
ls -la
```

Esse comando lista todos os arquivos, inclusive os ocultos.

---

# Listando todos os aliases

Para visualizar todos os aliases configurados no shell atual:
```bash
alias
```

Exemplo de saída
```bash
alias ll='ls -l'
alias la='ls -la'
```

Isso mostra todos os atalhos definidos no ambiente do shell.

---

# Verificando um alias específico

Podemos verificar um alias específico usando o comando type.
```bash
type ll
```
Saída possível
```bash
ll is aliased to 'ls -l'
```

Isso indica que ll é um alias para o comando ls -l.

---

# Removendo um alias

Para remover um alias usamos o comando unalias.

```bash
unalias ll
```

Depois disso o alias ll deixará de existir.

---

# Tornando aliases permanentes

Por padrão, os aliases existem apenas na sessão atual do terminal.

Para torná-los permanentes, podemos adicioná-los ao arquivo:

```bash
~/.bashrc
```

Exemplo:
```bash
alias ll="ls -l"
```

Depois de salvar o arquivo, execute:
```bash
source ~/.bashrc
```

Isso recarrega as configurações do shell.

---

# Resumo
Comando	Função
```bash
alias	->cria atalhos para comandos
alias	->lista aliases existentes
unalias	->remove um alias
```
