# 🚀 Projeto Escola - ETEC Irmã Augustina

## 🎯 Objetivo
Desenvolver uma página web em grupo, aplicando conceitos de HTML, CSS, JavaScript e GitHub colaborativo, utilizando um fluxo de trabalho muito próximo do mercado.

---

## 🌳 Branches principais:
- `main` → Produção e Deploy (**GitHub Pages**)
- `develop` → Integração das features

### 🚧 Branches de desenvolvimento:
- `feature/nome-da-feature` → Cada grupo cria sua própria branch para desenvolver uma parte do site.

---

## 🔥 Fluxo de trabalho:

1️⃣ **Clonar o repositório:**
```bash
git clone https://github.com/alevitorio/git-project.git
````

2️⃣ **Criar sua branch de feature:**

```bash
git checkout -b feature/nome-da-feature
```

3️⃣ **Desenvolver sua parte.**

4️⃣ **Fazer commit e push na sua branch:**

```bash
git add .
git commit -m "feat: adiciona nome-da-feature"
git push origin feature/nome-da-feature
```

5️⃣ **Abrir Pull Request para a branch `develop`:**

* Base: `develop`
* Compare: `feature/nome-da-feature`

6️⃣ Quando tudo estiver funcionando, fazemos um Pull Request de `develop` para `main`.

7️⃣ A branch `main` faz o deploy automático no **GitHub Pages**.

---

## 🛑 Regras importantes:

* ❌ Nunca fazer push direto na `main`.
* ❌ De preferência, também não fazer push direto na `develop` (usar Pull Request).
* ✅ Sempre trabalhar na sua própria branch.
* ✅ Antes de abrir um Pull Request, sincronizar sua branch:

```bash
git checkout develop
git pull
git checkout feature/nome-da-feature
git merge develop
```

---

## 🔥 Checklist dos alunos:

* [ ] Clonar o repositório
* [ ] Criar uma branch de feature
* [ ] Fazer commits claros e objetivos
* [ ] Push na sua branch
* [ ] Abrir Pull Request para `develop`
* [ ] Participar do merge final para `main`

---

## 🚀 GitHub Pages:

➡️ [https://alevitorio.github.io/git-project](https://alevitorio.github.io/git-project)

---

## 💡 Desenvolvido pelos alunos da **ETEC Irmã Augustina**, orientados pelo professor **Alessandro — AleDev 🚀**



---

## 📝 **Template de Pull Request**

## ✨ Descrição da Feature
Descreva de forma clara o que foi desenvolvido.

## 🔗 Relacionado a:
- [ ] Nenhuma Issue
- [ ] Issue #Número (se tiver)

## ✅ Checklist antes do merge:
- [ ] Código testado localmente
- [ ] Segue o padrão de pastas e arquivos
- [ ] Sem conflitos com a branch develop
- [ ] Commit bem descrito

## 📸 Screenshot (se aplicável):
Adicione imagens mostrando o funcionamento da feature.

---

## 🗺️ **Diagrama do Fluxo de Branches**


+-------------------------+
|       feature/X         |
+-------------------------+
           ↓  Pull Request
+-------------------------+
|        develop          |
+-------------------------+
           ↓  Pull Request
+-------------------------+
|          main           |
| (Deploy GitHub Pages)   |
+-------------------------+

