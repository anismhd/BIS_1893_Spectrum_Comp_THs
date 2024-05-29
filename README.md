Study on Efficacy of Single Set Spectrum Compatible Time History for Linear Seismic Analysis of Structures
Anis M.V., Bharti Banshiwal, A.D. Roshan
Objective
The latest draft version of BIS 1893, Sect 7.6.2 (b), specifies that at-least three sets of ground motions shall be used in linear response history analysis. AERB had commented on the earlier specification of minimum seven time history requirement and opined that for Linear response history analysis, which are often used in generation of input of sub-system design (seismic anchor movement, floor response spectra) single time history or single set of time history is sufficient. An example problem demonstrating efficacy of single spectrum compatible time history in one direction linear analysis was demonstrated using 30 recorded ground motion and single spectrum compatible time history analysis (x-direction). The results were also presented to committee. However, there was an apprehension that, multiple time history requirement is more prudent in the case of simultaneous analysis of lateral directions (X and Y) and the above exercise may not capture this phenomena.
The objective of the study to address the above query on efficacy of single set of spectrum compatible history in adequately capturing response of structure while earthquake has occurred in both x and y direction simultaneously.
Methodology
The series of steps followed in this exercise are briefly described below;
1.	A thirty one set of recorded ground motions are downloaded from PEER Ground motion database.
2.	These ground motion are processed and vertical direction ground motions are removed. The complete list ground motion selected for the study are provided in Table 01.
3.	The complete visualization of these recorded ground motion and its spatial correlations are shown in Annexure 01 and 02.
4.	The response spectra of above 31 set time histories are extracted using PyRotd library. The average response spectra of 31 time history also calculated.
5.	A set of spectrum compatible time history (for x-direction average and y direction average) is generated using EARTHQUAKE module of ACS SASSI software. A plot of 31 recorded ground motion, average ground motion and spectrum compatible ground motion is shown below for comparison. 
 
 
6.	A stick model of containment and internal structure which is often used in AERB’s pilot/demonstration studies is adopted for linear time history analysis (The structure is assumed to be fixed at bottom. A damping of 0.05 is considered throughout the structure.). A figure of the model is shown below (left- un-deformed, right deformed shape at one of the time instant);
 
7.	The modal characteristics of the structure is extracted. Complete modal characteristics is given Table 02. A graph of the same is shown below;
 
8.	A linear modal time history analysis of above structure is conducted for 31 recorded time histories obtained from PEER database and one set of spectrum compatible time history.
9.	The average of peak base shear in both X direction and Y direction for time history analysis using 31 ground motion are extracted.
10.	Above average is peak base shear is compared with peak bese shear obtained from single set spectrum compatible time history analysis. A comparison plots is give below;
11.	[Comparison of FRS] – Will be submitted

Conclusion
Based on the above study one can infer that single set of spectrum compatible time history is sufficient for linear seismic analysis. This aspect can also be theoretically proven using classical random vibration theory and peak factor formula. 
It is to be noted that spectrum compatible time history shall have strict compliance with codal requirements (criteria on PSa ratio as well as PSD).

Please note that the complete computer codes used in this exercise can be downloaded from HERE for verification.
 
Table 1 List of Ground Motions Considered for the Present Study
PEER EQ ID	Name	Station	Date	PGAx (g)	PGAy (g)
RSN1083	Northridge-01	Sunland - Mt Gleason Ave	1/17/1994	0.133	0.157
RSN1614	Duzce Turkey	Lamont 1061	11-12-1999	0.114	0.101
RSN1616	Duzce Turkey	Lamont 362	11-12-1999	0.025	0.044
RSN1633	Manjil Iran	Abbar	6/20/1990	0.515	0.462
RSN164	Imperial Valley-06	Cerro Prieto	10/15/1979	0.160	0.148
RSN286	Irpinia Italy-01	Bisaccia	11/23/1980	0.065	0.049
RSN289	Irpinia Italy-01	Calitri	11/23/1980	0.126	0.136
RSN290	Irpinia Italy-01	Mercato San Severino	11/23/1980	0.108	0.140
RSN313	Corinth Greece	Corinth	2/24/1981	0.237	0.296
RSN3750	Cape Mendocino	Loleta Fire Station	4/25/1992	0.205	0.222
RSN3753	Landers	Fun Valley	6/28/1992	0.146	0.206
RSN3757	Landers	North Palm Springs Fire Sta #36	6/28/1992	0.105	0.139
RSN3759	Landers	Whitewater Trout Farm	6/28/1992	0.123	0.124
RSN3907	Tottori Japan	OKY004	10-06-2000	0.825	0.539
RSN3926	Tottori Japan	OKYH08	10-06-2000	0.241	0.228
RSN3927	Tottori Japan	OKYH09	10-06-2000	0.290	0.163
RSN3932	Tottori Japan	OKYH14	10-06-2000	0.453	0.264
RSN3948	Tottori Japan	SMNH02	10-06-2000	0.282	0.576
RSN4013	San Simeon CA	San Antonio Dam - Toe	12/22/2003	0.093	0.103
RSN4841	Chuetsu-oki	Joetsu Yasuzukaku Yasuzuka	7/16/2007	0.223	0.154
RSN4843	Chuetsu-oki	Matsushiro Tokamachi	7/16/2007	0.193	0.185
RSN57	San Fernando	Castaic - Old Ridge Route	02-09-1971	0.320	0.275
RSN70	San Fernando	Lake Hughes #1	02-09-1971	0.151	0.094
RSN740	Loma Prieta	Anderson Dam (L Abut)	10/18/1989	0.064	0.061
RSN755	Loma Prieta	Coyote Lake Dam - Southwest Abutment	10/18/1989	0.132	0.280
RSN78	San Fernando	Palmdale Fire Station	02-09-1971	0.103	0.098
RSN827	Cape Mendocino	Fortuna - Fortuna Blvd	4/25/1992	0.106	0.114
RSN830	Cape Mendocino	Shelter Cove Airport	4/25/1992	0.229	0.184
RSN864	Landers	Joshua Tree	6/28/1992	0.274	0.284
RSN881	Landers	Morongo Valley Fire Station	6/28/1992	0.223	0.164
RSN88	San Fernando	Santa Felita Dam (Outlet)	02-09-1971	0.155	0.155

 
Table 2 Modal Characteristics of RB Stick Model
		Modal Mass	Cum. Modal Mass
