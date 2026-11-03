# 💬 ChatPulse — WhatsApp Chat Analyzer

A sleek, dark-themed analytics dashboard that transforms your exported WhatsApp chats into rich visual insights — timelines, heatmaps, word clouds, emoji breakdowns, and more.

---

## ✨ Features

| Feature | Description |
|---|---|
| 📊 **Top Statistics** | Total messages, words, media shared, and links |
| 📅 **Monthly Timeline** | Area chart of chat activity over time |
| 🗓️ **Activity Map** | Most active days of the week and months of the year |
| 🔥 **Hourly Heatmap** | Hour-by-day activity matrix to find peak chat times |
| 🏆 **Busiest Users** | Bar chart + percentage table for group chats |
| ☁️ **Word Cloud** | Visual frequency map with Hinglish stop-word filtering |
| 🔤 **Common Words** | Top 20 most used words ranked by frequency |
| 😄 **Emoji Analysis** | Emoji leaderboard with a donut chart breakdown |

All charts use a unified **dark glassmorphism** theme with neon gradient accents.

---

## 🗂️ Project Structure

```
whatsapp_chat_analyzer/
├── app.py               # Streamlit UI & visualisation logic
├── helper.py            # Analytics functions (stats, charts, NLP)
├── preprocessor.py      # Chat parser — raw .txt → structured DataFrame
├── requirements.txt     # Python dependencies
└── stop_hinglish.txt    # Stop-word list (English + Hindi/Hinglish)
```

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/your-username/whatsapp-chat-analyzer.git
cd whatsapp-chat-analyzer
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the app

```bash
streamlit run app.py
```

The app will open at `http://localhost:8501` in your browser.

---

## 📤 Exporting a WhatsApp Chat

1. Open any WhatsApp chat or group
2. Tap ⋮ **Menu → More → Export chat**
3. Choose **Without Media** (recommended)
4. Save the `.txt` file to your device

> ⚠️ The parser expects the **US date format** (`MM/DD/YY, HH:MM AM/PM`) used by WhatsApp on most Android and iOS devices set to English.

---

## 📦 Dependencies

```
streamlit
matplotlib
seaborn
pandas
wordcloud
urlextract
emoji
```

Install all at once:

```bash
pip install streamlit matplotlib seaborn pandas wordcloud urlextract emoji
```

---

## 🖥️ Usage

1. Launch the app and upload your exported `.txt` file in the sidebar
2. Select a specific user **or** choose **Overall** for the full group analysis
3. Hit **⚡ Run Analysis** — all charts render instantly
4. Scroll through the dashboard to explore each section

---

## 🎨 Design

ChatPulse uses a custom dark UI built entirely with Streamlit's `st.markdown` and injected CSS:

- **Fonts** — Syne (headings) · DM Sans (body) · Space Mono (data/mono)
- **Palette** — Deep `#07080d` base with atmospheric purple/teal/pink radial gradients
- **Charts** — Unified dark matplotlib theme with gradient accent bars and glow line plots
- **Cards** — Glassmorphic stat cards with per-card gradient accents and hover effects

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/cool-new-chart`
3. Commit your changes: `git commit -m 'Add cool new chart'`
4. Push to the branch: `git push origin feature/cool-new-chart`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">
  Made with ❤️ and Streamlit
</div>
