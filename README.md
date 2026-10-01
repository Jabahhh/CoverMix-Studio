CoverMix Studio

<img width="873" height="955" alt="1" src="https://github.com/user-attachments/assets/e5e2d9c6-8e33-42e0-8dc7-9f177a009c6a" />
<img width="640" height="640" alt="2" src="https://github.com/user-attachments/assets/20984737-49e3-49db-b7ce-8f92428f6bc7" />

# CoverMix Studio — Game Cover Generator

**CoverMix Studio** é uma ferramenta portátil para geração automatizada de capas 3D e conversão de mídia para front-ends retro como **RetroBat** e **Batocera**.

O programa combina screenshots, capas 2D, mídias (cartuchos/discos) e logos em artes prontas no formato final do sistema escolhido.

---

## 🎨 Principais Recursos

- **Geração de Capas 3D Personaliadas**: Monte arte em 3D ajustada ao formato exato de cada console (incluindo variações como *3DO* e *3DO Long Box*).
- **Suporte Inteligente a Mídia**: Altera automaticamente entre *Cartucho* e *Disco* com base no console selecionado.
- **Modos de Tela**: Alterne facilmente entre proporções SD (4:3 com efeito CRT) e HD (16:9).
- **Processamento em Lote**: Arraste múltiplos arquivos ou pastas inteiras para emparelhamento automático de assets.
- **Conversor Integrado de Thumbs**: Redimensione imagens para as dimensões exatas de cada sistema com opções para manter a proporção, esticar ou cortar.
- **Interface e Configurações Persistentes**: Temas Claro e Escuro, suporte multi-idioma (Português/Inglês) e salvamento automático das suas preferências.

---

## 📖 Como Usar

### 📌 Aba "Gerar Capas"
1. **Arraste seus assets**: Solte imagens ou pastas nos campos correspondentes: *Screenshot (Obrigatório)*, *Capa 2D*, *Imagem de disco*, *Cartucho* e *Logo*.
   > *Nota*: O programa ativa dinamicamente apenas o campo válido para o console selecionado (Cartucho vs. Disco), marcando o outro como não utilizado.
2. **Emparelhamento**: Arquivos com o mesmo nome são associados automaticamente. Se você soltar um arquivo de cada tipo por vez, eles serão pareados sequencialmente.
3. **Ajustes de Renderização**: Escolha o console alvo e a proporção da tela (SD ou HD).
4. **Exportação**: As capas geradas são salvas com o sufixo `<nome>-image.png` na pasta de saída configurada (Padrão: `Área de Trabalho\CoverMix Studio`).

### 🔄 Aba "Converter Imagens"
1. Arraste as imagens ou a pasta com suas mídias.
2. Selecione o console desejado (as dimensões em pixels aparecerão ao lado).
3. Ajuste o método de redimensionamento (Manter proporção com fundo transparente, Esticar ou Cortar para preencher).
4. As imagens convertidas serão salvas com o sufixo `<nome>-thumb.png`.

---

## ⚙️ Personalização de Consoles

Caso precise ajustar ou adicionar novos perfis de consoles, edite o arquivo `covermix_studio.py`:

- **Tabela `CONSOLES`**: Define as proporções e direções da lombada 3D `(nome, largura, altura, lombada, lado, cor)`.
- **Lista `CART_CONSOLES`**: Contém a relação dos sistemas que utilizam cartuchos ao invés de discos.
- **Tabela `THUMB_SIZES`**: Define os tamanhos de saída no conversor de miniaturas.

---

## 💾 Configurações do Usuário

As preferências do usuário (tema, idioma, console preferido, pastas de saída, etc.) são salvas em:
`%APPDATA%\CoverMix Studio\settings.json`

Para redefinir a aplicação para o estado padrão de fábrica, basta excluir o arquivo `settings.json`.

=========================
=========================

English version:


CoverMix Studio — Game Cover Generator

CoverMix Studio is a portable tool for automated 3D cover generation and media conversion for retro front-ends like RetroBat and Batocera.

The program combines screenshots, 2D covers, media (cartridges/discs), and logos into ready-to-use artwork tailored to the target system.

🎨 Key Features

Custom 3D Cover Generation: Create 3D artwork adjusted to the exact dimensions of each console (including variations like 3DO and 3DO Long Box).

Smart Media Support: Automatically switches between Cartridge and Disc based on the selected console.

Screen Modes: Easily toggle between SD (4:3 with CRT effect) and HD (16:9) aspect ratios.

Batch Processing: Drag and drop multiple files or entire folders for automatic asset pairing.

Built-in Thumb Converter: Resize images to the exact dimensions of each system with options to keep aspect ratio, stretch, or crop.

Interface & Persistent Settings: Light and Dark themes, multi-language support (Portuguese/English), and automatic saving of your preferences.

📖 How to Use

📌 "Generate Covers" Tab

Drag your assets: Drop images or folders into the corresponding fields: Screenshot (Required), 2D Cover, Disc Image, Cartridge, and Logo.

Note: The program dynamically enables only the valid field for the selected console (Cartridge vs. Disc), marking the other as unused.

Pairing: Files with the same name are automatically paired. If you drop one file of each type individually, they will be paired sequentially.

Render Settings: Choose the target console and screen ratio (SD or HD).

Exporting: Generated covers are saved with the <name>-image.png suffix in the configured output directory (Default: Desktop\CoverMix Studio).

🔄 "Convert Images" Tab

Drag and drop your images or media folder.

Select the desired console (pixel dimensions will appear next to it).

Choose the resize method (Keep aspect ratio with transparent background, Stretch, or Crop to fill).

Converted images will be saved with the <name>-thumb.png suffix.

⚙️ Console Customization

If you need to adjust or add new console profiles, edit the covermix_studio.py file:

CONSOLES Table: Defines the proportions and spine orientation for 3D covers (name, width, height, spine, side, color).

CART_CONSOLES List: Contains the list of systems that use cartridges instead of discs.

THUMB_SIZES Table: Defines the output sizes for the thumbnail converter.

💾 User Settings

User preferences (theme, language, preferred console, output folders, etc.) are saved in:
%APPDATA%\CoverMix Studio\settings.json

To reset the application to its default factory state, simply delete the settings.json file.
