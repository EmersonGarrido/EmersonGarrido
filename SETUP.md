# Promise Hub — README Profile Template

## Como Usar

### 1. Crie um repositorio com o mesmo nome do seu usuario

No GitHub, crie um repositorio com **exatamente o mesmo nome** do seu username.
Exemplo: se seu username e `EmersonGarrido`, crie o repo `EmersonGarrido/EmersonGarrido`.

### 2. Copie os arquivos deste template

Copie o `README.md` e a pasta `.github/` para o seu repositorio.

### 3. Configure o Secret

No seu repositorio, va em **Settings > Secrets and variables > Actions** e adicione:

- **Nome:** `PROMISE_HUB_README_URL`
- **Valor:** A URL da API que aparece no painel do Promise Hub em **Settings > README**

A URL tem o formato:
```
http://45.55.188.250:3001/api/readme/raw?userId=SEU_USER_ID&token=SEU_TOKEN
```

### 4. Execute o workflow

Va em **Actions > Update README with Promise Hub** e clique em **Run workflow**.

O workflow tambem roda automaticamente todos os dias as 6h UTC.

### 5. Personalize

No painel do Promise Hub em `/settings/readme`, voce pode:
- Ativar/desativar secoes (linguagens, horario, commits, etc.)
- Ver um preview do README gerado
- Copiar o markdown diretamente

## Requisitos

- Conta no Promise Hub com dados coletados (hook do Claude Code, extensao VS Code)
- Conta GitHub conectada ao Promise Hub (para dados de repos e commits)
