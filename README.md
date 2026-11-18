<div align="center">

# ✦ NoteForge
### Your topics. Your pages. Your personal study notebook.

**Turn a simple CSV file into a clean, printable A4 notebook — one topic at a time.**

<br>

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Handling-150458?style=for-the-badge&logo=pandas&logoColor=white)
![PDF](https://img.shields.io/badge/Output-PDF-EA4335?style=for-the-badge&logo=adobeacrobatreader&logoColor=white)

</div>

---

## ✨ The idea

A good study session deserves a good place for your notes.

**NoteForge** takes the topics in `topics.csv` and transforms them into a structured, ruled PDF notebook. Each topic gets its own section, with as many pages as you choose. The result is a simple A4 notebook you can print, write in, and organize around the subjects you're learning.

No manual page formatting. Just update your topic list and generate your notebook.

## 🖋️ What it creates

- **A dedicated section for every topic** — each section starts with a clear topic heading.
- **Your chosen page count** — decide how many pages each topic needs in the CSV file.
- **A4 ruled pages** — evenly spaced horizontal lines give you room for handwritten notes.
- **Topic labels on every page** — the footer helps keep printed pages organized.
- **Easy to customize** — edit the CSV to make a notebook for a new course or learning plan.

## 📁 Project structure

```text
NoteForge/
├── main.py       # Builds the PDF notebook
├── topics.csv    # Topics and page counts
└── output.pdf    # Generated notebook
```

## 🚀 Get started

### 1. Clone the project

```bash
git clone <YOUR-REPOSITORY-URL>
cd NoteForge
```

### 2. Install the dependencies

```bash
pip install pandas fpdf2
```

### 3. Generate your notebook

Keep `main.py` and `topics.csv` in the same folder, then run:

```bash
python main.py
```

Your notebook will be created as **`output.pdf`** in the project folder.

## 🧩 Make it yours

Open `topics.csv` and edit the topics and page counts.

| Column | Purpose |
|---|---|
| `Order` | Keeps track of the topic sequence in the file |
| `Topic` | The heading used for that section |
| `Pages` | Number of pages generated for that topic |

Example:

```csv
Order,Topic,Pages
1,Python Basics,3
2,Data Structures,5
3,Object-Oriented Programming,4
```

The script follows the rows in their existing CSV order. The `Order` value is for your reference; the current script does not sort the rows by this column.

## 🛠️ Built with

- **Python** — project logic
- **Pandas** — reads the topic list from CSV
- **FPDF2** — creates and formats the PDF

## 🌱 Ideas for future versions

- Add page numbers.
- Offer different page styles, such as blank, dotted, or grid paper.
- Let users customize line spacing and page margins.
- Add a simple interface for creating notebooks without editing the CSV.

---

<div align="center">

**Made with Python, for more organized learning.** ✦

</div>
