# Ocupacional Consultoria & Serviços — site

Site estático (HTML único, sem dependências) da Ocupacional Consultoria & Serviços, Marabá-PA.

## Estrutura
- `index.html` — página completa (CSS e JS embutidos)
- `logo-ocupacional.svg` — logo vetorizada standalone

## Deploy no VPS (CloudPanel)
1. No CloudPanel: **Sites → Add Site → Static HTML Site**, domínio `ocupacionalsst.com.br` (ou temporário).
2. Via SSH, na pasta do site:
   ```bash
   cd /home/<usuario-do-site>/htdocs/<dominio>
   rm -rf ./*
   git clone https://github.com/Gabriel-lima22/ocupacional-site.git .
   ```
3. Ative o SSL (Let's Encrypt) no CloudPanel.

## Atualizar depois
```bash
cd /home/<usuario-do-site>/htdocs/<dominio> && git pull
```
