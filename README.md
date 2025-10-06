# Mangrove Observatory – Ataíde dos Dados WhatsApp Bot

## Objective
The system was created to facilitate the collaborative **collection of environmental data** and provide a simple communication interface between communities, researchers, and artificial intelligence. It enables users to:
- Record environmental impacts with **location, description, date, and photos**.
- Send images of **plant and animal species** found in the mangrove ecosystem.
- Interact with the **Mangrove Observatory’s AI**, which answers questions about ecosystems, conservation, and sociobiodiversity.
- Automatically end inactive conversations for better session control.
- 
## Main Features

1. **Interactive Main Menu**
   - 1️ Send image of an environmental impact
   - 2️ Talk to artificial intelligence
   - 3️ Send photo of an animal or plant
   - 4️ End conversation

2. **Environmental Impact Recording**
   - Requests geographic location
   - Requests event date
   - Requests textual description
   - Requests a photo as evidence
   - All data are stored in Excel spreadsheets (`dados.xlsx`).

3. **Species Recording**
   - The user sends a photo of a plant or animal.
   - May include a caption or popular/scientific name.
   - Data are stored in `especies.xlsx`.

4. **Integration with Artificial Intelligence**
   - The user can send questions to the AI.
   - The system returns an automatic response.
   - The user remains in this mode until typing “back”.

5. **Session Control**
   - Session expires after 10 minutes of inactivity.
   - The user can manually end the session with option 4.

## File Structure

- `index.js` → Main bot code.
- `src/api.js` → Function responsible for AI integration.
- `dados.xlsx` → Environmental impact database.
- `especies.xlsx` → Species record database.
- `qrcode.png` → Image generated for WhatsApp authentication.

## How to Run

1. Clone this repository:

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the bot:
   ```bash
   node index.js
   ```

4. Scan the QR Code generated in the terminal or in the file `qrcode.png`.

## Technologies Used

- **Node.js** → System backed.
- **WPPConnect** → WhatsApp connection.
- **ExcelJS** → Excel spreadsheet management.
- **Integrated IA** → Automatic user responses.

## Data Storage

The data are organized in Excel spreadsheets:

- `dados.xlsx` → Environmental impacts (latitude, longitude, date, description, and image).
- `especies.xlsx` → Species records (caption and image).

This structure allows for easy integration with monitoring systems, statistical analyses, and future visualizations.

## Contributors

- **Yago de Jesus Martins** – Conceptualization, Software development, AI, and backend.
- **Indira Eyzaguirre** - Data validation and project management
- **Mangrove Researchers** - Mangrove Observatorio´s team 🌱

## License

This project is distributed under the MIT License.
See the [LICENSE] file for more details.
