Rule-Based Synthetic Dataset for MDD Treatment-Response Monitoring

This repository contains a clinically guided, rule-based, multimodal longitudinal synthetic dataset generated for research on treatment-response monitoring in Major Depressive Disorder (MDD).

The dataset was developed to support early-stage experimentation, simulation, and future machine learning and federated learning workflows in privacy-sensitive mental health research.

Overview

Monitoring treatment response in MDD remains challenging because treatment often follows a trial-and-error process, and real-world multimodal mental health data are difficult to access due to privacy, ethical, and availability constraints.

This repository provides a fully synthetic dataset designed to represent clinically plausible treatment-response patterns over a 12-week acute monitoring period. The dataset integrates PHQ-9 clinical assessments with simulated behavioral and physiological indicators derived from smartphones and wearable devices.

Important Disclaimer

This dataset is fully synthetic.

It does not contain real patient records, identifiable personal data, or data collected from actual individuals. The dataset was generated using rule-based assumptions informed by digital phenotyping literature, expert clinical input, and PHQ-9-based treatment-response monitoring logic.

The dataset should not be interpreted as real clinical evidence or used for clinical decision-making.

Repository Structure

mdd-synthetic-treatment-response-dataset/
│
├── data/
│   ├── participants.csv
│   ├── daily_data.csv
│   ├── clinical_assessments.csv
│   ├── weekly_summary.csv
│   └── final_outcomes.csv
│
├── code/
│   ├── synthetic_data_generator.py
│   ├── plausibility_analysis.py
│   └── visualization_code.py
│
├── supplementary_materials/
│   ├── synthetic_data_schema.xlsx
│   └── expert_interview_questionnaire.docx
│
├── outputs/
│   └── figures/
│
├── README.md
├── requirements.txt
└── LICENSE

Dataset Description

The dataset follows a 12-week acute-phase treatment-monitoring structure and includes:

* baseline participant characteristics;
* device-related information;
* daily behavioral and physiological monitoring variables;
* biweekly PHQ-9 clinical assessments;
* weekly summary features;
* treatment review points;
* treatment-response trajectories;
* final response and remission outcomes;
* missingness indicators.

Main Dataset Tables

participants.csv

Contains participant-level baseline information, including demographic characteristics, device-related characteristics, baseline PHQ-9 score, treatment type, initial severity group, and adherence risk profile.

daily_data.csv

Contains daily behavioral and physiological monitoring variables generated from Week 0 to Week 12. These include sleep, activity, mobility, physiology, social interaction, digital behavior, adherence, EMA-related variables, and missingness indicators.

clinical_assessments.csv

Contains PHQ-9 clinical assessment records at scheduled assessment points: Week 0, 2, 4, 6, 8, 10, and 12. It includes clinical scores, change from baseline, percentage change from baseline, response status, remission status, and treatment review decisions where applicable.

weekly_summary.csv

Contains weekly aggregated features calculated at the end of Weeks 1–12. These summaries represent broader behavioral and physiological trends over time.

final_outcomes.csv

Contains final Week 12 treatment-response labels, including final response status, final remission status, trajectory group, time to response, and sustained improvement indicators.

Synthetic Data Schema

The synthetic data schema is provided in the supplementary_materials/ folder.

The schema defines:

* variable domains;
* variable names;
* data types;
* measurement frequencies;
* expected ranges or categories;
* clinical or behavioral meanings;
* rule-based generation assumptions;
* relevance to MDD treatment-response monitoring.

The schema served as the blueprint for the rule-based synthetic data generation process.

Treatment-Response Trajectories

The dataset includes five treatment-response trajectory groups:

* early responders;
* delayed responders;
* partial responders;
* non-responders;
* unstable responders.

These groups were generated to represent different patterns of symptom progression and behavioral change during the 12-week monitoring period.

Clinical Anchor

PHQ-9 was used as the primary clinical anchor for symptom severity and treatment-response monitoring.

PHQ-9 assessments were represented at:

Week 0, Week 2, Week 4, Week 6, Week 8, Week 10, and Week 12

Treatment review points were represented at:

Week 4, Week 8, and Week 12

Variables Included

The dataset includes variables from the following domains:

* clinical anchors;
* sleep and circadian rhythm;
* physical activity;
* mobility and location;
* physiology;
* digital behavior;
* social interaction;
* adherence;
* Ecological Momentary Assessment;
* missingness and data quality.

