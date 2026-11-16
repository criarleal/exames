Warning: truncated output (original token count: 1720)
Total output lines: 97

# Dossiê Clínico & Radiológico Evolutivo (2023 - 2026)
### Paciente anonimizado

---

## 🎯 Visão Geral do Projeto

Este projeto foi construído para organizar, correlacionar e apresentar ao médico assistente (especialmente urologista e clínico) a totalidade do histórico de saúde do paciente, com foco primário na **investigação da elevação aguda do PSA para 7,94 ng/mL em 09/11/2026**.

O portal laboratorial disponibilizava apenas um laudo evolutivo incompleto, que omitia anos fundamentais, exames hormonais intermediários e a totalidade dos exames de imagem. Este dashboard integra **100% dos dados reais** contidos nos PDFs e disponibiliza um **visualizador ultrassonográfico profissional (PACS-style)** com as 28 capturas radiológicas dos exames de 17/10/2026.

---

## 🚀 Como Visualizar Localmente (Imediato)

1. Basta **dar dois cliques no arquivo `index.html`** nesta pasta para abri-lo em qualquer navegador (Google Chrome, Microsoft Edge, Firefox, Safari).
2. O aplicativo é **100% autônomo e autocontido** — todos os dados laboratoriais, regras de estilo e laudos estão embutidos diretamente no código, não exigindo instalação de nenhum servidor.

*(Opcional: Caso prefira rodar via servidor local leve, execute no terminal PowerShell: `py -m http.server 8000` e acesse `http://localhost:8000`).*

---

## 🌐 Como Publicar no GitHub Pages (Passo a Passo)

Para disponibilizar este painel online com link direto para o seu médico:

1. Abra o terminal nesta pasta (`c:\PATH_Programs\Downloads\postar\programas\Exames`).
2. Inicialize o repositório Git e faça o commit inicial:
   ```bash
   git init
   git add .
   git commit -m "Dossie medico anonimizado - PSA e imagens"
   ```
3. Crie um novo repositório (público ou privado) na sua conta do GitHub (ex: `dossie-medico`).
4. Conecte o repositório remoto e envie os arquivos:
   ```bash
   git branch -M main
   git remote add origin h…720 tokens truncated…am apagadas do laudo evolutivo gerado pelo site.
2. **Basal de PSA:** O laudo do site ocultou que o paciente possuía PSA estável de 0,47 ng/mL em 2023 e 0,60 ng/mL em 2024.
3. **Relação Livre/Total:** Não calculada pelo laboratório (17,25% em 2026 vs 74,47% em 2023).
4. **Hormônios Fundamentais:** FSH (0,4 mUI/mL - suprimido), DHT (55, 52,7 e 65,2 ng/dL), Testosterona Livre e Biodisponível, Progesterona.
5. **Inflamação e Metabolismo:** Ferritina elevada (336,4 e 464,4 ng/mL), Insulina e HOMA-IR (3,05 - resistência insulínica), Vitamina D (19,7 ng/mL), enzimas hepáticas e perfil lipídico.
6. **Exames de Imagem:** O portal laboratorial não exibe nenhuma menção aos dois laudos ultrassonográficos nem às 28 imagens radiológicas.

---

## 🔬 Recursos do Visualizador Ultrassonográfico (PACS)

- **Modos de Exibição:** Modo Único e Modo Comparação Lado a Lado (Split-Screen).
- **Controles Radiológicos:** Pan & Zoom contínuo na roda do mouse, inversão de cores (Modo Negativo / Filme de Raio-X), controle deslizante de brilho e contraste, rotação 90° e tela cheia.
- **HUD Técnico & Calipers:** Sobreposição em tempo real do transdutor (C5-1 Convexo vs eL18-4 Linear), modo Doppler colorido, frequência acústica e medidas exatas marcadas pelo radiologista (ex: volumetria testicular 7,0 e 7,6 cm³; calibres venosos ao repouso e Valsalva).
- **Filmstrip:** Carrossel inferior de miniaturas para navegação instantânea.
- **Atalhos de Teclado:** Setas `◀`/`▶` (frames), `+`/`-` (zoom), `0` (ajustar), `R` (reset), `I` (negativo), `C` (comparar), `F` (tela cheia).

---

## 🖨️ Impressão & Exportação para o Médico

- Basta clicar no botão azul **"Imprimir Dossiê para o Médico"** no topo da página ou pressionar `Ctrl + P`.
- A folha de estilos `@media print` oculta todos os botões e abas da interface web e diagrama automaticamente um **relatório médico formal em papel A4**, perfeito para entregar em mãos na consulta urológica!