Mode NO	Freq (Hz)	X-Dir	Y-Dir	Z-Dir	X-Dir	Y-Dir	Z-Dir
1	1.68	16904.00	112611.00	0.00	16904.00	112611.00	0.00
2	1.68	112611.00	16904.00	0.00	129515.00	129515.00	0.00
3	3.65	4782.70	16772.00	0.00	134297.70	146287.00	0.00
4	3.65	16772.00	4782.70	0.00	151069.70	151069.70	0.00
5	4.99	0.00	0.00	144208.00	151069.70	151069.70	144208.00
6	5.20	23454.00	4310.90	0.00	174523.70	155380.60	144208.00
7	5.20	4310.90	23454.00	0.00	178834.60	178834.60	144208.00
8	5.50	45959.00	18231.00	0.00	224793.60	197065.60	144208.00
9	5.50	18231.00	45959.00	0.00	243024.60	243024.60	144208.00
10	9.34	1240.20	5644.90	0.00	244264.80	248669.50	144208.00
11	9.34	5644.90	1240.20	0.00	249909.70	249909.70	144208.00
12	12.55	0.00	0.00	92101.00	249909.70	249909.70	236309.00
13	13.36	2100.10	888.09	0.00	252009.80	250797.79	236309.00
14	13.36	888.09	2100.10	0.00	252897.89	252897.89	236309.00
15	14.05	0.00	0.00	14724.00	252897.89	252897.89	251033.00
16	14.83	22039.00	1713.80	0.00	274936.89	254611.69	251033.00
17	14.83	1713.80	22039.00	0.00	276650.69	276650.69	251033.00
18	17.16	789.22	331.31	0.00	277439.91	276982.00	251033.00
19	17.16	331.31	789.22	0.00	277771.22	277771.22	251033.00
20	19.79	0.64	414.18	0.00	277771.86	278185.40	251033.00
21	19.79	414.18	0.64	0.00	278186.04	278186.04	251033.00
22	20.51	0.00	0.00	6203.50	278186.04	278186.04	257236.50
23	22.02	0.00	0.00	5645.90	278186.04	278186.04	262882.40
24	22.29	139.40	131.77	0.00	278325.44	278317.81	262882.40
25	22.29	131.77	139.40	0.00	278457.21	278457.21	262882.40
26	24.47	439.78	28.39	0.00	278896.99	278485.60	262882.40
27	24.47	28.39	439.78	0.00	278925.38	278925.38	262882.40
28	24.93	88.15	9.22	0.00	279013.53	278934.61	262882.40
29	24.93	9.22	88.15	0.00	279022.76	279022.76	262882.40
30	26.77	18.23	0.70	0.00	279040.99	279023.45	262882.40
31	26.77	0.70	18.23	0.00	279041.68	279041.68	262882.40
32	27.85	20.38	1982.60	0.00	279062.07	281024.28	262882.40
33	27.85	1982.60	20.38	0.00	281044.67	281044.67	262882.40
34	29.06	0.01	0.00	0.00	281044.67	281044.67	262882.40
35	29.06	0.00	0.01	0.00	281044.67	281044.67	262882.40
36	30.75	0.00	0.00	2703.80	281044.67	281044.67	265586.20
37	35.77	0.00	0.00	12637.00	281044.67	281044.67	278223.20
38	39.22	0.00	0.00	1068.20	281044.67	281044.67	279291.40
39	41.72	1007.10	2196.00	0.00	282051.77	283240.67	279291.40
40	41.72	2196.00	1007.10	0.00	284247.77	284247.77	279291.40
41	45.27	0.00	0.00	368.42	284247.77	284247.77	279659.82
42	50.51	0.00	0.00	246.83	284247.77	284247.77	279906.65
43	56.27	0.00	0.00	92.42	284247.77	284247.77	279999.07
44	60.35	0.00	0.00	18.29	284247.77	284247.77	280017.36
45	61.30	0.00	0.00	318.42	284247.77	284247.77	280335.78
46	66.24	0.00	0.00	0.00	284247.77	284247.77	280335.78
47	70.53	0.00	0.00	2194.50	284247.77	284247.77	282530.28
48	82.03	210.73	4.80	0.00	284458.50	284252.58	282530.28
49	82.03	4.80	210.73	0.00	284463.31	284463.31	282530.28
50	83.07	0.00	0.00	0.00	284463.31	284463.31	282530.28
51	83.07	0.00	0.00	0.00	284463.31	284463.31	282530.28
52	86.57	0.00	0.00	1745.60	284463.31	284463.31	284275.88
53	94.21	0.00	0.00	0.00	284463.31	284463.31	284275.88
54	97.32	0.00	0.00	0.00	284463.31	284463.31	284275.88
55	97.32	0.00	0.00	0.00	284463.31	284463.31	284275.88