Examples of variables include:

* PHQ-9 score;
* sleep efficiency;
* wake after sleep onset;
* steps;
* sedentary minutes;
* resting heart rate;
* heart-rate variability;
* time at home;
* location entropy;
* screen time;
* night screen time;
* unique contacts;
* medication adherence;
* therapy adherence;
* GPS missingness;
* heart-rate missingness.

Plausibility Assessment

The generated dataset was assessed for internal plausibility using:

* descriptive statistics;
* distribution checks;
* longitudinal trajectory analysis;
* correlation analysis;
* responder-group comparisons;
* missingness assessment.

The aim of the plausibility assessment was to determine whether the generated dataset preserved clinically interpretable, statistically plausible, and behaviorally coherent patterns for controlled experimentation.

Intended Use

This dataset is intended for:

* early-stage modelling;
* simulation studies;
* treatment-response monitoring research;
* machine learning workflow testing;
* federated learning experimentation;
* privacy-preserving mental health research;
* methodological development using synthetic data.

Not Intended For

This dataset should not be used for:

* clinical diagnosis;
* clinical treatment decisions;
* real-world patient outcome prediction;
* estimating actual population-level MDD treatment effects;
* replacing real-world clinical validation.

Installation

To run the code, first install the required Python packages:

pip install -r requirements.txt

Example Usage

To generate the synthetic dataset:

python code/synthetic_data_generator.py

To run plausibility analysis:

python code/plausibility_analysis.py

To generate figures:

python code/visualization_code.py

Citation

If you use this dataset, code, or schema, please cite the associated manuscript:

[Add citation after publication]

Data Availability

The synthetic dataset, synthetic data schema, and code are made available for research and methodological experimentation. The dataset is fully synthetic and does not contain real patient records or identifiable personal data.

Funding

This research was supported by the DAAD Doctoral Programme.

License

Please see the LICENSE file for details.

Recommended licensing:

* code: MIT License;
* dataset and documentation: Creative Commons Attribution 4.0 International (CC BY 4.0).

Contact

For questions about the dataset or code, please contact:

Elsie Kaaya
elsie.kaaya@uni_oldenburg.de
Here is a ready-to-upload README.md draft for your GitHub repository:

Rule-Based Synthetic Dataset for MDD Treatment-Response Monitoring

This repository contains a clinically guided, rule-based, multimodal longitudinal synthetic dataset generated for research on treatment-response monitoring in Major Depressive Disorder (MDD).

The dataset was developed to support early-stage experimentation, simulation, and future machine learning and federated learning workflows in privacy-sensitive mental health research.

Overview

Monitoring treatment response in MDD remains challenging because treatment often follows a trial-and-error process, and real-world multimodal mental health data are difficult to access due to privacy, ethical, and availability constraints.

This repository provides a fully synthetic dataset designed to represent clinically plausible treatment-response patterns over a 12-week acute monitoring period. The dataset integrates PHQ-9 clinical assessments with simulated behavioral and physiological indicators derived from smartphones and wearable devices.

Important Disclaimer

This dataset is fully synthetic.

It does not contain real patient records, identifiable personal data, or data collected from actual individuals. The dataset was generated using rule-based assumptions informed by digital phenotyping literature, expert clinical input, and PHQ-9-based treatment-response monitoring logic.

The dataset should not be interpreted as real clinical evidence or used for clinical decision-making.

Repository Structure

mdd-synthetic-treatment-response-dataset/
│
├── data/
│   ├── participants.csv
│   ├── daily_data.csv
│   ├── clinical_assessments.csv
│   ├── weekly_summary.csv
│   └── final_outcomes.csv
│
├── code/
│   ├── synthetic_data_generator.py
│   ├── plausibility_analysis.py
│   └── visualization_code.py
│
├── supplementary_materials/
│   ├── synthetic_data_schema.xlsx
│   └── expert_interview_questionnaire.docx
│
├── outputs/
│   └── figures/


Dataset Description

The dataset follows a 12-week acute-phase treatment-monitoring structure and includes:

* baseline participant characteristics;
* device-related information;
* daily behavioral and physiological monitoring variables;
* biweekly PHQ-9 clinical assessments;
* weekly summary features;
* treatment review points;
* treatment-response trajectories;
* final response and remission outcomes;
* missingness indicators.

