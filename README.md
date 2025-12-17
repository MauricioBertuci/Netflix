# Netflix

Landing page estática que replica visualmente a página inicial da Netflix usando apenas HTML e CSS. O projeto serve como exercício de maquetagem, estudo de layout responsivo simples e referência visual para experimentos de estilização.

## Visão geral
- **Stack:** HTML5 + CSS3 (sem dependências externas ou build tools).
- **Público-alvo:** pessoas desenvolvedoras iniciantes que querem praticar estruturação de páginas e estilização; instrutores que precisam de um exemplo minimalista para aulas.
- **Status:** protótipo estático, sem integrações ou comportamento dinâmico.

## Estrutura do projeto
```
.
├── Imagens/          # Ativos estáticos usados no layout (background, ícones e ilustrações)
├── index.html        # Estrutura principal da página
├── style.css         # Estilos globais e seções da página
└── README.md         # Este guia
```

## Pré-requisitos
- Navegador moderno.
- Qualquer servidor HTTP simples (opcional, mas recomendado para evitar problemas de CORS ao carregar as imagens). Exemplos: `python -m http.server`, extensões como Live Server ou a funcionalidade "Go Live" do VS Code.

## Como rodar localmente (<= 10 minutos)
1. Clone o repositório e acesse a pasta do projeto:
   ```bash
   git clone <URL_DO_REPOSITORIO>
   cd Netiflix
   ```
2. Inicie um servidor estático na raiz do projeto (use uma das opções abaixo):
   - Python 3 embutido:
     ```bash
     python -m http.server 8000
     ```
   - Ou, se preferir outra porta:
     ```bash
     python -m http.server 3000
     ```
   - Qualquer alternativa equivalente (Live Server/Go Live) também funciona.
3. Abra o navegador em `http://localhost:8000` (ou na porta escolhida) e a landing page será exibida.

> Dica: basta abrir o `index.html` diretamente no navegador, mas um servidor evita alertas de segurança ao carregar imagens locais.

## Componentes principais
- **Cabeçalho (`header`):** logotipo e seletor de idioma simples.
- **Hero (`.home` / `.title`):** chamada principal com campo de e-mail e CTA.
- **Painel de destaques (`.quadro` / `.item`):** quatro cartões com imagens e textos.
- **Rodapé (`footer`):** links informativos, seletor de idioma e contato.

## Estilos e comportamento
- Plano de fundo com `background-image` e sobreposição em gradiente para contraste do texto.
- Layout flexível nos blocos de destaque (`.quadro`) permitindo quebra de linha em telas menores.
- Nenhum JavaScript ou fonte externa é carregado; toda a estilização está em `style.css`.

## Variáveis de ambiente
- Não há variáveis de ambiente ou arquivos de configuração adicionais.

## Testes e lint
- Não há pipeline de testes ou lint configurados. Como o projeto é estático, valide visualmente no navegador.

## Deploy
- Por ser um site estático, o deploy pode ser feito em qualquer serviço de hosting de arquivos estáticos (GitHub Pages, Netlify, Vercel, S3, etc.).
- Basta publicar os arquivos `index.html`, `style.css` e a pasta `Imagens/` mantendo a mesma estrutura de diretórios.

## Contribuição
1. Crie um fork ou branch de trabalho.
2. Mantenha a estrutura simples (HTML/CSS puro) e evite adicionar dependências desnecessárias.
3. Faça commits claros e abra um pull request descrevendo as mudanças.

## Licença
O repositório não declara uma licença explícita. Consulte o(a) responsável antes de usar em produção.
