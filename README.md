````markdown
# 🚀 Projeto Escola - ETEC Irmã Augustina

## 🎯 Objetivo
Desenvolver uma página web em grupo, aplicando conceitos de HTML, CSS, JavaScript e Git colaborativo, utilizando um fluxo de trabalho muito próximo do mercado.

---

## 🌳 Branches principais:
- `main` → Produção e Deploy (**GitHub Pages**)
- `develop` → Integração das features (todos trabalham diretamente nela)

### 🚧 Branches de desenvolvimento:
- `feature/nome-da-feature` → Cada grupo cria sua própria branch local para desenvolver sua parte.

---

## 🔥 Fluxo de trabalho:

1️⃣ **Clonar o repositório:**
```bash
git clone https://github.com/alevitorio/git-project.git
````

2️⃣ **Criar sua branch de feature localmente (opcional):**

```bash
git checkout -b feature/nome-da-feature
```

3️⃣ **Desenvolver sua parte.**

4️⃣ **Sincronizar com a develop (caso precise):**

```bash
git checkout develop
git pull
git checkout feature/nome-da-feature
git merge develop
```

Ou:

```bash
git rebase develop
```

5️⃣ **Integrar seu trabalho na `develop`:**

* Pode fazer **merge** da sua feature na `develop`:

```bash
git checkout develop
git merge feature/nome-da-feature
git push origin develop
```

Ou:

* Pode aplicar **rebase** e depois push:

```bash
git checkout develop
git pull
git rebase feature/nome-da-feature
git push origin develop
```

6️⃣ Quando a `develop` estiver estável e finalizada, abrir um **Pull Request da `develop` para `main`**.

7️⃣ A `main` faz o deploy no **GitHub Pages**.

---

## 🔥 Merge ou Rebase?

✔️ **Merge:** Junta sua branch na develop com um commit de merge. Simples, rápido e seguro.

✔️ **Rebase:** Deixa o histórico mais limpo e linear. Atualiza sua branch como se ela tivesse sido criada após as mudanças mais recentes da develop. Requer atenção em conflitos.

**Na dúvida? Use merge.**

---

## 🛑 Regras importantes:

* ❌ Nunca fazer push direto na `main`.
* ✅ Na `develop` é permitido push, merge e rebase.
* ✅ Sempre trabalhar em sua própria branch local antes de integrar.
* ✅ Resolver conflitos se aparecerem durante merge ou rebase.
* ✅ O único Pull Request acontece de `develop` para `main`.

---

## 🔥 Checklist dos alunos:

* [ ] Clonar o repositório
* [ ] Criar uma branch local de feature (opcional)
* [ ] Desenvolver sua parte
* [ ] Fazer push na `develop` (via merge ou rebase)
* [ ] Participar do Pull Request de `develop` para `main`

---

## 🚀 GitHub Pages:

➡️ [https://alevitorio.github.io/git-project](https://alevitorio.github.io/git-project)

---

## 💡 Desenvolvido pelos alunos da **ETEC Irmã Augustina**, orientados pelo professor **Alessandro — AleDev 🚀**

````

---

## 📝 **Template de Pull Request (para PR da `develop` para `main`)**
```markdown
## ✨ O que foi feito:
- Descrever brevemente o que está sendo entregue para produção.

## ✅ Checklist:
- [ ] Testado e funcionando localmente
- [ ] Todos os arquivos estão corretos
- [ ] A develop está funcionando sem erros

## 🚀 Observações:
- Descreva qualquer ponto importante

---
````

---

## 🗺️ **Diagrama do Fluxo de Branches — Atualizado**

```plaintext
+-------------------------+
|  feature/nome-da-feature| (local)
+-------------------------+
           ↓  merge ou rebase (direto)
+-------------------------+
|        develop          | (Push livre)
+-------------------------+
           ↓  Pull Request
+-------------------------+
|          main           | (Deploy GitHub Pages)
+-------------------------+
```