Main Dataset Tables

participants.csv

Contains participant-level baseline information, including demographic characteristics, device-related characteristics, baseline PHQ-9 score, treatment type, initial severity group, and adherence risk profile.

daily_data.csv

Contains daily behavioral and physiological monitoring variables generated from Week 0 to Week 12. These include sleep, activity, mobility, physiology, social interaction, digital behavior, adherence, EMA-related variables, and missingness indicators.

clinical_assessments.csv

Contains PHQ-9 clinical assessment records at scheduled assessment points: Week 0, 2, 4, 6, 8, 10, and 12. It includes clinical scores, change from baseline, percentage change from baseline, response status, remission status, and treatment review decisions where applicable.

weekly_summary.csv

Contains weekly aggregated features calculated at the end of Weeks 1–12. These summaries represent broader behavioral and physiological trends over time.

final_outcomes.csv

Contains final Week 12 treatment-response labels, including final response status, final remission status, trajectory group, time to response, and sustained improvement indicators.

Synthetic Data Schema

The synthetic data schema is provided in the supplementary_materials/ folder.

The schema defines:

* variable domains;
* variable names;
* data types;
* measurement frequencies;
* expected ranges or categories;
* clinical or behavioral meanings;
* rule-based generation assumptions;
* relevance to MDD treatment-response monitoring.

The schema served as the blueprint for the rule-based synthetic data generation process.

Treatment-Response Trajectories

The dataset includes five treatment-response trajectory groups:

* early responders;
* delayed responders;
* partial responders;
* non-responders;
* unstable responders.

These groups were generated to represent different patterns of symptom progression and behavioral change during the 12-week monitoring period.

Clinical Anchor

PHQ-9 was used as the primary clinical anchor for symptom severity and treatment-response monitoring.

PHQ-9 assessments were represented at:

Week 0, Week 2, Week 4, Week 6, Week 8, Week 10, and Week 12

Treatment review points were represented at:

Week 4, Week 8, and Week 12

Variables Included

The dataset includes variables from the following domains:

* clinical anchors;
* sleep and circadian rhythm;
* physical activity;
* mobility and location;
* physiology;
* digital behavior;
* social interaction;
* adherence;
* Ecological Momentary Assessment;
* missingness and data quality.

Examples of variables include:

* PHQ-9 score;
* sleep efficiency;
* wake after sleep onset;
* steps;
* sedentary minutes;
* resting heart rate;
* heart-rate variability;
* time at home;
* location entropy;
* screen time;
* night screen time;
* unique contacts;
* medication adherence;
* therapy adherence;
* GPS missingness;
* heart-rate missingness.

Plausibility Assessment

The generated dataset was assessed for internal plausibility using:

* descriptive statistics;
* distribution checks;
* longitudinal trajectory analysis;
* correlation analysis;
* responder-group comparisons;
* missingness assessment.

The aim of the plausibility assessment was to determine whether the generated dataset preserved clinically interpretable, statistically plausible, and behaviorally coherent patterns for controlled experimentation.

Intended Use

This dataset is intended for:

* early-stage modelling;
* simulation studies;
* treatment-response monitoring research;
* machine learning workflow testing;
* federated learning experimentation;
* privacy-preserving mental health research;
* methodological development using synthetic data.

Not Intended For

This dataset should not be used for:

* clinical diagnosis;
* clinical treatment decisions;
* real-world patient outcome prediction;
* estimating actual population-level MDD treatment effects;
* replacing real-world clinical validation.

Installation

To run the code, first install the required Python packages:

pip install -r requirements.txt

Example Usage

To generate the synthetic dataset:

python code/synthetic_data_generator.py

To run plausibility analysis:

python code/plausibility_analysis.py

To generate figures:

python code/visualization_code.py

Citation

If you use this dataset, code, or schema, please cite the associated manuscript:

[Add citation after publication]

Data Availability

The synthetic dataset, synthetic data schema, and code are made available for research and methodological experimentation. The dataset is fully synthetic and does not contain real patient records or identifiable personal data.

Funding

This research was supported by the DAAD Doctoral Programme.


Contact

For questions about the dataset or code, please contact:

Elsie Kaaya
elsie.kaaya@uni-oldenburg.de
Carl von Ossietzky Universität Oldenburg 
