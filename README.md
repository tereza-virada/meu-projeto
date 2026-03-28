![imagem git](https://hermes.dio.me/articles/cover/d2489f96-d56f-4b82-bc7f-84fbc9fb1368.jpg)

# 🚀 Guia Essencial de Git (do zero ao fluxo profissional)


## 📦 1. Configuração inicial (primeira vez no Git)

Antes de tudo, configure seu usuário:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

Ver configurações:

```bash
git config --list
```

---

## 📁 2. Criar um repositório

### 👉 Criar um repositório local

```bash
git init
```

### 👉 Clonar um repositório existente (GitHub, por exemplo)

```bash
git clone URL_DO_REPOSITORIO
```

---

## 📤 3. Fluxo básico (salvar alterações)

### Ver status do projeto:

```bash
git status
```

### Adicionar arquivos:

```bash
git add .
```

ou específico:

```bash
git add nome-do-arquivo
```

### Criar um commit:

```bash
git commit -m "mensagem do commit"
```

---

## 🌐 4. Conectar com repositório remoto (GitHub)

```bash
git remote add origin URL_DO_REPOSITORIO
```

Ver conexão:

```bash
git remote -v
```

---

## 🚀 5. Subir código (push)

### Primeiro push:

```bash
git push -u origin main
```

Depois:

```bash
git push
```

---

## 🌿 6. Trabalhando com branchs (ESSENCIAL no mercado)

### Criar uma nova branch:

```bash
git branch nome-da-branch
```

### Trocar de branch:

```bash
git checkout nome-da-branch
```

👉 Forma moderna (melhor prática):

```bash
git switch nome-da-branch
```

### Criar e já mudar para a branch:

```bash
git checkout -b nome-da-branch
```

ou:

```bash
git switch -c nome-da-branch
```

### Listar branchs:

```bash
git branch
```

---

## 📤 7. Subir uma branch para o remoto

```bash
git push -u origin nome-da-branch
```

---

## 🔄 8. Atualizar branchs

### Puxar atualizações do repositório remoto:

```bash
git pull
```

### Atualizar sua branch com a main:

```bash
git pull origin main
```

---

## 🔀 9. Fazer merge (juntar branchs)

```bash
git checkout main
git merge nome-da-branch
```

---

## 🧹 10. Deletar branch

### Local:

```bash
git branch -d nome-da-branch
```

### Remota:

```bash
git push origin --delete nome-da-branch
```

---

## ⚠️ 11. Resolver conflitos (resumo prático)

Quando ocorrer conflito:

1. Abra o arquivo
2. Escolha o código correto
3. Depois:

```bash
git add .
git commit -m "resolve conflito"
```

---

## 🧠 12. Fluxo profissional (o que o mercado usa)

👉 Fluxo padrão:

```bash
git checkout main
git pull

git checkout -b minha-feature

# faz alterações
git add .
git commit -m "feat: minha feature"

git push -u origin minha-feature
```

Depois → Pull Request no GitHub

---

## 🔥 Dicas que fazem diferença (nível mercado)

* Use commits claros:

  * `feat:` nova funcionalidade
  * `fix:` correção
  * `refactor:` melhoria de código

* Nunca trabalhe direto na `main`

* Sempre atualize antes de começar (`git pull`)

* Nomeie branches assim:

  * `feature/login`
  * `fix/erro-cadastro`

---

## 💡 Resumo rápido (cola de prova / aula)

```bash
git init
git add .
git commit -m "mensagem"
git remote add origin URL
git push -u origin main

git switch -c nova-branch
git push -u origin nova-branch

git pull
git merge branch
```



