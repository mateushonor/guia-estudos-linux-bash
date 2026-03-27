# Comando type

O comando `type` mostra como o shell interpreta um comando.

Ele informa se o comando é:

- comando interno do shell
- programa executável
- alias
- função

---

# Exemplo

```bash
type ls
```

Saída possível

```bash
ls is /usr/bin/ls
```
Isso significa que o comando ls é um programa executável localizado no diretório /usr/bin/ls.

---

# Verificando um comando interno do shell

Alguns comandos não são programas externos, mas sim comandos internos do Bash.

Podemos verificar isso com:

```bash
type cd
```
Saída

```bash
cd is a shell builtin
```

Isso indica que cd é um comando interno do shell Bash.

---

#Verificando um alias

Se existir um alias configurado no sistema, o comando type mostrará essa informação.

```bash
type ll
```
Saída possível

```bash
ll is aliased to 'ls -alF'
```
Isso significa que ll é um atalho (alias) para o comando ls -alF.

---

# Verificando múltiplos comandos

Também podemos verificar mais de um comando ao mesmo tempo:

```bash
type ls pwd cd
```
Exemplo de saída

```bash
ls is /usr/bin/ls
pwd is a shell builtin
cd is a shell builtin
```
