# Australia Wildfire Analysis & Dashboard  
# تحليل حرائق أستراليا ولوحة متابعة التفاعلية

---

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white)
![Dash](https://img.shields.io/badge/Dash-Plotly-blueviolet)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 🇬🇧 English & 🇸🇦 Arabic Version

### 📄 Project Overview / نظرة عامة عن المشروع
This repository contains a complete analysis of wildfire activities in Australia, from historical data exploration to an interactive dashboard. The goal is to help understand wildfire patterns, distributions, and seasonal behavior across different Australian regions.  
يحتوي هذا المستودع على تحليل كامل لأنشطة حرائق الغابات في أستراليا، بدءًا من استكشاف البيانات التاريخية وصولًا إلى لوحة متابعة تفاعلية. الهدف هو فهم أنماط الحرائق، توزيعها، وسلوكها الموسمي عبر المناطق المختلفة في أستراليا.

### 📂 Dataset / مجموعة البيانات
The dataset: `Historical_Wildfires.csv`  
Key columns / الأعمدة الرئيسية:  
- `Date` — Fire date / تاريخ وقوع الحريق  
- `Region` — Name of the region / اسم المنطقة  
- `Estimated_fire_area` — Estimated area of fire (km²) / المساحة المقدرة للحريق (كم²)  
- `Count` — Number of fire-pixel detections / عدد بكسلات الحرائق المكتشفة  
- Additional metrics like fire brightness and radiative power (if available) / مقاييس إضافية مثل شدة الحريق والقوة الإشعاعية (إن وجدت)  

### 📊 Data Visualizations / الرسوم البيانية
Python libraries used: pandas, matplotlib, seaborn, plotly.  
المكتبات المستخدمة: pandas, matplotlib, seaborn, plotly.

Visualizations include / تشمل الرسوم:  

1. **Line Chart – Fire Area Over Time / مخطط خطي – تغير مساحة الحرائق مع الوقت**  
   ![Line Chart](https://github.com/Raghad-ALmarshadi/Australia-Wildfire-Analysis-Dashboard/blob/main/ScreenShot/Line%20chart.png?raw=true)  

2. **Bar Chart – Estimated Fire Area by Month / مخطط شريطي – مجموع المساحات الشهرية للحريق**  
   ![Bar Chart](https://github.com/Raghad-ALmarshadi/Australia-Wildfire-Analysis-Dashboard/blob/main/ScreenShot/Estimated%20fire%20area%20over%20month.png?raw=true)  

3. **Bar Chart – Mean Estimated Fire Brightness per Region / مخطط شريطي – مقارنة شدة الحرائق بين المناطق**  
   ![Brightness Bar Chart](https://github.com/Raghad-ALmarshadi/Australia-Wildfire-Analysis-Dashboard/blob/main/ScreenShot/Pie%20chart%20%E2%80%93%20portion%20of%20count%20of%20pixels.png?raw=true)  

4. **Pie Chart – Portion of Pixels for Vegetation Fires by Region / مخطط دائري – توزيع عدد البكسلات حسب المنطقة**  
   ![Pie Chart](https://github.com/Raghad-ALmarshadi/Australia-Wildfire-Analysis-Dashboard/blob/main/ScreenShot/Histogram%20of%20mean%20fire%20brightness.png?raw=true)  

5. **Histogram – Distribution of Fire Brightness / مخطط التوزيع – توزيع شدة الحرائق**  
   ![Brightness Histogram](https://github.com/Raghad-ALmarshadi/Australia-Wildfire-Analysis-Dashboard/blob/main/ScreenShot/Distribution%20per%20region%20using%20Seaborn.png?raw=true)  

6. **Scatter Plot – Radiative Power vs Confidence / مخطط تشتت – القوة الإشعاعية مقابل الثقة**  
   ![Scatter Plot](https://github.com/Raghad-ALmarshadi/Australia-Wildfire-Analysis-Dashboard/blob/main/ScreenShot/Scatter%20plot%20%E2%80%93%20Radiative%20power%20vs%20confidence.png?raw=true)  

7. **Map – Approximate Fire Locations / خريطة – المواقع التقريبية للحرائق**  
   ![Map](https://github.com/Raghad-ALmarshadi/Australia-Wildfire-Analysis-Dashboard/blob/main/ScreenShot/Map%20%E2%80%93%20Mark%20all%20regions%20using%20Folium.png?raw=true)  

### 🖥️ Interactive Dashboard / لوحة متابعة تفاعلية
Built with **Dash & Plotly / تم تطويرها باستخدام Dash & Plotly**  
Features / الميزات:  
- Dropdowns for **Region** and **Year** selection / قوائم منسدلة لاختيار المنطقة والسنة  
- Dynamic **Pie Chart**: monthly fire area based on selection / مخطط دائري ديناميكي: المساحة الشهرية للحريق  
- Dynamic **Bar Chart**: monthly pixel count based on selection / مخطط شريطي ديناميكي: عدد البكسلات الشهري  
- Real-time updates on selection changes / تحديثات فورية عند تغيير الاختيار  

### 🚀 How to Run Locally / طريقة التشغيل محليًا
1. Install dependencies / تثبيت المكتبات المطلوبة:  
```bash
pip install pandas plotly dash seaborn matplotlib folium jupyter-dash
```
2. Run the dashboard script / تشغيل ملف لوحة المتابعة:
```bash
python dashboard.py
```
3.Open the browser at / فتح المتصفح على الرابط:
```bash
http://127.0.0.1:8050/
```
4.Interact with the dashboard / التفاعل مع لوحة المتابعة:

- Use the Region dropdown to select a region / استخدمي قائمة المنسدلة لاختيار المنطقة

- Use the Year dropdown to select a year / استخدمي قائمة المنسدلة لاختيار السنة

- Charts will update automatically based on your selection / ستتحدث المخططات تلقائيًا حسب اختياراتك


📝 Project Structure
graphql
Copy code
├── data/                  # CSV dataset from Kaggle


├── visuals/               # Exported static charts


├── app.py                 # Dash interactive dashboard


├── analysis.ipynb         # Jupyter Notebook with analysis


└── README.md              # Project documentation


📈 License
Open-source for educational purposes / مفتوح المصدر لأغراض تعليمية

✨ Author / المؤلف: Raghad Almarshadi


✨ GitHub: https://github.com/Raghad-ALmarshadi


✨ LinkedIn: https://www.linkedin.com/in/raghad-almarshadi-99b5bb25b/

