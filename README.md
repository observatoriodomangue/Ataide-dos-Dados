# Observatório do Mangue - Bot WhatsApp Ataíde dos Dados

## Objetivo
O sistema foi criado para facilitar a **coleta de dados ambientais colaborativos** e disponibilizar uma interface de comunicação simples entre comunidades, pesquisadores e a inteligência artificial. Ele possibilita:

- Registrar impactos ambientais com **localização, descrição, data e fotos**.
- Enviar imagens de **espécies de plantas e animais** encontradas no manguezal.
- Interagir com a **IA do Observatório do Mangue**, que responde a perguntas sobre ecossistemas, conservação e sociobiodiversidade.
- Encerrar conversas automaticamente em casos de inatividade para melhor controle de sessões.

## Funcionalidades principais

1. **Menu inicial interativo**
   - 1️ Enviar imagem de impacto ambiental
   - 2️ Falar com a inteligência artificial
   - 3️ Enviar foto de bicho ou planta
   - 4️ Encerrar conversa

2. **Registro de impactos ambientais**
   - Solicita localização geográfica 
   - Solicita data do evento 
   - Solicita descrição textual 
   - Solicita foto para comprovação 
   - Todos os dados são armazenados em planilhas Excel (`dados.xlsx`).

3. **Registro de espécies**
   - Usuário envia foto de planta ou animal.
   - Pode incluir legenda ou nome popular/científico.
   - Dados armazenados em `especies.xlsx`.

4. **Integração com Inteligência Artificial**
   - Usuário pode enviar perguntas para a IA.
   - Sistema retorna resposta automática.
   - Usuário permanece nesse modo até digitar "voltar".

5. **Controle de sessão**
   - Sessão expira após 10 minutos de inatividade .
   - Usuário pode encerrar manualmente com a opção 4.

## Estrutura de Arquivos

- `index.js` → Código principal do bot.
- `src/api.js` → Função responsável por integrar com a IA.
- `dados.xlsx` → Base de dados dos impactos ambientais.
- `especies.xlsx` → Base de dados de espécies enviadas.
- `qrcode.png` → Imagem gerada para autenticação no WhatsApp.

## Como executar

1. Clone este repositório:

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Execute o bot:
   ```bash
   node index.js
   ```

4. Escaneie o QR Code gerado no terminal ou no arquivo `qrcode.png`.

## Tecnologias utilizadas

- **Node.js** → Backend do sistema.
- **WPPConnect** → Conexão com o WhatsApp.
- **ExcelJS** → Manipulação de planilhas Excel.
- **IA integrada** → Respostas automáticas para usuários.

## Armazenamento de dados

Os dados são organizados em planilhas Excel:

- `dados.xlsx` → Impactos ambientais (latitude, longitude, data, descrição e imagem).
- `especies.xlsx` → Registro de espécies (legenda e imagem).

Isso permite fácil integração com sistemas de monitoramento, análises estatísticas e visualizações futuras.

## Contribuidores

- **Yago de Jesus** – Desenvolvimento de software, IA e backend.
- Equipe Observatório do Mangue 🌱

## Licença

Este projeto é distribuído sob a licença MIT.  
Consulte o arquivo [LICENSE] para mais detalhes.
