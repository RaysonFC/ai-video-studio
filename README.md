# AI Video Studio — Fase 1
Aplicação React/Vite PWA responsiva. Não gera vídeo nesta fase; exporta configurações JSON para futura integração Wan. Dados locais por navegador, sem login ou sincronização. Imagens são redimensionadas para até 1280 px e comprimidas para armazenamento local, sujeito a quota.

## Publicar sem computador
1. Extraia o ZIP. No GitHub, crie um repositório ai-video-studio.
2. Envie os arquivos e pastas internos preservando src/ e public/ (no celular, use a versão desktop do navegador se necessário; se o seletor não aceitar pastas, crie os arquivos nos caminhos correspondentes pelo editor do GitHub).
3. No Netlify, Add new project > Import an existing project > GitHub. Autorize e selecione o repositório.
4. Build command: npm run build. Publish directory: dist. Base directory: vazio. Deploy.
5. Abra a URL HTTPS em ambos os aparelhos. Chrome: menu Instalar aplicativo; iOS Safari: Compartilhar > Adicionar à Tela de Início.

## Executar no PC
Node.js 22, npm install, npm run dev. Para testar PWA: npm run build && npm run preview. Service worker ativo apenas na versão de produção. Offline depende de cache após acesso online.

## Backup
Configurações > Exportar backup; importe no outro aparelho. A importação substitui os dados locais. Não envie imagens privadas ao GitHub.

## Próxima fase
Backend autenticado com GPU, upload, fila, status e download MP4. Nenhum segredo de API deve ficar no frontend.
