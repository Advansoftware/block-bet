# 🛡️ Advans Blocklist

Lista personalizada de bloqueio para **Pi-hole** e **AdGuard Home**, focada em bloquear domínios de anúncios, rastreamento e conteúdos indesejados.  
Atualizada automaticamente a partir de fontes confiáveis.

---

## 📌 URL da Lista

Use este link direto para adicionar no seu Pi-hole ou AdGuard Home:

```
https://raw.githubusercontent.com/Advansoftware/block-bet/main/advans-blocklist.txt
```

---

## 🚀 Como Usar

### 📍 Pi-hole
1. Acesse **Settings → Adlists** no painel do Pi-hole.
2. Clique em **Add a new adlist** e insira:
   ```
   https://raw.githubusercontent.com/Advansoftware/block-bet/main/advans-blocklist.txt
   ```
3. Salve e rode no terminal:
   ```bash
   pihole -g
   ```

---

### 📍 AdGuard Home
1. Vá em **Filtros → Regras de filtragem personalizadas**.
2. Clique em **Adicionar filtro** e insira:
   ```
   https://raw.githubusercontent.com/Advansoftware/block-bet/main/advans-blocklist.txt
   ```
3. Clique em **Aplicar**.

---

## 📂 Formato da Lista
- Um domínio por linha (exemplo: `example.com`).
- Sem prefixos como `0.0.0.0` ou `127.0.0.1` — Pi-hole e AdGuard processam automaticamente.
- Sem espaços extras.

---

## 🔄 Atualização Automática
Esta lista é atualizada diariamente através de **GitHub Actions** que:
1. Baixam listas de bloqueio de fontes confiáveis.
2. Filtram e removem duplicatas.
3. Sobrescrevem `advans-blocklist.txt` com a nova versão.
4. Publicam a lista automaticamente neste repositório.

Você sempre terá a **versão mais recente** sem precisar atualizar manualmente.

---

## 📥 Fontes Utilizadas
- [StevenBlack/hosts](https://github.com/StevenBlack/hosts)
- [oisd.nl](https://oisd.nl)
- Outras fontes personalizadas

---

## ⚠️ Aviso
- Esta lista pode bloquear alguns domínios legítimos.
- Use por sua conta e risco.
- Caso um site importante seja bloqueado, adicione-o à whitelist do seu Pi-hole ou AdGuard.

---

## 🤝 Contribuindo
- Envie **Pull Requests** para sugerir novos domínios ou remover falsos positivos.
- Ou abra uma **Issue** descrevendo o problema.

---

## 📄 Licença
Distribuída sob a licença **MIT**.  
Você pode usar, modificar e distribuir livremente.

---
