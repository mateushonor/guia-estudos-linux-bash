# Comando `chsh`

O comando `chsh` significa **change shell** e permite alterar o shell padrão de um usuário no sistema Linux.

O shell padrão é o programa que será iniciado automaticamente quando o usuário fizer login no sistema.

---

# Verificando o shell atual

Podemos verificar qual shell está sendo utilizado com o comando:

```bash
echo $SHELL
```

Exemplo de saída

```bash
/bin/bash
```

Isso indica que o shell atual é o Bash.

---

# Alterando o shell padrão

Para alterar o shell padrão usamos o comando chsh com a opção -s.
```bash
chsh -s /bin/bash
```

Esse comando define o Bash como shell padrão para o usuário.

Depois da alteração, o novo shell será utilizado na próxima sessão de login.

---

# Verificando shells disponíveis no sistema

Os shells disponíveis no sistema são listados no arquivo:
```bash
cat /etc/shells
```
Exemplo de saída
```bash
/bin/sh
/bin/bash
/bin/zsh
/bin/dash
```
Esses são os shells que podem ser configurados como padrão.

---

# Exemplo usando outro shell

Se quisermos alterar para o Zsh, por exemplo:
```bash
chsh -s /bin/zsh
```
Depois de fazer logout e login novamente, o sistema iniciará usando o Zsh.

---

# Resumo
Comando	Função
```bash
echo $SHELL	--->mostra o shell atual
chsh -s /bin/bash	--->altera o shell padrão
cat /etc/shells	---> mostra os shells disponíveis
```
