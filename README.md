# Student Mental Health & Smartphone Use Survey (Excel)

## Objective
After an internal survey of students, the educational institution is concerned about the relationship between smartphones and excessive exposure, and how this affects academic performance and mental health. This project analyses that survey — based on study patterns, usage duration and habits — to:

- Assess impact on **academic performance** and **mental health**
- Flag points of attention to prevent further damage, or improve performance
- Check whether the institution can offer targeted assistance based on the diagnosis

## Dataset
- **Source:** Self-reported student survey ("Impact of Mobile Phone on Students' Health" — see `aboutdataset.txt` for the full field dictionary).
- **Respondents:** ~99 students.
- **Key fields:** age, gender, mobile OS, daily usage hours, performance impact, usage distraction, attention span, physical/mental symptoms (headache, sleep disturbance, anxiety/stress), symptom frequency, health precautions taken, and self-rated overall health.
- Two versions of the dataset are included: the original raw export and a modified/cleaned version used for the analysis.

## Data Cleaning & Preparation
- Cleaned in Excel from the raw export (`_original_dataset_` → `_modified_`).
- **Data quality issue identified and flagged in the report itself:** a handful of respondents selected multiple, contradictory options for the same question — e.g. rating their overall health as "Excellent;Good;Fair;Poor" simultaneously. These inconsistent responses limit how much weight can be placed on the health-rating cross-tabs.
- Cross-tab (pivot-style) tables were built directly in Excel to compare pairs of variables (see Visualisations below).

## Key Visualisations
Around 15 cross-tab charts were built to explore the data, including:
- Students × Gender, Students × Mobile OS, Gender × Mobile OS
- Health Rating × Daily Usage
- Headache × Daily Usage, Sleep Disturbance × Daily Usage, Anxiety/Stress × Daily Usage
- Symptom Frequency × Headache / Sleep Disturbance / Anxiety
- Age × Daily Usage, Age × Attention Span, Age × Health Precautions
- Educational Apps × Daily Usage, Educational Apps × Usage Distraction
- Mobile Phone Activities × Symptom Frequency
- Useful Features (e.g. Internet Access) × Attention Span

## Method
Rather than formal statistical tests, the analysis relies on **descriptive cross-tabulation** (percentages per category via Excel PivotTable-style tables), with findings cross-referenced against external research (medical/health articles, cited directly in the report) to support or challenge each pattern found in the data.

## Results & Limitations
- **Headaches:** students using their phone under 2 hours/day reported almost no headaches, while usage above 2 hours showed a clear increase — consistent with external research on "text neck" and screen-related headaches (cited in the report).
- **Sleep disturbance:** the strongest and most consistent pattern in the dataset — usage is clearly linked to disrupted sleep, aligning with research on blue light suppressing melatonin.
- **Anxiety/stress:** showed **no clear pattern** against usage — interpreted as a symptom likely driven by other life factors, with the phone as only one contributing element.
- **Health risk awareness:** only 58.2% of students are fully aware of the health risks of excessive use; 21.4% only partially aware, 20.4% not aware at all.
- **Age 21–25 anomaly:** this group showed the widest gap in attention-span impact and took the most precautions — but they also make up ~72% of the sample (71 of 99), so the report explicitly flags this as a possible **sample-skew artifact** rather than a genuine age effect.
- **Video-based studiers** study for longer, but are also more distracted and report more symptoms than students using other study methods.
- ⚠️ **Sample limitations:** heavily skewed toward males (81.8%) and the 21–25 age group (~72%), plus the self-contradictory health-rating responses noted above — both limit how confidently these patterns generalise.

## Business Conclusion & Recommendations
- **Run an awareness campaign:** over 40% of students are not fully aware of the health risks of excessive smartphone use.
- **Partner with psychologists/therapists:** since anxiety/stress didn't correlate cleanly with usage, the report recommends the institution address it as a broader mental-health issue rather than a phone-usage one alone.
- **Promote sport/leisure initiatives** (e.g. gym partnerships, group activities) as a way to reduce stress and screen time, which prior studies link to improved academic performance.
- **Improve the survey itself** for future rounds: add fields such as nutrition self-rating, physical activity and hobbies, and prevent contradictory multi-select answers — both would reduce the noise seen in this round's data.

## Files in this repository

| File | Description |
|---|---|
| [`dataset/`](./dataset) | Survey data — original export and cleaned/modified version used for analysis |
| [`Report.odp`](./Report.odp) | Full presentation: EDA charts, findings, external references, and recommendations |
