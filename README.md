🎬 Clone da Página de Vídeo do YouTube!
Criei um clone completo da página de reprodução de vídeos do YouTube (/watch) com foco em CSS Flexbox e design responsivo moderno!
🎯 Flexbox em Ação - Estruturas Implementadas:
📱 Header Flexível

display: flex com justify-content: space-between
Seções left, center, right organizadas perfeitamente
Barra de pesquisa expansível com flex: 1

🎬 Layout Principal

Container principal: display: flex para dividir conteúdo/sidebar
Responsivo: Muda para flex-direction: column no mobile
Flexbox aninhado em todos os componentes

⚡ Componentes com Flexbox:
🎥 Video Player & Info:

Player com aspect-ratio 16:9
Metadados organizados com flex
Actions bar com justify-content: space-between

💬 Sistema de Comentários:

Cada comentário usa flex para layout
Input de comentário com avatar + campo expansível
Actions dos comentários alinhados com gap

📋 Sidebar de Vídeos Relacionados:

Grid responsivo que vira flex column no mobile
Cards com thumbnail
🌟 Recursos Avançados Implementados:
🎨 Design Autêntico

Tema escuro idêntico ao YouTube
Cores oficiais: #0f0f0f (background), #ff0000 (YouTube red)
Typography Roboto para fidelidade visual
Gradientes coloridos nos thumbnails e avatares

⚡ Interatividade JavaScript

Play button funcional que simula reprodução
Subscribe button com toggle de estado
Like/Dislike com contador dinâmico
Show more/less na descrição expandível
Comment input com estados focus/blur
Hover effects em todos os elementos clicáveis

📱 Responsividade Completa
css/* Desktop: Layout em duas colunas */
.main-container { display: flex; gap: 24px; }

/* Tablet: Sidebar vira grid */
@media (max-width: 1024px) {
    .main-container { flex-direction: column; }
    .related-videos { 
        display: grid; 
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); 
    }
}

/* Mobile: Layout vertical */
@media (max-width: 768px) {
    .video-actions { flex-direction: column; }
    .related-video { flex-direction: column; }
}
🎯 Flexbox Masterclass - Conceitos Aplicados:
1. Flex Containers Aninhados:
css.header { display: flex; justify-content: space-between; }
  .header-left { display: flex; gap: 16px; }
  .header-center { display: flex; flex: 1; }
    .search-container { display: flex; flex: 1; }
2. Flex Items Responsivos:
css.search-input { flex: 1; } /* Expande */
.search-btn { width: 64px; } /* Fixo */
.secondary-content { width: 402px; flex-shrink: 0; }
3. Alinhamento Perfeito:
css.channel-info { 
    display: flex; 
    align-items: center; 
    gap: 12px; 
}
🔥 Funcionalidades Premium:
✅ Player de vídeo com botão play funcional
✅ Sistema de likes com contador
✅ Subscribe button com toggle
✅ Comentários com avatares e ações
✅ Descrição expandível com timestamps
✅ Vídeos relacionados interativos
✅ Barra de pesquisa funcional
✅ Scrollbar customizada
✅ Animações suaves em hovers
✅ Estados visuais (focus, hover, active)
🎨 Detalhes Visuais Autênticos:

Gradientes únicos para cada thumbnail
Avatars coloridos com gradientes
Ícones usando Unicode para compatibilidade
Spacing consistente seguindo design system
Shadows e borders sutis para profundidade
Transitions suaves em todas as interações

📊 Estrutura Flexbox Hierárquica:
Body
├── Header (flex row)
│   ├── Header-left (flex row)
│   ├── Header-center (flex row)
│   └── Header-right (flex row)
└── Main-container (flex row → column no mobile)
    ├── Primary-content (flex column)
    │   ├── Video-actions (flex row → column no mobile)
    │   ├── Comments (flex column)
    │   └── Each comment (flex row)
    └── Secondary-content (flex column → grid no tablet)
        └── Related-videos (flex column)
Este clone demonstra domínio completo do Flexbox, desde layouts simples até estruturas complexas aninhadas, tudo com responsividade perfeita e interatividade moderna!
🚀 Perfeito para portfólio - mostra habilidades avançadas em CSS, Flexbox, responsividade e JavaScript!
