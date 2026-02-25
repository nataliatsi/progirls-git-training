# 💜 Tutorial – Como usar o Git no desafio `git-training`

Repositório do desafio:
🔗 [https://github.com/nataliatsi/progirls-git-training](https://github.com/nataliatsi/progirls-git-training)

---

## Clonar o repositório

Após instalar e configurar o Git, abra:

* **VS Code** (terminal interno)
  ou
* **Git Bash**

Digite:

```bash
git clone https://github.com/nataliatsi/progirls-git-training.git
```

O Git vai baixar o repositório do GitHub para sua máquina.

![Git clonando repositório](/progirls-git-training/assets/image2.png)

Você verá que uma nova pasta chamada `progirls-git-training` foi criada.

![Pasta com projeto](/progirls-git-training/assets/image.png)

---

## Entrar na pasta do projeto

Use o comando abaixo para listar arquivos e pastas:

```bash
ls
```

Agora entre na pasta:

```bash
cd progirls-git-training
```

![Listar e entrar na pasta do projeto](/progirls-git-training/assets/image3.png)

---

## Criar uma branch

⚠️ Nunca trabalhe direto na `main`.

Crie uma branch com seu nome ou seguindo o padrão `feat/seu-nome`.

Sim, atenção Clarisses 😹

```bash
git checkout -b feat/seu-nome
```

Exemplo:

```bash
git checkout -b feat/natalia-apresentacao
```

---

## Fazer as modificações

Agora faça as alterações solicitadas no desafio:

* Editar o README (se apresente)

---

## Adicionar as alterações

Veja o que foi modificado:

```bash
git status
```

Adicione os arquivos:

```bash
git add .
```

Ou um arquivo específico:

```bash
git add nome-do-arquivo.md
```

### Usando o VS Code

No VS Code é possível adicionar ou remover alterações da Staging Area (área de preparação do commit).

> A **Staging Area** é a área onde você escolhe quais alterações irão entrar no próximo commit.
> Só o que estiver no stage será versionado quando você rodar `git commit`.

![Visualizar alterações](/progirls-git-training/assets/image4.png)

* O botão + adiciona a alteração ao stage

* É possível adicionar arquivos individualmente ou todos de uma vez

---

## Fazer o commit

Sempre siga os padrões técnicos definidos no guia.

Exemplo:

```bash
git commit -m "feat: adiciona apresentação da Natália"
```

---

## Enviar sua branch para o GitHub

```bash
git push origin nome-da-sua-branch
```

Exemplo:

```bash
git push origin feat/natalia-apresentacao
```

---

## Abrir Pull Request (PR)

Após o push:

1. Vá até o seu repositório no GitHub.
2. Clique em **Compare & Pull Request**
3. Confirme:

   * Base: `main`
   * Compare: sua branch
4. Escreva título e descrição seguindo o padrão do guia.
5. Clique em **Create Pull Request**

Agora é só esperar a aprovação 💜

---

## Manter sua branch atualizada

Antes de começar novas alterações, atualize sua branch:

```bash
git checkout main
git pull origin main
```

Depois volte para sua branch:

```bash
git checkout nome-da-sua-branch
git merge main
```

---

## 🚨 Importante

* ❌ Não fazer commit direto na `main`
* ❌ Não editar direto pelo GitHub
* ✅ Sempre trabalhar em branch
* ✅ Seguir padrão de commits
* ✅ Seguir padrão de PR
* ✅ Manter sua branch atualizada

Os padrões técnicos estão disponíveis no guia 💜
