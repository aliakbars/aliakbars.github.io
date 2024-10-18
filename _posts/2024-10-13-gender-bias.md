---
title: "Gender Bias in Intensive Care"
date: 2024-10-13
permalink: /posts/2024/10/missing-values
toc: true
tags:
  - gender-bias
  - intensive-care
  - healthcare
---

Intensive care provides specialised treatment and close monitoring for patients with serious illnesses, injuries, or life-threatening conditions. Clinicians may withdraw or withhold treatments when intensive care is not deemed beneficial for the patient. Additionally, intensive care is often expensive, and demand frequently exceeds available resources ([Todorov et al., 2021](https://doi.org/10.1007/s00134-021-06393-3)). While factors such as older age or high illness severity scores may justify withdrawing or withholding intensive care, Block et al. ([2019](https://doi.org/10.1111/aas.13411)) found that even after adjusting for these variables, females are more likely to have their intensive care withdrawn.

This pattern is evident in several studies across various aspects of intensive care. A recent study involving over 500,000 participants revealed that women were less likely than men to receive mechanical ventilation or renal replacement therapy and had shorter ICU stays ([Modra et al., 2022](https://doi.org/10.1097/CCM.0000000000005469)). Similarly, Todorov et al. ([2021](https://doi.org/10.1007/s00134-021-06393-3)), in a study of comparable size, also observed that female cardiovascular patients were less likely to receive intensive care than men despite being more severely ill. Pietropaoli et al. ([2010](https://doi.org/10.1016/j.genm.2010.09.005)) noted differences in ICU admission rates for severe sepsis or septic shock between genders, though they concluded that the higher in-hospital mortality risk for women was not associated with differences in care delivery. Finally, using MIMIC and eICU, two publicly available intensive care datasets, Liu et al. ([2022](https://doi.org/10.1101/2022.08.01.22277736)) discovered that women are subject to inequality, such as treatment delays, lower rates of ventilation, and a higher likelihood of choosing limited care.

Unfortunately, most of the studies mentioned above did not identify the potential sources of bias, as establishing causal relationships requires comprehensive analysis, often involving counterfactuals that are difficult or sometimes impossible to obtain in clinical settings. However, as Pietropaoli et al. ([2010](https://doi.org/10.1016/j.genm.2010.09.005)) also summarised, gender bias in code status on ICU admission may arise from two potential sources: women (or their surrogates) tending to prefer less aggressive treatments (as shown by Bookwala et al. ([2021](https://doi.org/10.1080/07481180126202)) and Wenger ([1995](https://doi.org/10.1001/archinte.1995.00430190042006))), or healthcare providers influencing end-of-life decisions while misunderstanding patients' actual preferences (as shown by Cook ([1995](https://doi.org/10.1001/jama.1995.03520330033033))).

As plausible steps to prevent gender bias, Todorov et al. ([2021](https://doi.org/10.1007/s00134-021-06393-3)) suggested that intensivists and emergency physicians reassess triage decisions to ensure critically ill (young) women receive necessary care, addressing potential gender biases in protocols. Research into gender-specific factors could also lead to targeted therapies ([Pietropaoli et al., 2010](https://doi.org/10.1016/j.genm.2010.09.005)). Additionally, this effort should not be separated from educational initiatives to identify and address gender biases.

# Bibliography

Block, L. et al. (2019) ‘Age, SAPS 3 and female sex are associated with decisions to withdraw or withhold intensive care’, Acta Anaesthesiologica Scandinavica, 63(9), pp. 1210–1215. Available at: https://doi.org/10.1111/aas.13411.

Bookwala, Kristen M. Coppola, Angel, J. (2001) ‘GENDER DIFFERENCES IN OLDER ADULTS’ PREFERENCES FOR LIFE-SUSTAINING MEDICAL TREATMENTS AND END-OF-LIFE VALUES’, Death Studies, 25(2), pp. 127–149. Available at: https://doi.org/10.1080/07481180126202.

Cook, D.J. (1995) ‘Determinants in Canadian Health Care Workers of the Decision to Withdraw Life Support From the Critically Ill’, JAMA: The Journal of the American Medical Association, 273(9), p. 703. Available at: https://doi.org/10.1001/jama.1995.03520330033033.

Liu, X. et al. (2022) ‘Evaluating Prognostic Bias of Critical Illness Severity Scores Based on Age, Gender, and Primary Language in the USA: A Retrospective Multicenter Study’. Available at: https://doi.org/10.1101/2022.08.01.22277736.

Modra, L.J. et al. (2022) ‘Sex Differences in Treatment of Adult Intensive Care Patients: A Systematic Review and Meta-Analysis’, Critical Care Medicine, 50(6), pp. 913–923. Available at: https://doi.org/10.1097/CCM.0000000000005469.

Todorov, A. et al. (2021) ‘Gender differences in the provision of intensive care: a Bayesian approach’, Intensive Care Medicine, 47(5), pp. 577–587. Available at: https://doi.org/10.1007/s00134-021-06393-3.

Pietropaoli, A.P. et al. (2010) ‘Gender differences in mortality in patients with severe sepsis or septic shock’, Gender Medicine, 7(5), pp. 422–437. Available at: https://doi.org/10.1016/j.genm.2010.09.005.

Wenger, N.S. (1995) ‘Epidemiology of Do-Not-Resuscitate Orders: Disparity by Age, Diagnosis, Gender, Race, and Functional Impairment’, Archives of Internal Medicine, 155(19), p. 2056. Available at: https://doi.org/10.1001/archinte.1995.00430190042006.

```bibtex
@article{septiandri2024bias,
  title   = {Gender Bias in Intensive Care},
  author  = {Septiandri, Ali Akbar},
  year    = 2024,
  month   = {October},
  url     = {https://aliakbars.id/posts/2024/10/gender-bias}
}
```