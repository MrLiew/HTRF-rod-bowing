# Subchannel modeling of single rod bowing in a bundle geometry

Here we collect all COBRA-TF(CTF) input decks to reproduce results published in NED paper: R. Mukin, R. Puragliesi, M. Pecchia and M. Seidl. "Subchannel modeling of single rod bowing in a bundle geometry" _Nuclear Engineering and Design_ **XXX** (2018): PPP-PPP.

COBRA-TF (CTF) is a subchannel thermal-hydraulic code used in this work. It is a two-fluid, three-field thermal-hydraulic code maintained by research groups in Oak Ridge National Laboratory and North Carolina State University.

In this study, an assessment of subchannel code CTF v3.5 in addressing the effect of rod bowing on the departure from the nucleate boiling ratio (DNBR) is performed. Two well-known approaches for the critical heat flux (CHF) prediction are used: the W3 correlation and Groeneveld look-up table. Four different rod bowing geometries in a 4x4 rod bundle from the [HTRF CHF data bank](http://www.epri.com/#/pages/product/NP-2609-V3P1/?lang=en) are modelled: rod bowing with a gap closure of 50% and 85% of the nominal gap, and two configurations of rod bowing to contact. Comparison of calculated critical power resulted in an agreement of 10\% with measured values for the straight rod bundle and partial rod bowing configurations. Results for the rod bowing to contact tests are less in agreement with the experimental values.


- HTRF tests: HTRF-Test-Data

- Submitted paper: Paper-NED2018

- All input decks for each test are in the following folders:
	- HTRF-Test-166
	- HTRF-Test-167
	- HTRF-Test-168
	- HTRF-Test-169
	- HTRF-Test-170



1. Folders structure:
```
		HTRF-Test-[Name]
		|-- HTRF-Test-[Name]-beta_[beta]
		    |-- HTRF-[Name]-[ID]
			`-- HTRF-[Name]-[ID]-IRFC-[Fric]
			    |-- HTRF-[Name]-[ID]-[CHF]-broyden1-[Power]
```

where:

- [Name]: HTRF test names are: 166, 167, 168, 169 and 170;	
- [beta]: beta is a mixing coefficient, for which sensetivity is performed in the test HTRF 166;
- [ID]: test ID in each of the test name;
- [Fric]: rod friction model 5 is applied in all tests;
- [CHF]: Critical heat flux (CHF) model used in this work: W3, Groeneveld LUT, Bowring, Doroschuk LUT;
- [Power]: power at which DNBR = 1.

2. Each HTRF test folder contain the CTF input deck template: **HTRF-Test-[Name]-CTF_deck_template.inp**

	 e.g. CTF input deck template for test HTRF 166 HTRF-Test-166-CTF_deck_template.inp_

3. **HTRF-Test-[Name]\log_files** :Log files for searching tube bundle power at which DNBR = 1

4. Results for each test are in the CSV files in the corresponding folder: **HTRF-[Test Name]-DNB-Power-[CHF model]-beta_[beta].csv**
