# Guia Prático para Baixar Vídeos da Hotmart  

## Passo a Passo Simplificado  

### 1. Instale a extensão "FetchV"  
- Adicione ao seu navegador para capturar links de vídeos da Hotmart.  
- **Link da extensão**: [FetchV](https://fetchv.net) *(substitua pelo link real)*  

---

### 2. Verifique o yt-dlp  
- Certifique-se de ter o **[yt-dlp](https://github.com/yt-dlp/yt-dlp)** instalado.  
- **Comando de instalação** (se necessário):  
  ```bash
  pip install yt-dlp
  ```


### 3. Acesse o vídeo desejado  
1. Abra a página do vídeo na Hotmart.  
2. Atualize a página (`F5`), dê *play* no vídeo e **pause-o assim que começar**.  

---

### 4. Use a extensão FetchV  
1. Clique no ícone da FetchV no navegador.  
2. Copie o **URL da playlist principal** (geralmente a primeira das 3 opções).  

---

### 5. Execute o comando no terminal  
- Abra o **CMD** ou **PowerShell** e cole o comando abaixo:  
  ```bash
  yt-dlp -o "NOME-DO-VIDEO.mp4" --add-headers Referer:https://player.hotmart.com/ --format best[height=1080] "LINK-DO-VIDEO"
  ```  
  - **Substitua**:  
    - `NOME-DO-VIDEO`: Nome desejado para o arquivo (ex: `Aula-01`).  
    - `LINK-DO-VIDEO`: Link copiado da FetchV.  

---

## Exemplo Prático  
```bash
yt-dlp -o "Marketing-Digital.mp4" --add-headers Referer:https://player.hotmart.com/ --format best[height=1080] "https://exemplo.com/playlist_principal"
```

---

## Dicas Importantes  
- Mantenha as **aspas** ao redor do nome do vídeo e do link.  
- Para alterar a qualidade, ajuste `height=1080` (ex: `height=720`).  

> ⚠️ **Nota**: Garanta que o yt-dlp está atualizado com o comando `yt-dlp -U`.  
