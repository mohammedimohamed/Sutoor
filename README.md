# مولد أوراق عمل الخط العربي للأطفال
## Printable Arabic Handwriting Worksheet Generator (A4)

A specialized, interactive, and printable Arabic handwriting worksheet generator designed for early learners (Kindergarten, Preschool, and Early Primary grades). It generates pedagogically sound, print-perfect single-sheet A4 practice pages adhering to standard Arabic Naskh calligraphy guidelines.

---

## 🌟 Key Features

- **Exact A4 Portrait Layout (`210mm x 297mm`)**: Engineered to strictly fit on a single A4 page with zero multi-page spill during printing or PDF export.
- **Pedagogical 4-Line Ruling System**:
  1. **Top Ascender Line (السطر العلوي)**: Dashed sky blue (`#0284c7`) marking maximum height (e.g. أ, ل, ك, ط).
  2. **Waistline / Midline (خط الوسط - الخصر)**: Dotted slate (`#94a3b8`) for letter heads and lowercase bodies (e.g. د, ر, و, loop of م).
  3. **Baseline (سطر الارتكاز الأساسي)**: Solid dark blue (`#1e3a8a`, 2.2px) where letter bodies sit.
  4. **Descender Line (سطر الهبوط - القاع)**: Dashed crimson (`#e11d48`) marking the bottom depth for letters with deep bowls or tails (e.g. ح, ع, ل, ي, ر).
- **All 28 Arabic Letters Supported**: Complete letter presets with custom vector mascot illustrations, phonics words, isolated and positional forms (بداية، وسط، نهاية), and short vowels with full Tashkeel (الحركات القصيرة: الفتحة، الضمة، الكسرة).
- **Standard Tracing Pedagogical Style**:
  - Reference sample in solid high-contrast dark slate (`#1e293b`).
  - Tracing guide in solid educational light-gray (`#cbd5e1` / `#94a3b8`), allowing children to trace smoothly over the letters without visual distortion or character fragmentation.
  - Natural cursive Arabic ligatures with unbroken glyphs and zero artificial letter-spacing.
- **Dynamic Personalization**:
  - Student name input with instant worksheet update.
  - Interactive direct-on-page name editing.
  - Quick student name presets (عائشة، يوسف، فاطمة، أحمد، مريم، عمر).
  - Sentence generator supporting dynamic `{name}` template interpolation.
- **Audio Feedback & Interactive Zoom**:
  - Educational audio chimes on letter and name selection.
  - Viewport zoom controls: **Fit to Screen (ملاءمة للشاشة)**, **100% Actual Print Size**, and **85%**.
- **1-Click Print & PDF Export**: Instant print preview with custom `@media print` rules that hide all browser UI and control toolbars automatically.

---

## 📋 Project Structure

```text
├── index.html          # Core application (standalone HTML5, CSS3, and JavaScript)
├── package.json        # Node.js project manifest & dependencies
├── vite.config.ts      # Vite development and build configuration
├── metadata.json       # Applet metadata and capabilities
├── README.md           # Documentation & instructions (this file)
└── src/
    ├── main.tsx        # Application entry point
    ├── App.tsx         # React root wrapper
    └── index.css       # Tailwind CSS entry point
```

---

## 🚀 How to Run the Project

You can run this project in multiple ways depending on your environment:

### Method 1: Using the Node.js Development Server (Recommended)

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Start the Development Server**:
   ```bash
   npm run dev
   ```
   The application will start on `http://localhost:3000` (or the port specified by your environment).

3. **Build for Production**:
   ```bash
   npm run build
   ```

4. **Preview Production Build**:
   ```bash
   npm run preview
   ```

### Method 2: Standalone Direct File Opening (No Node.js Required)

Because the generator is self-contained in `index.html`, you can also:
1. Double-click `index.html` in your file manager, or
2. Open `index.html` directly in any modern web browser (Google Chrome, Microsoft Edge, Mozilla Firefox, or Apple Safari).

---

## 📖 How to Use the Generator

### 1. Select an Arabic Letter
- Use the **Letter Dropdown (اختر الحرف)** in the top control bar, or
- Click any of the **Quick Alphabet Chips (أ، ب، ت...)** in the scrollable alphabet bar.
- The mascot artwork, vocabulary words, positions, vowels, and practice sentence will automatically update.

### 2. Personalize with the Student's Name
- Type the student's name in the **اسم التلميذ** input in the top bar, or
- Click one of the **Quick Names (عائشة، يوسف، فاطمة...)**, or
- Click directly on the dotted name line on the printed sheet itself and type!

### 3. Customize the Practice Sentence
- Enter a custom sentence in the **جملة التتبع** field.
- If **دمج اسم التلميذ تلقائيًا (Auto-combine name)** is checked, the `{name}` placeholder will automatically be replaced with the active student's name (e.g. `عَائِشَةُ تَرْسُمُ عُصْفُورًا جَمِيلًا`).

### 4. Adjust the Screen View
- Click **ملاءمة (Fit)** to scale the full A4 sheet neatly to your browser viewport.
- Click **100%** to view the worksheet at exact physical printing scale.
- Click **85%** for compact laptop screens.

### 5. Print or Save as PDF
1. Click the blue **طباعة الورقة (A4)** button in the top toolbar (or press `Ctrl + P` / `Cmd + P`).
2. In your browser's print dialog:
   - **Destination**: Choose your physical printer, or select **Save as PDF (حفظ كملف PDF)**.
   - **Paper Size**: Set to **A4**.
   - **Orientation**: Set to **Portrait (عمودي)**.
   - **Margins**: Set to **None** or **Default**.
   - **Options**: Check **Background graphics (رسومات الخلفية)** so guideline colors and badges print vividly.
3. Click **Print** or **Save**.

---

## 📐 Worksheet Layout Structure

1. **Header**: Student Name, Class/Group, Date, and Letter Badge.
2. **Mascot & Phonics Card**: Cute vector illustration, vocabulary word with complete Tashkeel, meaning, and pedagogical stroke direction tips.
3. **Practice Track 1 (Vowels & Positions)**:
   - Short vowels (الفتحة، الضمة، الكسرة) with solid reference, 2 light-gray tracing slots, and 1 independent slot.
   - Letter positions (Isolated منفصل, Initial بداية, Medial وسط, Final نهاية).
   - Freestyle numbered guide points for independent letter repetition.
4. **Practice Track 2 (Words Tracing)**: 4 curated vocabulary words with solid references and light-gray tracing guides sitting on the blue baseline with safe 30px horizontal clearances.
5. **Practice Track 3 (Sentence Tracing & Copying)**:
   - Full-width tracing sentence in clear `#94a3b8` light gray across the 55px writing track.
   - Dedicated freehand line for independent copying with an encouraging star badge (`اُكْتُبْ بِمُفْرَدِك 🌟`).
6. **Footer**: 5-star evaluation rating for teachers/parents, positive motivational badge, and worksheet notes.

---

## 🛠️ Technologies Used

- **HTML5 & CSS3**: Native CSS flexbox and grid layouts, `@page` print rules, and print-color optimization.
- **SVG Engine**: Scalable vector graphics for pixel-perfect continuous 4-line guidelines and mascot illustrations.
- **Google Fonts**:
  - `Amiri`: Standard Naskh calligraphic typeface for correct Arabic cursive ligatures and Tashkeel.
  - `Cairo`: Modern, friendly Arabic typeface for labels, badges, and headers.
- **Web Audio API**: Synthesized chimes for tactile classroom engagement.
- **Vite & TypeScript**: Tooling and build configuration.

---

## 📄 License

This project is licensed under the Apache-2.0 License.
