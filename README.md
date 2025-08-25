# Landing Page Solar com Notion CMS

Uma landing page moderna e responsiva para captura de leads utilizando vídeo incorporado da plataforma VTurb, com integração ao Notion como CMS.

## 🚀 Funcionalidades

- **Design Responsivo**: Otimizado para todos os dispositivos
- **CMS Notion**: Conteúdo dinâmico carregado via API do Notion
- **Loading States**: Estados de carregamento elegantes
- **SEO Otimizado**: Meta tags e estrutura semântica

## 📋 Configuração

### 1. Variáveis de Ambiente

Crie um arquivo `.env` baseado no `.env.example`:

```env
VITE_NOTION_TOKEN=seu_token_secreto_do_notion
VITE_NOTION_DATABASE_ID=seu_database_id_do_notion
```

### 2. Configuração do Notion

Crie uma database no Notion com as seguintes propriedades:

- `slug` (Text) - Use "landing" para a página principal
- `video_embed_code` (Text) - Parte do código de incorporação do vturb
- `video_script_url` (URL) - Parte do código de incorporação do vturb
- `sobre_mim_texto` (Text) - Texto descritivo personalizado

### 3. Token do Notion

1. Acesse [Notion Developers](https://www.notion.so/my-integrations)
2. Crie uma nova integração
3. Copie o token secreto
4. Compartilhe sua database com a integração criada

### 4. Deploy no Netlify

1. Conecte seu repositório ao Netlify
2. Configure as variáveis de ambiente no painel do Netlify
3. O formulário será automaticamente processado pelo Netlify Forms

## 🛠️ Desenvolvimento

```bash
# Instalar dependências
npm install

# Iniciar servidor de desenvolvimento
npm run dev

# Build para produção
npm run build
```


## 🎨 Personalização

- Cores no arquivo `style.css` (variáveis CSS)
- Conteúdo estático pode ser editado diretamente no HTML
- Conteúdo dinâmico é gerenciado pelo Notion

## 📊 Estrutura do Projeto

```
├── index.html          # Página principal
├── style.css           # Estilos e responsividade
├── .env.example        # Exemplo de configuração
└── README.md           # Documentação
```

## 🌟 Recursos Incluídos

- **Index principal**: Com vídeo incorporado do vturb via notion
- **Seção de Quem sou eu**: vinda da database do notion
- **Rodapé**: Botão de contato via whatsapp

## 🚀 Performance

- Carregamento otimizado de imagens
- CSS minificado e otimizado
- JavaScript modular
- Fallbacks para conteúdo offline
- Loading states para melhor UX

## 📞 Suporte

Para dúvidas ou problemas, consulte a documentação do Notion API e Netlify Forms.