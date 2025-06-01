# 🎨 Colour Detective Tool

## 👁️ Helping the Colorblind, Creatives, and Curious Minds

This project is designed to **detect the name of a color** from any point in an image — just by double-clicking! It's especially helpful for people with **color vision deficiency**, UI/UX designers, and anyone who finds it tricky to distinguish between similar shades.

---

## 🧠 What Does It Do?

* You load an image.
* You **double-click** anywhere on it.
* It instantly shows the **closest color name** along with its RGB (Red, Green, Blue) values.
* It's that simple — and pretty fun too!

---

## 🖥️ How to Run It

### ✅ Prerequisites:

Make sure you have:

* Python 3 installed
* `pip` installed (Python’s package manager)

---

### 📥 Step-by-step Setup:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Arjundixit18/Color-Detective-Tool.git
   cd Colour-Detection
   ```

2. **Install dependencies:**

   ```bash
   pip install opencv-python pandas
   ```

   *(Tested with opencv-python 4.1.1.26 and pandas 0.24.2)*

3. **Add your image** to the same folder as `colour.py`.

4. **Run the project:**

   ```bash
   python3 colour.py
   ```

---

## 📸 How to Use

1. When prompted, **enter the image file name** (e.g., `sample.jpg`).
2. The image will open in a new window.
3. **Double-click** anywhere on the image — the app will display:

   * The name of the color
   * Its RGB values
4. Press **ESC** to exit.

---

## 📝 Example

Let's say you double-click on a dark blue sky in a photo.
It might show:
`Navy Blue  R=0 G=0 B=128`

---

## 🗂️ Notes

* The image file **must be in the same directory** as the Python file.
* Color names are matched using a **CSV file of color names and RGB values**.
* Works entirely offline after setup.

---

## 💡 Behind the Scenes

* Uses **OpenCV** to display the image and capture mouse events.
* Uses **Pandas** to read the color list from `colors.csv`.
* Calculates the closest color using simple RGB distance formula:

  ```python
  distance = |R1 - R2| + |G1 - G2| + |B1 - B2|
  ```

---

## 🙌 Who Can Use This?

* People with **color blindness**
* **Web/UI Designers** and **Artists**
* **Students** learning image processing
* Anyone curious about color codes

---

## 📫 Feedback / Contributions

Feel free to fork, star ⭐ the repo, or open a pull request.
Feedback and improvements are always welcome!

---

## ✨ Acknowledgment

Built to make color recognition easier for everyone — because color should be accessible to all.

---
