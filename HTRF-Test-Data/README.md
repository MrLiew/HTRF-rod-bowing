# HTRF-rod-bowing
## HTRF database and subchannel analysis results with code COBRA-TF(CTF)

Original tests data from the report NP-2609-V3P1.pdf Parametric Study of CHF Data Vol.3 Part1: Critical Heat Flux Data
URL: [http://www.epri.com/#/pages/product/NP-2609-V3P1/?lang=en](http://www.epri.com/#/pages/product/NP-2609-V3P1/?lang=en)


###### HTRF tests description:
- HTRF 166 (no rod bowing), the reference test with a nominal configuration of rods, 47 tests;
- HTRF 167 (bowing to contact), rod 10 is bowed towards thimble tube 7 to contact rods 6 and 11, 35 tests;
- HTRF 168 (bowing to contact), heated rod 11 is bowed towards rod 6 to contact rods 7 and 10, 65 tests;
- HTRF 169 (partly rod bowing, no contact), heated rod 11 is bowed towards rod 6, reducing gap between rod 10 and thimble tube 7 to 15\% of the nominal gap, 48 tests;
- HTRF 170 (partly rod bowing, no contact), heated rod 11 bowed towards rod 6, reducing gap between rod 10 and thimble tube 7 to 50\% of nominal gap, 48 tests;

###### Thermal hydraulic parameters used in the files:
- Pressure: Test section outlet pressure in psia
- Inlet temperature: coolant temperature at the inlet to the test section in F
- Mass velocity: average mass velocity of coolant entering the test section in Million lbs/hr-ft2
- Heat flux: average heat flux to the test section at CHF in Million Btu/hr-ft2
- CHF rods: order of occurance of CHF; digits to the left of the decimal point designate the rod number, and digits to the right of the decimal point designate the axial location of circumferential location of the thermocouple detecting CHF.

###### in US units:
	- HTRF_Test_166.dat
	- HTRF_Test_167.dat
	- HTRF_Test_168.dat
	- HTRF_Test_169.dat
	- HTRF_Test_170.dat
###### in SI units:
	- HTRF_166_SI_units.dat
	- HTRF_167_SI_units.dat
	- HTRF_168_SI_units.dat
	- HTRF_169_SI_units.dat
	- HTRF_170_SI_units.dat
	- HTRF_database_SI_units.dat
