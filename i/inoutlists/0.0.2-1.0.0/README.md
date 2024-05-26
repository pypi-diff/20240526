# Comparing `tmp/inoutlists-0.0.2.tar.gz` & `tmp/inoutlists-1.0.0.tar.gz`

## Comparing `inoutlists-0.0.2.tar` & `inoutlists-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 inoutlists-0.0.2/requirements.txt
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 inoutlists-0.0.2/inoutlists/OFAC_Id_Types.csv
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 inoutlists-0.0.2/inoutlists/__init__.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 inoutlists-0.0.2/inoutlists/country_ISO_codes.csv
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 inoutlists-0.0.2/inoutlists/country_names.csv
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 inoutlists-0.0.2/inoutlists/dumpers.py
--rw-r--r--   0        0        0    40979 2020-02-02 00:00:00.000000 inoutlists-0.0.2/inoutlists/loaders.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 inoutlists-0.0.2/tests/context.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 inoutlists-0.0.2/tests/lists_mapper.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 inoutlists-0.0.2/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 inoutlists-0.0.2/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 inoutlists-0.0.2/README.md
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 inoutlists-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 inoutlists-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 inoutlists-1.0.0/requirements.txt
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 inoutlists-1.0.0/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 inoutlists-1.0.0/inoutlists/OFAC_Id_Types.csv
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 inoutlists-1.0.0/inoutlists/__init__.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 inoutlists-1.0.0/inoutlists/country_ISO_codes.csv
+-rw-r--r--   0        0        0     5194 2020-02-02 00:00:00.000000 inoutlists-1.0.0/inoutlists/country_names.csv
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 inoutlists-1.0.0/inoutlists/dumpers.py
+-rw-r--r--   0        0        0    39929 2020-02-02 00:00:00.000000 inoutlists-1.0.0/inoutlists/loaders.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 inoutlists-1.0.0/tests/context.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 inoutlists-1.0.0/tests/lists_mapper.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 inoutlists-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 inoutlists-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 inoutlists-1.0.0/README.md
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 inoutlists-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10313 2020-02-02 00:00:00.000000 inoutlists-1.0.0/PKG-INFO
```

### Comparing `inoutlists-0.0.2/inoutlists/OFAC_Id_Types.csv` & `inoutlists-1.0.0/inoutlists/OFAC_Id_Types.csv`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-OFAC_ID_TYPE
-Passport
-Tax ID No.
-Registration Number
-National ID No.
-Cedula No.
-C.U.R.P.
-R.F.C.
-Government Gazette Number
-Identification Number
-NIT #
-Registration ID
-Business Registration Number
-Company Number
-Folio Mercantil No.
-RUC #
-Commercial Registry Number
-V.A.T. Number
-Trade License No.
-C.R. No.
-Legal Entity Number
-Unified Social Credit Code (USCC)
-License
-Matricula Mercantil No
-D.N.I.
-D-U-N-S Number
-Economic Register Number (CBLS)
-Business Registration Document #
-Driver's License No.
-Istanbul Chamber of Comm. No.
-Central Registration System Number
-RIF #
-BIK (RU)
-Business Number
-Diplomatic Passport
-Electoral Registry No.
-RFC
-Chamber of Commerce Number
-National Foreign ID Number
-Personal ID Card
-Enterprise Number
-Italian Fiscal Code
-Credencial electoral
-Public Registration Number
-UK Company Number
-C.U.I.
-Cartilla de Servicio Militar Nacional
-I.F.E.
-Permit Number
-Residency Number
-US FEIN
-Dubai Chamber of Commerce Membership No.
-SSN
-Registered Charity No.
-Vessel Registration Identification
-Branch Unit Number
-Certificate of Incorporation Number
-Numero de Identidad
-Turkish Identification Number
-C.U.I.T.
-Citizen's Card Number
-LE Number
-United Social Credit Code Certificate (USCCC)
-Kenyan ID No.
-RTN
-Travel Document Number
-C.U.I.P.
-VisaNumberID
-File Number
-SRE Permit No.
-Paraguayan tax identification number
-Refugee ID Card
-Romanian C.R.
-Tazkira National ID Card
-Afghan Money Service Provider License Number
-C.I.F.
-Immigration No.
-Numero Unico de Identificacao Tributaria (NUIT)
-Pilot License Number
-Bosnian Personal ID No.
-British National Overseas Passport
-Fiscal Code
-MSB Registration Number
-Moroccan Personal ID No.
-N.I.E.
-N.I.F.
-Public Security and Immigration No.
-Romanian Permanent Resident
-Romanian Tax Registration
-Seafarer's Identification Document
-Stateless Person ID Card
-Stateless Person Passport
-Tourism License No.
-Trademark number
-UAE Identification
-Aircraft Construction Number (also called L/N or S/N or F/N)
-Aircraft Manufacturer's Serial Number (MSN)
-Aircraft Tail Number
-MMSI
-Other Vessel Call Sign
-Previous Aircraft Tail Number
-SWIFT/BIC
-Military Registration Number
-C.I.N.
-Registration Certificate Number (Dubai)
+OFAC_ID_TYPE
+Passport
+Tax ID No.
+Registration Number
+National ID No.
+Cedula No.
+C.U.R.P.
+R.F.C.
+Government Gazette Number
+Identification Number
+NIT #
+Registration ID
+Business Registration Number
+Company Number
+Folio Mercantil No.
+RUC #
+Commercial Registry Number
+V.A.T. Number
+Trade License No.
+C.R. No.
+Legal Entity Number
+Unified Social Credit Code (USCC)
+License
+Matricula Mercantil No
+D.N.I.
+D-U-N-S Number
+Economic Register Number (CBLS)
+Business Registration Document #
+Driver's License No.
+Istanbul Chamber of Comm. No.
+Central Registration System Number
+RIF #
+BIK (RU)
+Business Number
+Diplomatic Passport
+Electoral Registry No.
+RFC
+Chamber of Commerce Number
+National Foreign ID Number
+Personal ID Card
+Enterprise Number
+Italian Fiscal Code
+Credencial electoral
+Public Registration Number
+UK Company Number
+C.U.I.
+Cartilla de Servicio Militar Nacional
+I.F.E.
+Permit Number
+Residency Number
+US FEIN
+Dubai Chamber of Commerce Membership No.
+SSN
+Registered Charity No.
+Vessel Registration Identification
+Branch Unit Number
+Certificate of Incorporation Number
+Numero de Identidad
+Turkish Identification Number
+C.U.I.T.
+Citizen's Card Number
+LE Number
+United Social Credit Code Certificate (USCCC)
+Kenyan ID No.
+RTN
+Travel Document Number
+C.U.I.P.
+VisaNumberID
+File Number
+SRE Permit No.
+Paraguayan tax identification number
+Refugee ID Card
+Romanian C.R.
+Tazkira National ID Card
+Afghan Money Service Provider License Number
+C.I.F.
+Immigration No.
+Numero Unico de Identificacao Tributaria (NUIT)
+Pilot License Number
+Bosnian Personal ID No.
+British National Overseas Passport
+Fiscal Code
+MSB Registration Number
+Moroccan Personal ID No.
+N.I.E.
+N.I.F.
+Public Security and Immigration No.
+Romanian Permanent Resident
+Romanian Tax Registration
+Seafarer's Identification Document
+Stateless Person ID Card
+Stateless Person Passport
+Tourism License No.
+Trademark number
+UAE Identification
+Aircraft Construction Number (also called L/N or S/N or F/N)
+Aircraft Manufacturer's Serial Number (MSN)
+Aircraft Tail Number
+MMSI
+Other Vessel Call Sign
+Previous Aircraft Tail Number
+SWIFT/BIC
+Military Registration Number
+C.I.N.
+Registration Certificate Number (Dubai)
 Russian State Individual Business Registration Number Pattern (OGRNIP)
```

### Comparing `inoutlists-0.0.2/inoutlists/country_ISO_codes.csv` & `inoutlists-1.0.0/inoutlists/country_ISO_codes.csv`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,254 +1,254 @@
-ISO2_CODE	ISO3_CODE	COUNTRY_NAME
-AF	AFG	AFGHANISTAN
-AX	ALA	ÅLAND ISLANDS
-AL	ALB	ALBANIA
-DZ	DZA	ALGERIA
-AS	ASM	AMERICAN SAMOA
-AD	AND	ANDORRA
-AO	AGO	ANGOLA
-AI	AIA	ANGUILLA
-AQ	ATA	ANTARCTICA
-AG	ATG	ANTIGUA AND BARBUDA
-AR	ARG	ARGENTINA
-AM	ARM	ARMENIA
-AW	ABW	ARUBA
-AU	AUS	AUSTRALIA
-AT	AUT	AUSTRIA
-AZ	AZE	AZERBAIJAN
-BS	BHS	BAHAMAS
-BH	BHR	BAHRAIN
-BD	BGD	BANGLADESH
-BB	BRB	BARBADOS
-BY	BLR	BELARUS
-BE	BEL	BELGIUM
-BZ	BLZ	BELIZE
-BJ	BEN	BENIN
-BM	BMU	BERMUDA
-BT	BTN	BHUTAN
-BO	BOL	BOLIVIA
-BA	BIH	BOSNIA AND HERZEGOVINA
-BW	BWA	BOTSWANA
-BV	BVT	BOUVET ISLAND
-BR	BRA	BRAZIL
-IO	IOT	BRITISH INDIAN OCEAN TERRITORY
-VG	VGB	BRITISH VIRGIN ISLANDS
-BN	BRN	BRUNEI
-BG	BGR	BULGARIA
-BF	BFA	BURKINA FASO
-BI	BDI	BURUNDI
-KH	KHM	CAMBODIA
-CM	CMR	CAMEROON
-CA	CAN	CANADA
-CV	CPV	CAPE VERDE
-BQ	BES	CARIBBEAN NETHERLANDS
-KY	CYM	CAYMAN ISLANDS
-CF	CAF	CENTRAL AFRICAN REPUBLIC
-TD	TCD	CHAD
-CL	CHL	CHILE
-CN	CHN	CHINA
-CX	CXR	CHRISTMAS ISLAND
-CC	CCK	COCOS (KEELING) ISLANDS
-CO	COL	COLOMBIA
-KM	COM	COMOROS
-CK	COK	COOK ISLANDS
-CR	CRI	COSTA RICA
-HR	HRV	CROATIA
-CU	CUB	CUBA
-CW	CUW	CURACAO
-CY	CYP	CYPRUS
-CZ	CZE	CZECHIA
-CD	COD	DEMOCRATIC REPUBLIC OF THE CONGO
-DK	DNK	DENMARK
-DJ	DJI	DJIBOUTI
-DM	DMA	DOMINICA
-DO	DOM	DOMINICAN REPUBLIC
-TL	TLS	EAST TIMOR
-EC	ECU	ECUADOR
-EG	EGY	EGYPT
-SV	SLV	EL SALVADOR
-GQ	GNQ	EQUATORIAL GUINEA
-ER	ERI	ERITREA
-EE	EST	ESTONIA
-SZ	SWZ	ESWATINI
-ET	ETH	ETHIOPIA
-FK	FLK	FALKLAND ISLANDS
-FO	FRO	FAROE ISLANDS
-FM	FSM	FEDERATED STATES OF MICRONESIA
-FJ	FJI	FIJI
-FI	FIN	FINLAND
-FR	FRA	FRANCE
-GF	GUF	FRENCH GUIANA
-PF	PYF	FRENCH POLYNESIA
-TF	ATF	FRENCH SOUTHERN AND ANTARCTIC LANDS
-GA	GAB	GABON
-GM	GMB	GAMBIA
-GE	GEO	GEORGIA
-DE	DEU	GERMANY
-GH	GHA	GHANA
-GI	GIB	GIBRALTAR
-GR	GRC	GREECE
-GL	GRL	GREENLAND
-GD	GRD	GRENADA
-GP	GLP	GUADELOUPE
-GU	GUM	GUAM
-GT	GTM	GUATEMALA
-GG	GGY	GUERNSEY
-GN	GIN	GUINEA
-GW	GNB	GUINEA-BISSAU
-GY	GUY	GUYANA
-HT	HTI	HAITI
-HM	HMD	HEARD ISLAND AND MCDONALD ISLANDS
-HN	HND	HONDURAS
-HK	HKG	HONG KONG
-HU	HUN	HUNGARY
-IS	ISL	ICELAND
-IN	IND	INDIA
-ID	IDN	INDONESIA
-IR	IRN	IRAN
-IQ	IRQ	IRAQ
-IE	IRL	IRELAND
-IM	IMN	ISLE OF MAN
-IL	ISR	ISRAEL
-IT	ITA	ITALY
-CI	CIV	IVORY COAST
-JM	JAM	JAMAICA
-JP	JPN	JAPAN
-JE	JEY	JERSEY
-JO	JOR	JORDAN
-KZ	KAZ	KAZAKHSTAN
-KE	KEN	KENYA
-KI	KIR	KIRIBATI
-XK	XXK	KOSOVO
-KW	KWT	KUWAIT
-KG	KGZ	KYRGYZSTAN
-LA	LAO	LAOS
-LV	LVA	LATVIA
-LB	LBN	LEBANON
-LS	LSO	LESOTHO
-LR	LBR	LIBERIA
-LY	LBY	LIBYA
-LI	LIE	LIECHTENSTEIN
-LT	LTU	LITHUANIA
-LU	LUX	LUXEMBOURG
-MO	MAC	MACAO
-MG	MDG	MADAGASCAR
-MW	MWI	MALAWI
-MY	MYS	MALAYSIA
-MV	MDV	MALDIVES
-ML	MLI	MALI
-MT	MLT	MALTA
-MH	MHL	MARSHALL ISLANDS
-MQ	MTQ	MARTINIQUE
-MR	MRT	MAURITANIA
-MU	MUS	MAURITIUS
-YT	MYT	MAYOTTE
-MX	MEX	MEXICO
-MD	MDA	MOLDOVA
-MN	MNG	MONGOLIA
-ME	MNE	MONTENEGRO
-MS	MSR	MONTSERRAT
-MA	MAR	MOROCCO
-MZ	MOZ	MOZAMBIQUE
-MM	MMR	MYANMAR
-NA	NAM	NAMIBIA
-NR	NRU	NAURU
-NP	NPL	NEPAL
-NL	NLD	NETHERLANDS
-NC	NCL	NEW CALEDONIA
-NZ	NZL	NEW ZEALAND
-NI	NIC	NICARAGUA
-NE	NER	NIGER
-NG	NGA	NIGERIA
-NU	NIU	NIUE
-NF	NFK	NORFOLK ISLAND
-KP	PRK	NORTH KOREA
-MK	MKD	NORTH MACEDONIA
-MP	MNP	NORTHERN MARIANA ISLANDS
-NO	NOR	NORWAY
-OM	OMN	OMAN
-PK	PAK	PAKISTAN
-PW	PLW	PALAU
-PS	PSE	PALESTINE
-PA	PAN	PANAMA
-PG	PNG	PAPUA NEW GUINEA
-PY	PRY	PARAGUAY
-PE	PER	PERU
-PH	PHL	PHILIPPINES
-PN	PCN	PITCAIRN ISLANDS
-PL	POL	POLAND
-PT	PRT	PORTUGAL
-MC	MCO	PRINCIPALITY OF MONACO
-PR	PRI	PUERTO RICO
-QA	QAT	QATAR
-CG	COG	REPUBLIC OF THE CONGO
-RE	REU	REUNION
-RO	ROU	ROMANIA
-RU	RUS	RUSSIA
-RW	RWA	RWANDA
-BL	BLM	SAINT BARTHELEMY
-SH	SHN	SAINT HELENA, ASCENSION AND TRISTAN DA CUNHA
-KN	KNA	SAINT KITTS AND NEVIS
-LC	LCA	SAINT LUCIA
-MF	MAF	SAINT MARTIN
-PM	SPM	SAINT PIERRE AND MIQUELON
-VC	VCT	SAINT VINCENT AND THE GRENADINES
-WS	WSM	SAMOA
-SM	SMR	SAN MARINO
-ST	STP	SAO TOME AND PRINCIPE
-SA	SAU	SAUDI ARABIA
-SN	SEN	SENEGAL
-RS	SRB	SERBIA
-SC	SYC	SEYCHELLES
-SL	SLE	SIERRA LEONE
-SG	SGP	SINGAPORE
-SX	SXM	SINT MAARTEN
-SK	SVK	SLOVAKIA
-SI	SVN	SLOVENIA
-SB	SLB	SOLOMON ISLANDS
-SO	SOM	SOMALIA
-ZA	ZAF	SOUTH AFRICA
-GS	SGS	SOUTH GEORGIA AND SOUTH SANDWICH ISLANDS
-KR	KOR	SOUTH KOREA
-SS	SSD	SOUTH SUDAN
-ES	ESP	SPAIN
-LK	LKA	SRI LANKA
-SD	SDN	SUDAN
-SR	SUR	SURINAME
-SJ	SJM	SVALBARD
-SE	SWE	SWEDEN
-CH	CHE	SWITZERLAND
-SY	SYR	SYRIA
-TW	TWN	TAIWAN
-TJ	TJK	TAJIKISTAN
-TZ	TZA	TANZANIA
-TH	THA	THAILAND
-TG	TGO	TOGO
-TK	TKL	TOKELAU
-TO	TON	TONGA
-TT	TTO	TRINIDAD AND TOBAGO
-TN	TUN	TUNISIA
-TR	TUR	TURKEY
-TM	TKM	TURKMENISTAN
-TC	TCA	TURKS AND CAICOS ISLANDS
-TV	TUV	TUVALU
-UG	UGA	UGANDA
-UA	UKR	UKRAINE
-AE	ARE	UNITED ARAB EMIRATES
-GB	GBR	UNITED KINGDOM
-UM	UMI	UNITED STATES MINOR OUTLYING ISLANDS
-US	USA	UNITED STATES OF AMERICA
-UY	URY	URUGUAY
-UZ	UZB	UZBEKISTAN
-VU	VUT	VANUATU
-VA	VAT	VATICAN CITY
-VE	VEN	VENEZUELA
-VN	VNM	VIETNAM
-VI	VIR	VIRGIN ISLANDS
-WF	WLF	WALLIS AND FUTUNA
-EH	ESH	WESTERN SAHARA
-YE	YEM	YEMEN
-ZM	ZMB	ZAMBIA
-ZW	ZWE	ZIMBABWE
-CS	SCG	SERBIA AND MONTENEGRO
-SU	SUN	USSR
+ISO2_CODE	ISO3_CODE	COUNTRY_NAME
+AF	AFG	AFGHANISTAN
+AX	ALA	ÅLAND ISLANDS
+AL	ALB	ALBANIA
+DZ	DZA	ALGERIA
+AS	ASM	AMERICAN SAMOA
+AD	AND	ANDORRA
+AO	AGO	ANGOLA
+AI	AIA	ANGUILLA
+AQ	ATA	ANTARCTICA
+AG	ATG	ANTIGUA AND BARBUDA
+AR	ARG	ARGENTINA
+AM	ARM	ARMENIA
+AW	ABW	ARUBA
+AU	AUS	AUSTRALIA
+AT	AUT	AUSTRIA
+AZ	AZE	AZERBAIJAN
+BS	BHS	BAHAMAS
+BH	BHR	BAHRAIN
+BD	BGD	BANGLADESH
+BB	BRB	BARBADOS
+BY	BLR	BELARUS
+BE	BEL	BELGIUM
+BZ	BLZ	BELIZE
+BJ	BEN	BENIN
+BM	BMU	BERMUDA
+BT	BTN	BHUTAN
+BO	BOL	BOLIVIA
+BA	BIH	BOSNIA AND HERZEGOVINA
+BW	BWA	BOTSWANA
+BV	BVT	BOUVET ISLAND
+BR	BRA	BRAZIL
+IO	IOT	BRITISH INDIAN OCEAN TERRITORY
+VG	VGB	BRITISH VIRGIN ISLANDS
+BN	BRN	BRUNEI
+BG	BGR	BULGARIA
+BF	BFA	BURKINA FASO
+BI	BDI	BURUNDI
+KH	KHM	CAMBODIA
+CM	CMR	CAMEROON
+CA	CAN	CANADA
+CV	CPV	CAPE VERDE
+BQ	BES	CARIBBEAN NETHERLANDS
+KY	CYM	CAYMAN ISLANDS
+CF	CAF	CENTRAL AFRICAN REPUBLIC
+TD	TCD	CHAD
+CL	CHL	CHILE
+CN	CHN	CHINA
+CX	CXR	CHRISTMAS ISLAND
+CC	CCK	COCOS (KEELING) ISLANDS
+CO	COL	COLOMBIA
+KM	COM	COMOROS
+CK	COK	COOK ISLANDS
+CR	CRI	COSTA RICA
+HR	HRV	CROATIA
+CU	CUB	CUBA
+CW	CUW	CURACAO
+CY	CYP	CYPRUS
+CZ	CZE	CZECHIA
+CD	COD	DEMOCRATIC REPUBLIC OF THE CONGO
+DK	DNK	DENMARK
+DJ	DJI	DJIBOUTI
+DM	DMA	DOMINICA
+DO	DOM	DOMINICAN REPUBLIC
+TL	TLS	EAST TIMOR
+EC	ECU	ECUADOR
+EG	EGY	EGYPT
+SV	SLV	EL SALVADOR
+GQ	GNQ	EQUATORIAL GUINEA
+ER	ERI	ERITREA
+EE	EST	ESTONIA
+SZ	SWZ	ESWATINI
+ET	ETH	ETHIOPIA
+FK	FLK	FALKLAND ISLANDS
+FO	FRO	FAROE ISLANDS
+FM	FSM	FEDERATED STATES OF MICRONESIA
+FJ	FJI	FIJI
+FI	FIN	FINLAND
+FR	FRA	FRANCE
+GF	GUF	FRENCH GUIANA
+PF	PYF	FRENCH POLYNESIA
+TF	ATF	FRENCH SOUTHERN AND ANTARCTIC LANDS
+GA	GAB	GABON
+GM	GMB	GAMBIA
+GE	GEO	GEORGIA
+DE	DEU	GERMANY
+GH	GHA	GHANA
+GI	GIB	GIBRALTAR
+GR	GRC	GREECE
+GL	GRL	GREENLAND
+GD	GRD	GRENADA
+GP	GLP	GUADELOUPE
+GU	GUM	GUAM
+GT	GTM	GUATEMALA
+GG	GGY	GUERNSEY
+GN	GIN	GUINEA
+GW	GNB	GUINEA-BISSAU
+GY	GUY	GUYANA
+HT	HTI	HAITI
+HM	HMD	HEARD ISLAND AND MCDONALD ISLANDS
+HN	HND	HONDURAS
+HK	HKG	HONG KONG
+HU	HUN	HUNGARY
+IS	ISL	ICELAND
+IN	IND	INDIA
+ID	IDN	INDONESIA
+IR	IRN	IRAN
+IQ	IRQ	IRAQ
+IE	IRL	IRELAND
+IM	IMN	ISLE OF MAN
+IL	ISR	ISRAEL
+IT	ITA	ITALY
+CI	CIV	IVORY COAST
+JM	JAM	JAMAICA
+JP	JPN	JAPAN
+JE	JEY	JERSEY
+JO	JOR	JORDAN
+KZ	KAZ	KAZAKHSTAN
+KE	KEN	KENYA
+KI	KIR	KIRIBATI
+XK	XXK	KOSOVO
+KW	KWT	KUWAIT
+KG	KGZ	KYRGYZSTAN
+LA	LAO	LAOS
+LV	LVA	LATVIA
+LB	LBN	LEBANON
+LS	LSO	LESOTHO
+LR	LBR	LIBERIA
+LY	LBY	LIBYA
+LI	LIE	LIECHTENSTEIN
+LT	LTU	LITHUANIA
+LU	LUX	LUXEMBOURG
+MO	MAC	MACAO
+MG	MDG	MADAGASCAR
+MW	MWI	MALAWI
+MY	MYS	MALAYSIA
+MV	MDV	MALDIVES
+ML	MLI	MALI
+MT	MLT	MALTA
+MH	MHL	MARSHALL ISLANDS
+MQ	MTQ	MARTINIQUE
+MR	MRT	MAURITANIA
+MU	MUS	MAURITIUS
+YT	MYT	MAYOTTE
+MX	MEX	MEXICO
+MD	MDA	MOLDOVA
+MN	MNG	MONGOLIA
+ME	MNE	MONTENEGRO
+MS	MSR	MONTSERRAT
+MA	MAR	MOROCCO
+MZ	MOZ	MOZAMBIQUE
+MM	MMR	MYANMAR
+NA	NAM	NAMIBIA
+NR	NRU	NAURU
+NP	NPL	NEPAL
+NL	NLD	NETHERLANDS
+NC	NCL	NEW CALEDONIA
+NZ	NZL	NEW ZEALAND
+NI	NIC	NICARAGUA
+NE	NER	NIGER
+NG	NGA	NIGERIA
+NU	NIU	NIUE
+NF	NFK	NORFOLK ISLAND
+KP	PRK	NORTH KOREA
+MK	MKD	NORTH MACEDONIA
+MP	MNP	NORTHERN MARIANA ISLANDS
+NO	NOR	NORWAY
+OM	OMN	OMAN
+PK	PAK	PAKISTAN
+PW	PLW	PALAU
+PS	PSE	PALESTINE
+PA	PAN	PANAMA
+PG	PNG	PAPUA NEW GUINEA
+PY	PRY	PARAGUAY
+PE	PER	PERU
+PH	PHL	PHILIPPINES
+PN	PCN	PITCAIRN ISLANDS
+PL	POL	POLAND
+PT	PRT	PORTUGAL
+MC	MCO	PRINCIPALITY OF MONACO
+PR	PRI	PUERTO RICO
+QA	QAT	QATAR
+CG	COG	REPUBLIC OF THE CONGO
+RE	REU	REUNION
+RO	ROU	ROMANIA
+RU	RUS	RUSSIA
+RW	RWA	RWANDA
+BL	BLM	SAINT BARTHELEMY
+SH	SHN	SAINT HELENA, ASCENSION AND TRISTAN DA CUNHA
+KN	KNA	SAINT KITTS AND NEVIS
+LC	LCA	SAINT LUCIA
+MF	MAF	SAINT MARTIN
+PM	SPM	SAINT PIERRE AND MIQUELON
+VC	VCT	SAINT VINCENT AND THE GRENADINES
+WS	WSM	SAMOA
+SM	SMR	SAN MARINO
+ST	STP	SAO TOME AND PRINCIPE
+SA	SAU	SAUDI ARABIA
+SN	SEN	SENEGAL
+RS	SRB	SERBIA
+SC	SYC	SEYCHELLES
+SL	SLE	SIERRA LEONE
+SG	SGP	SINGAPORE
+SX	SXM	SINT MAARTEN
+SK	SVK	SLOVAKIA
+SI	SVN	SLOVENIA
+SB	SLB	SOLOMON ISLANDS
+SO	SOM	SOMALIA
+ZA	ZAF	SOUTH AFRICA
+GS	SGS	SOUTH GEORGIA AND SOUTH SANDWICH ISLANDS
+KR	KOR	SOUTH KOREA
+SS	SSD	SOUTH SUDAN
+ES	ESP	SPAIN
+LK	LKA	SRI LANKA
+SD	SDN	SUDAN
+SR	SUR	SURINAME
+SJ	SJM	SVALBARD
+SE	SWE	SWEDEN
+CH	CHE	SWITZERLAND
+SY	SYR	SYRIA
+TW	TWN	TAIWAN
+TJ	TJK	TAJIKISTAN
+TZ	TZA	TANZANIA
+TH	THA	THAILAND
+TG	TGO	TOGO
+TK	TKL	TOKELAU
+TO	TON	TONGA
+TT	TTO	TRINIDAD AND TOBAGO
+TN	TUN	TUNISIA
+TR	TUR	TURKEY
+TM	TKM	TURKMENISTAN
+TC	TCA	TURKS AND CAICOS ISLANDS
+TV	TUV	TUVALU
+UG	UGA	UGANDA
+UA	UKR	UKRAINE
+AE	ARE	UNITED ARAB EMIRATES
+GB	GBR	UNITED KINGDOM
+UM	UMI	UNITED STATES MINOR OUTLYING ISLANDS
+US	USA	UNITED STATES OF AMERICA
+UY	URY	URUGUAY
+UZ	UZB	UZBEKISTAN
+VU	VUT	VANUATU
+VA	VAT	VATICAN CITY
+VE	VEN	VENEZUELA
+VN	VNM	VIETNAM
+VI	VIR	VIRGIN ISLANDS
+WF	WLF	WALLIS AND FUTUNA
+EH	ESH	WESTERN SAHARA
+YE	YEM	YEMEN
+ZM	ZMB	ZAMBIA
+ZW	ZWE	ZIMBABWE
+CS	SCG	SERBIA AND MONTENEGRO
+SU	SUN	USSR
 00	000	UNKNOWN
```

### Comparing `inoutlists-0.0.2/inoutlists/dumpers.py` & `inoutlists-1.0.0/inoutlists/dumpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import json
-import pandas as pd
-
-__all__ = [
-    "dump",
-    "Dumper",
-    "DumperJSON",
-    "DumperPandas",
-    "DumperCSV"
-
-]
-
-class Dumper():
-
-    def __init__(self, *args, **kwargs):
-        self.args = args
-        self.kwargs = kwargs        
-
-    def dump(self, data):
-        pass
-
-class DumperJSON(Dumper):
-
-    def dump(self, data):
-        file = self.kwargs.get("file", None)
-        if file is None:
-            return json.dumps(data, **self.kwargs)
-        else:
-            kwargs = {k:v for k,v in self.kwargs.items() if k != "file"}
-            try:
-                with open(file, mode="w", encoding="utf-8") as fileOut:
-                    json.dump(data, fileOut, **kwargs)
-                return True
-            except OSError as err:
-                print("OS error:", err)
-                return False
-            except Exception as err:
-                print(f"Unexpected {err=}, {type(err)=}")
-                return False
-
-class DumperPandas(Dumper):
-
-    def dump(self, data):        
-
-        metaFields = [            
-            "id",
-            "type"
-        ]
-        
-        recordFields = {
-            "names": {"dict": True},
-            "addresses": {"dict": True},
-            "nationalities": {"dict": True},
-            "dates_of_birth": {"dict": True},
-            "places_of_birth": {"dict": True},
-            "identifications": {"dict": True},
-            "programs": {"dict": False}
-        }
-
-        df = pd.DataFrame({metafield:[] for metafield in metaFields})
-
-        for recordFieldName, recordFieldInfo in recordFields.items():
-            dataNorm = [
-                {k:v for k, v in x.items() if k in metaFields + [recordFieldName]}
-                for x in data["list_entries"]
-            ]
-            dataNormUpdate = [
-                x.update({recordFieldName: []}) 
-                for x in dataNorm if recordFieldName not in x.keys()
-            ]
-            if recordFieldInfo["dict"]:
-                dfRecordField = pd.json_normalize(
-                    dataNorm, 
-                    recordFieldName, 
-                    metaFields,
-                    record_prefix = f'{recordFieldName}_'
-                )
-            else:
-                dfRecordField = pd.json_normalize(
-                    dataNorm, 
-                    recordFieldName, 
-                    metaFields                    
-                )
-                dfRecordField.rename(
-                    columns = {0: recordFieldName},
-                    inplace=True)
-            df = df.merge(dfRecordField, how="outer", on = metaFields)
-
-        return df
-    
-class DumperCSV(Dumper):
-    
-    def dump(self, data):
-        output = self.kwargs.get("output", None)        
-        df = dump(data, dumper=DumperPandas)
-        if output is None:
-            return df.to_csv(**self.kwargs)
-        else:
-            kwargs = {k:v for k,v in self.kwargs.items() if k != "output"}
-            try:
-                df.to_csv(output, **kwargs)
-                return True
-            except OSError as err:
-                print("OS error:", err)
-                return False            
-            except Exception as err:
-                print(f"{err=}, {type(err)=}")
-                return False
-            
-def dump(data, dumper=Dumper, *args, **kwargs):
+import json
+import pandas as pd
+
+__all__ = [
+    "dump",
+    "Dumper",
+    "DumperJSON",
+    "DumperPandas",
+    "DumperCSV"
+
+]
+
+class Dumper():
+
+    def __init__(self, *args, **kwargs):
+        self.args = args
+        self.kwargs = kwargs        
+
+    def dump(self, data):
+        pass
+
+class DumperJSON(Dumper):
+
+    def dump(self, data):
+        output = self.kwargs.get("output", None)
+        if output is None:
+            return json.dumps(data, **self.kwargs)
+        else:
+            kwargs = {k:v for k,v in self.kwargs.items() if k != "output"}
+            try:
+                with open(output, mode="w", encoding="utf-8") as fileOut:
+                    json.dump(data, fileOut, **kwargs)
+                return True
+            except OSError as err:
+                print("OS error:", err)
+                return False
+            except Exception as err:
+                print(f"Unexpected {err=}, {type(err)=}")
+                return False
+
+class DumperPandas(Dumper):
+
+    def dump(self, data):        
+
+        metaFields = [            
+            "id",
+            "type"
+        ]
+        
+        recordFields = {
+            "names": {"dict": True},
+            "addresses": {"dict": True},
+            "nationalities": {"dict": True},
+            "dates_of_birth": {"dict": True},
+            "places_of_birth": {"dict": True},
+            "identifications": {"dict": True},
+            "programs": {"dict": False}
+        }
+
+        df = pd.DataFrame({metafield:[] for metafield in metaFields})
+
+        for recordFieldName, recordFieldInfo in recordFields.items():
+            dataNorm = [
+                {k:v for k, v in x.items() if k in metaFields + [recordFieldName]}
+                for x in data["list_entries"]
+            ]
+            dataNormUpdate = [
+                x.update({recordFieldName: []}) 
+                for x in dataNorm if recordFieldName not in x.keys()
+            ]
+            if recordFieldInfo["dict"]:
+                dfRecordField = pd.json_normalize(
+                    dataNorm, 
+                    recordFieldName, 
+                    metaFields,
+                    record_prefix = f'{recordFieldName}_'
+                )
+            else:
+                dfRecordField = pd.json_normalize(
+                    dataNorm, 
+                    recordFieldName, 
+                    metaFields                    
+                )
+                dfRecordField.rename(
+                    columns = {0: recordFieldName},
+                    inplace=True)
+            df = df.merge(dfRecordField, how="outer", on = metaFields)
+
+        return df
+    
+class DumperCSV(Dumper):
+    
+    def dump(self, data):
+        output = self.kwargs.get("output", None)        
+        df = dump(data, dumper=DumperPandas)
+        if output is None:
+            return df.to_csv(**self.kwargs)
+        else:
+            kwargs = {k:v for k,v in self.kwargs.items() if k != "output"}
+            try:
+                df.to_csv(output, **kwargs)
+                return True
+            except OSError as err:
+                print("OS error:", err)
+                return False            
+            except Exception as err:
+                print(f"{err=}, {type(err)=}")
+                return False
+            
+def dump(data, dumper=Dumper, *args, **kwargs):
     return dumper(*args, **kwargs).dump(data)
```

### Comparing `inoutlists-0.0.2/inoutlists/loaders.py` & `inoutlists-1.0.0/inoutlists/loaders.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,1051 +1,1051 @@
-import lxml.etree as ET
-import csv
-from pathlib import Path
-import requests
-import os
-from datetime import datetime
-
-__all__ = [
-    "load",
-    "Loader",
-    "LoaderXML",
-    "LoaderOFACXML",
-    "LoaderEUXML",
-    "LoaderUNXML"    
-]
-
-_modulePath = Path(os.path.dirname(__file__))
-
-class Loader():
-
-    def __init__(self, description):        
-        self.meta = {
-            "description": description
-        }        
-        self.countryNames = {}
-        with open(Path(_modulePath, "country_names.csv"), 
-                  mode="r", 
-                  encoding="utf-8") as f:
-            reader = csv.DictReader(f, delimiter="\t")
-            for row in reader:
-                self.countryNames[row["COUNTRY_NAME"]] = row["ISO2_CODE"]
-        self.countryISOCodes = {}
-        with open(Path(_modulePath, "country_ISO_codes.csv"),
-                    mode="r", 
-                    encoding="utf-8") as f:
-            reader = csv.DictReader(f, delimiter="\t")
-            for row in reader:
-                self.countryISOCodes[row["ISO2_CODE"]] = row["COUNTRY_NAME"]
-
-    def load(self, data):
-        pass
-
-    def loadListEntry(self, listEntry):
-        result = {            
-            "id": self.getId(listEntry),
-            "type": self.getType(listEntry),
-            "names": self.getNames(listEntry)
-        }
-        addresses = self.getAddresses(listEntry)
-        if len(addresses) > 0:
-            result["addresses"] = addresses
-        nationalities = self.getNationalities(listEntry)
-        if len(nationalities) > 0:
-            result["nationalities"] = nationalities
-        dates_of_birth = self.getDatesOfBirth(listEntry)
-        if len(dates_of_birth) > 0:
-            result["dates_of_birth"] = dates_of_birth
-        places_of_birth = self.getPlacesOfBirth(listEntry)
-        if len(places_of_birth) > 0:
-            result["places_of_birth"] = places_of_birth
-        identifications = self.getIdentifications(listEntry)
-        if len(identifications) > 0:
-            result["identifications"] = identifications
-        programs = self.getPrograms(listEntry)
-        if len(programs) > 0:
-            result["programs"] = programs
-        additionalInformation = self.getAddtionalInformation(listEntry)
-        if bool(additionalInformation):
-            result["additional_information"] = additionalInformation
-
-        return result
-    
-    def getId(self, listEntry):
-        return ""
-    
-    def getType(self, listEntry):
-        return ""
-
-    def getNames(self, listEntry):
-        return []
-
-    def getAddresses(self, listEntry):
-        return []
-
-    def getNationalities(self, listEntry):
-        return []
-
-    def getDatesOfBirth(self, listEntry):
-        return []
-
-    def getPlacesOfBirth(self, listEntry):
-        return []
-
-    def getIdentifications(self, listEntry):
-        return []
-    
-    def getPrograms(self, listEntry):
-        return []
-    
-    def getAddtionalInformation(self, listEntry):
-        pass
-    
-    def getISOCodeFromCountryName(self, countryName):
-        return self.countryNames.get(countryName, "00")
-    
-    def getCountryNameFromISOCode(self, ISOCode):
-        return self.countryISOCodes.get(ISOCode, "UNKNOWN")
-    
-    @staticmethod
-    def lxmlFindText(element, path: str, ns: dict):
-        pathText = element.findtext(path, namespaces = ns)
-        return "" if pathText is None else pathText.strip()
-
-    @staticmethod
-    def lxmlGetAttribValue(element, attribName: str):
-        return element.attrib.get(attribName, "").strip()
-
-    @staticmethod
-    def dedupDictsList(dictsList: dict):
-        return [i for n, i in enumerate(dictsList) if i not in dictsList[:n]]
-
-    @staticmethod
-    def dedupList(dupList: list):
-        return list(dict.fromkeys(dupList))
-    
-    @staticmethod
-    def stripAdvance(string: str):
-        return " ".join(string.split()).strip()
-
-class LoaderXML(Loader):
-
-    def load(self, data_source):        
-        try:
-            if isinstance(data_source, str):
-                if data_source.startswith(('https://', 'http://')):
-                    r = requests.get(data_source)
-                    if r.status_code == 200:
-                        self.data = ET.fromstring(r.content)
-                        self.meta["source"] = data_source
-                    else:
-                        r.raise_for_status()
-                elif os.path.exists(data_source):                    
-                    self.data = ET.parse(data_source).getroot()
-                    self.meta["source"] = data_source
-                else:
-                    self.data = ET.fromstring(data_source)
-                    self.meta["source"] = "String flow"
-            elif isinstance(data_source, Path):
-                self.data = ET.parse(data_source).getroot()
-                self.meta["source"] = str(data_source.resolve())
-            else:
-                raise Exception("Data source not allowed")
-        except Exception as err:
-            print(f"{err=}, {type(err)=}")
-            
-        self.ns = self.data.nsmap
-
-class LoaderOFACXML(LoaderXML):
-
-    def __init__(self, description):
-        super().__init__(description)        
-        self.allowedIdTypes = []
-        with open(Path(_modulePath, "./OFAC_id_Types.csv"), 
-                  mode="r", 
-                  encoding="utf-8") as f:
-            reader = csv.DictReader(f)
-            for row in reader:
-                self.allowedIdTypes.append(row["OFAC_ID_TYPE"])
-
-    def load(self, data_source):        
-        super().load(data_source)
-        listDateTxt = self.lxmlFindText(
-                        self.data, 
-                        "publshInformation/Publish_Date",
-                        self.ns
-                    )
-        try:
-            listDateDt = datetime.strptime(listDateTxt, '%m/%d/%Y').date()
-            self.meta["list_date"] = listDateDt.isoformat()
-            listEntries = []
-        except Exception as err:
-            print(f"{err=}, {type(err)=}")
-            self.meta["list_date"] = ""
-        for listEntry in self.data.findall(".//sdnEntry", namespaces = self.ns):
-            listEntries.append(self.loadListEntry(listEntry))
-        return {
-            "meta": self.meta,
-            "list_entries": listEntries
-        }
-    
-    def getId(self, listEntry):
-        return self.lxmlFindText(listEntry, "uid", self.ns)    
-    
-    def getType(self, listEntry):
-        
-        sdnType = self.lxmlFindText(listEntry, "sdnType", self.ns)
-
-        if sdnType == "Entity":
-            return "O"
-        elif sdnType == "Individual":
-            return "I"
-        elif sdnType == "Vessel":
-            return "V"
-        elif sdnType == "Aircraft":
-            return "A"
-        else:
-            return "U"
-    
-    def getNames(self, listEntry):
-
-        names = []
-
-        entityType = self.getType(listEntry)
-
-        # Main Name
-
-        first_nameOFAC = self.lxmlFindText(listEntry, "firstName", self.ns)
-        last_nameOFAC = self.lxmlFindText(listEntry, "lastName", self.ns)        
-        names.append(self.getNameOFAC("strong", first_nameOFAC, last_nameOFAC, entityType))
-
-        # Aliases
-                
-        for aliasEl in listEntry.findall("akaList/aka", namespaces = self.ns):            
-            category = self.lxmlFindText(aliasEl, "category", self.ns) 
-            first_nameOFAC = self.lxmlFindText(aliasEl, "firstName", self.ns)
-            last_nameOFAC = self.lxmlFindText(aliasEl, "lastName", self.ns)            
-            names.append(self.getNameOFAC(category, first_nameOFAC, last_nameOFAC, entityType))
-
-        return self.dedupDictsList(names)    
-    
-    def getNameOFAC(self, category, first_nameOFAC, last_nameOFAC, entitytype):
-        strong = True if category == "strong" else False
-        if entitytype == "I":
-            first_name = first_nameOFAC
-            last_name = last_nameOFAC
-            whole_name = " ".join([first_name, last_name])            
-        else:
-            first_name = ""
-            last_name = ""
-            whole_name = last_nameOFAC        
-        return {
-            "whole_name": self.stripAdvance(whole_name).upper(),
-            "strong": strong,
-            "first_name": self.stripAdvance(first_name).upper(),
-            "last_name": self.stripAdvance(last_name).upper()          
-        }
-    
-    def getAddresses(self, listEntry):
-
-        addresses = []
-
-        for addressEl in listEntry.findall("addressList/address", namespaces = self.ns):            
-            
-            street1 = self.lxmlFindText(addressEl, "address1", self.ns)
-            street2 = self.lxmlFindText(addressEl, "address2", self.ns)
-            street3 = self.lxmlFindText(addressEl, "address2", self.ns)
-            street = " ".join([street1, street2, street3])            
-            city = self.lxmlFindText(addressEl, "city", self.ns)
-            country_subdivision = self.lxmlFindText(addressEl, "stateOrProvince", self.ns)
-            country_ori = self.lxmlFindText(addressEl, "country", self.ns)
-            country_ori= self.stripAdvance(country_ori).upper()
-            country_ISO_code = self.getISOCodeFromCountryName(country_ori)
-            country_desc = self.getCountryNameFromISOCode(country_ISO_code)
-            address = " ".join(
-                [
-                    street,
-                    city,
-                    country_subdivision,
-                    country_ori   
-                ]
-            )            
-            address = self.stripAdvance(address)
-            if len(address) > 0:
-                addresses.append(
-                    {
-                        "address": address.upper(),
-                        "street": self.stripAdvance(street).upper(),
-                        "city": self.stripAdvance(city).upper(),
-                        "country_subdivision": self.stripAdvance(country_subdivision).upper(),
-                        "country_ori": country_ori,
-                        "country_ISO_code": country_ISO_code,
-                        "country_desc": country_desc 
-                    }
-                )
-
-        return self.dedupDictsList(addresses)
-    
-    def getNationalities(self, listEntry):
-
-        nationalitiesPaths = [
-            "nationalityList/nationality",
-            "citizenshipList/citizenship"
-        ]
-
-        nationalities = []
-
-        for nationalitiesPath in nationalitiesPaths:
-            for nationalityEL in listEntry.findall(nationalitiesPath, namespaces = self.ns):
-                nationality_ori = self.lxmlFindText(nationalityEL, "country", self.ns)
-                nationality_ori = self.stripAdvance(nationality_ori).upper()
-                if len(nationality_ori) > 0:
-                    country_ISO_code = self.getISOCodeFromCountryName(nationality_ori)
-                    country_desc = self.getCountryNameFromISOCode(country_ISO_code)
-                    nationalities.append(
-                        {
-                            "country_ori": nationality_ori,
-                            "country_ISO_code": country_ISO_code,
-                            "country_desc": country_desc
-                        }
-                    )
-
-        return self.dedupDictsList(nationalities)
-    
-    def getDatesOfBirth(self, listEntry):
-
-        datesOfBirth = []
-        xpath = "dateOfBirthList/dateOfBirthItem"
-
-        for dobEl in listEntry.findall(xpath, namespaces = self.ns):            
-            dobOFAC = self.lxmlFindText(dobEl, "dateOfBirth", self.ns)
-            dob =  self.getISODateFromOFACDate(dobOFAC)
-            if dob is not None:            
-                dobParts = dob.split("-")
-                datesOfBirth.append(
-                    {
-                        "date_of_birth": dob if len(dobParts) == 3 else "",
-                        "year": dobParts[0],
-                        "month": dobParts[1] if len(dobParts) == 3 else "",
-                        "day": dobParts[2] if len(dobParts) == 3 else ""
-                    }
-                )
-        
-        return self.dedupDictsList(datesOfBirth)
-
-    @staticmethod
-    def getISODateFromOFACDate(OFACDate):
-
-        OFACMonths = {
-            "Jan": "01",
-            "Feb": "02",
-            "Mar": "03",
-            "Apr": "04",            
-            "May": "05",
-            "Jun": "06",
-            "Jul": "07",
-            "Aug": "08",
-            "Sep": "09",
-            "Oct": "10",
-            "Nov": "11",
-            "Dec": "12"
-        }
-        OFACDateParts = OFACDate.split(" ")
-        if len(OFACDateParts) == 0:
-            return None
-        elif len(OFACDateParts) == 1:
-            return f'{OFACDateParts[0]}'
-        elif len(OFACDateParts) == 3:
-            month = OFACMonths.get(OFACDateParts[1],"")
-            if len(month) == 0:
-                return f'{OFACDateParts[2]}'                
-            else:                
-                return f'{OFACDateParts[2]}-{month}-{OFACDateParts[0]}'
-        else:
-            return None
-        
-    def getPlacesOfBirth(self, listEntry):
-
-        placesOfBirth = []
-        xpath = "placeOfBirthList/placeOfBirthItem"
-
-        for pobEl in listEntry.findall(xpath, namespaces = self.ns):
-            pob = self.lxmlFindText(pobEl, "placeOfBirth", self.ns)
-            pob =  self.stripAdvance(pob)
-            if len(pob) > 0:
-                countryOfBirth = self.getCountryOfBirthOFAC(pob)
-                placesOfBirth.append(
-                    {
-                            "place_of_birth": pob.upper(),
-                            "street": "",
-                            "city": "",
-                            "country_subdivision": "",
-                            "country_ori": countryOfBirth["country_ori"],
-                            "country_ISO_code": countryOfBirth["country_ISO_code"],
-                            "country_desc": countryOfBirth["country_desc"]
-                    }
-                )
-
-        return self.dedupDictsList(placesOfBirth)
-    
-    def getCountryOfBirthOFAC(self, pob):
-        pobParts = pob.split(",")
-        country_ori = self.stripAdvance(pobParts[-1]).upper()
-        country_ISO_code = self.getISOCodeFromCountryName(country_ori)
-        country_desc = self.getCountryNameFromISOCode(country_ISO_code)        
-        return {
-            "country_ori": "" if country_ISO_code == "00" else country_ori,
-            "country_ISO_code": country_ISO_code,
-            "country_desc": country_desc
-        }        
-    
-    def getIdentifications(self, listEntry):        
-        
-        identifications = []
-
-        for IdEl in listEntry.findall("idList/id", namespaces = self.ns):
-            idType = self.lxmlFindText(IdEl, "idType", self.ns)
-            idNumber = self.lxmlFindText(IdEl, "idNumber", self.ns)
-            if idType in self.allowedIdTypes and len(idNumber) > 0:
-                country_ori = self.lxmlFindText(IdEl, "idCountry", self.ns)
-                country_ori = self.stripAdvance(country_ori).upper()
-                country_ISO_code = self.getISOCodeFromCountryName(country_ori)
-                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
-                identifications.append(
-                    {
-                        "type": self.stripAdvance(idType).upper(),
-                        "id": idNumber,
-                        "country_ori": country_ori,
-                        "country_ISO_code": country_ISO_code,
-                        "country_desc": country_desc
-                    }
-                )
-
-        return self.dedupDictsList(identifications)
-    
-    def getPrograms(self, listEntry):
-         
-         programs = []
-         for prEl in listEntry.findall("programList/program", namespaces = self.ns):
-             if prEl.text is not None:
-                programs.append(self.stripAdvance(prEl.text))
-
-         return self.dedupList(programs)
-    
-    def getAddtionalInformation(self, listEntry):
-
-        result = {}
-
-        remark = self.stripAdvance(
-                self.lxmlFindText(
-                    listEntry, 
-                    "remarks", 
-                    self.ns
-                )
-            )
-        if len(remark) > 0:
-            result["remarks"] = remark
-        
-        for IdEl in listEntry.findall("idList/id", namespaces = self.ns):
-            idType = self.lxmlFindText(IdEl, "idType", self.ns)
-            idNumber = self.stripAdvance(
-                            self.lxmlFindText(
-                                IdEl, 
-                                "idNumber", 
-                                self.ns
-                            )
-                        )
-            if idType not in self.allowedIdTypes and len(idNumber) > 0:                
-                idType = self.stripAdvance(idType)
-                idType = idType.replace(" ", "_")
-                idType = idType.replace(":", "")
-                if len(idNumber) > 0:
-                    result[idType.lower()] = idNumber
-        
-        return result
-
-class LoaderEUXML(LoaderXML):
-
-    def load(self, data_source):
-        super().load(data_source)
-        self.meta["list_date"] = self.lxmlGetAttribValue(self.data, "generationDate")        
-        listEntries = []
-        for listEntry in self.data.findall(".//sanctionEntity", namespaces = self.ns):
-            listEntries.append(self.loadListEntry(listEntry))
-        return {
-            "meta": self.meta,
-            "list_entries": listEntries
-        }
-    
-    def getId(self, listEntry):
-        return self.lxmlGetAttribValue(listEntry, "euReferenceNumber")
-    
-    def getType(self, listEntry):
-
-        euTypeEl = listEntry.find("subjectType", namespaces = self.ns)        
-        if euTypeEl is not None:            
-            euType = self.lxmlGetAttribValue(euTypeEl, "classificationCode")
-        else:
-            euType = ""
-
-        if euType == "P":
-            return "I"
-        elif euType == "E":
-            return "O"
-        else:
-            return "U"
-        
-    def getNames(self, listEntry):
-
-        names = []
-
-        for nameEl in listEntry.findall("nameAlias", namespaces = self.ns):            
-            strong = True if self.lxmlGetAttribValue(nameEl, "strong") == "true" else False
-            first_nameEU = self.lxmlGetAttribValue(nameEl, "firstName")
-            middle_nameEU = self.lxmlGetAttribValue(nameEl, "middleName")
-            last_nameEU = self.lxmlGetAttribValue(nameEl, "lastName")
-            whole_nameEU = self.lxmlGetAttribValue(nameEl, "wholeName")
-            first_name = " ".join([first_nameEU, middle_nameEU])            
-            names.append(
-                {                    
-                    "whole_name": self.stripAdvance(whole_nameEU).upper(),
-                    "strong": strong,
-                    "first_name": self.stripAdvance(first_name).upper(),
-                    "last_name": self.stripAdvance(last_nameEU).upper()                    
-                }
-            )
-
-        return self.dedupDictsList(names)
-    
-    def getAddresses(self, listEntry):
-
-        addresses = []
-
-        for addressEl in listEntry.findall("address", namespaces = self.ns):
-            street = self.lxmlGetAttribValue(addressEl, "street")
-            city = " ".join(
-                [
-                    self.lxmlGetAttribValue(addressEl, "place") , 
-                    self.lxmlGetAttribValue(addressEl, "city")
-                ]
-            )            
-            country_subdivision = self.lxmlGetAttribValue(addressEl, "region")
-            country_ori = self.lxmlGetAttribValue(addressEl, "countryDescription")
-            country_ori = self.stripAdvance(country_ori).upper()
-            address = " ".join(
-                [
-                    street,
-                    city,
-                    country_subdivision,
-                    "" if country_ori == "UNKNOWN" else country_ori
-                ]
-            )
-            address = self.stripAdvance(address)
-            if len(address) > 0:
-                country_ISO_code = self.getISOCodeFromCountryName(country_ori)
-                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
-                addresses.append(
-                    {
-                        "address": address.upper(),
-                        "street": self.stripAdvance(street).upper(),
-                        "city": self.stripAdvance(city).upper(),
-                        "country_subdivision": self.stripAdvance(country_subdivision).upper(),
-                        "country_ori": country_ori,
-                        "country_ISO_code": country_ISO_code,
-                        "country_desc": country_desc
-                    }
-                )
-
-        return self.dedupDictsList(addresses)
-    
-    def getNationalities(self, listEntry):
-
-        nationalities = []
-
-        for nationalityEl in listEntry.findall("citizenship", namespaces = self.ns):
-            nationality_ori = self.lxmlGetAttribValue(nationalityEl, "countryDescription")
-            nationality_ori = self.stripAdvance(nationality_ori).upper()
-            if len(nationality_ori) > 0 and nationality_ori != "UNKNOWN":
-                country_ISO_code = self.getISOCodeFromCountryName(nationality_ori)
-                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
-                nationalities.append(
-                    {
-                        "country_ori": nationality_ori,
-                        "country_ISO_code": country_ISO_code,
-                        "country_desc": country_desc
-                    }
-                )
-
-        return self.dedupDictsList(nationalities)
-    
-    def getDatesOfBirth(self, listEntry):
-
-        datesOfBirth = []
-
-        for dobEl in listEntry.findall("birthdate", namespaces = self.ns):
-
-            yearIni = self.lxmlGetAttribValue(dobEl, "yearRangeFrom")
-            yearEnd = self.lxmlGetAttribValue(dobEl, "yearRangeTo")
-
-            if len(yearIni) > 0 and len(yearEnd) > 0:
-                for year in range(int(yearIni), int(yearEnd) + 1, 1):
-                    datesOfBirth.append(
-                        {
-                            "date_of_birth": "",
-                            "year": str(year),
-                            "month": "",
-                            "day": ""
-                        }
-                    )
-            else:
-                date_of_birth = self.lxmlGetAttribValue(dobEl, "birthdate")
-                monthOri = self.lxmlGetAttribValue(dobEl, "monthOfYear")
-                month = "{:02d}".format(int(monthOri)) if len(monthOri) > 0 else ""
-                dayOri = self.lxmlGetAttribValue(dobEl, "dayOfMonth")
-                day = "{:02d}".format(int(dayOri)) if len(dayOri) > 0 else ""
-                year = self.lxmlGetAttribValue(dobEl, "year")                
-
-                if len(date_of_birth) > 0 or \
-                   len(month) > 0  or \
-                   len(day) > 0 or \
-                   len(year) > 0:
-                    
-                    datesOfBirth.append(
-                        {
-                            "date_of_birth": date_of_birth,
-                            "year": year,
-                            "month": month,
-                            "day": day
-                        }
-                    )
-
-        return self.dedupDictsList(datesOfBirth)
-    
-    def getPlacesOfBirth(self, listEntry):
-
-        placesOfBirth = []
-
-        for pobEl in listEntry.findall("birthdate", namespaces = self.ns):
-            street = ""
-            city = " ".join(
-                [
-                    self.lxmlGetAttribValue(pobEl, "place"), 
-                    self.lxmlGetAttribValue(pobEl, "city")
-                ]
-            )
-            country_subdivision = self.lxmlGetAttribValue(pobEl, "region")            
-            country_ori = self.lxmlGetAttribValue(pobEl, "countryDescription")
-            country_ori = self.stripAdvance(country_ori).upper()
-            pob = " ".join(
-                    [
-                        street,
-                        city,
-                        country_subdivision,
-                        "" if country_ori == "UNKNOWN"  else country_ori
-                    ]
-                )               
-            pob = self.stripAdvance(pob)
-            if len(pob) > 0:
-                country_ISO_code = self.getISOCodeFromCountryName(country_ori)
-                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
-                placesOfBirth.append(
-                    {
-                        "place_of_birth": pob.upper(),
-                        "street": self.stripAdvance(street).upper(),
-                        "city": self.stripAdvance(city).upper(),
-                        "country_subdivision": self.stripAdvance(country_subdivision).upper(),
-                        "country_ori": country_ori,
-                        "country_ISO_code": country_ISO_code,
-                        "country_desc": country_desc
-                    }
-                )
-
-        return self.dedupDictsList(placesOfBirth)
-    
-    def getIdentifications(self, listEntry):
-
-        identifications = []
-
-        for IdEl in listEntry.findall("identification", namespaces = self.ns):
-            idNumber =  self.lxmlGetAttribValue(IdEl, "number")
-            if len(idNumber) > 0:
-                idType = self.lxmlGetAttribValue(IdEl, "identificationTypeDescription")
-                country_ori = self.lxmlGetAttribValue(IdEl, "countryDescription")
-                country_ori = self.stripAdvance(country_ori).upper()
-                country_ISO_code = self.getISOCodeFromCountryName(country_ori)
-                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
-                identifications.append(
-                    {
-                        "type": self.stripAdvance(idType).upper(),
-                        "id": idNumber,
-                        "country_ori": country_ori,
-                        "country_ISO_code": country_ISO_code,
-                        "country_desc": country_desc
-                    }
-                )
-
-        return self.dedupDictsList(identifications)
-    
-    def getPrograms(self, listEntry):
-         
-        regulationEl = listEntry.find("regulation", namespaces = self.ns)
-        if regulationEl is not None:
-            program = self.stripAdvance(
-                self.lxmlGetAttribValue(regulationEl, "programme")
-            )
-        else:
-            program = ""
-        if len(program) > 0:
-            return [program]
-        else:
-            return []
-        
-    def getAddtionalInformation(self, listEntry):
-
-        result = {}
-        
-        remarks = []
-        for remarkEL in listEntry.findall("remark", namespaces = self.ns):
-            if remarkEL is not None:
-                remarks.append(remarkEL.text)
-
-        remark = " ".join(remarks)
-        remark = self.stripAdvance(remark)
-        
-        if len(remark) > 0:
-            result["remarks"] = remark
-
-        return result
-    
-class LoaderUNXML(LoaderXML):
-    
-    def load(self, data_source):
-        super().load(data_source)
-        self.listEntryPath = ""
-        self.meta["list_date"] = self.lxmlGetAttribValue(self.data, "dateGenerated")
-        
-        listEntries = []
-        listEntryPaths = [
-            ".//INDIVIDUALS/INDIVIDUAL",
-            ".//ENTITIES/ENTITY"
-        ]
-        for listEntryPath in listEntryPaths:
-            self.listEntryPath = listEntryPath
-            for listEntry in self.data.findall(
-                listEntryPath,
-                namespaces=self.ns):
-                listEntries.append(self.loadListEntry(listEntry))
-
-        return {
-            "meta": self.meta,
-            "list_entries": listEntries
-        }
-    
-    def getId(self, listEntry):
-        return self.lxmlFindText(listEntry, "REFERENCE_NUMBER", self.ns)
-    
-    def getType(self, listEntry):
-        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
-            return "I"
-        elif self.listEntryPath == ".//ENTITIES/ENTITY":
-            return "O"
-        else:
-            return "U"
-        
-    def getNames(self, listEntry):
-        
-        names = []
-
-        entityType = self.getType(listEntry)
-        
-        # Main Name        
-
-        first_nameUN = self.lxmlFindText(listEntry, "FIRST_NAME", self.ns)
-        second_nameUN = self.lxmlFindText(listEntry, "SECOND_NAME", self.ns)
-        third_nameUN = self.lxmlFindText(listEntry, "THIRD_NAME", self.ns)
-        fourth_nameUN = self.lxmlFindText(listEntry, "FOURTH_NAME", self.ns)
-
-        if entityType == "I":
-            whole_name = " ".join(
-                [
-                    first_nameUN, 
-                    second_nameUN, 
-                    third_nameUN, 
-                    fourth_nameUN
-                ]
-            )            
-            names.append(
-                {
-                    "whole_name": self.stripAdvance(whole_name).upper(),
-                    "strong": True, 
-                    "first_name": "", 
-                    "last_name": ""
-                }
-            )
-        else:
-            names.append(
-                {
-                    "whole_name": self.stripAdvance(first_nameUN).upper(),
-                    "strong": True, 
-                    "first_name": "", 
-                    "last_name": ""
-                }
-            )
-
-        # Main Name Original Script
-        
-        name_original_script = self.lxmlFindText(listEntry, "NAME_ORIGINAL_SCRIPT", self.ns)
-        if len(name_original_script) > 0:
-            names.append(
-                {
-                    "whole_name": self.stripAdvance(name_original_script).upper(),
-                    "strong": True, 
-                    "first_name": "", 
-                    "last_name": ""
-                }
-            )
-
-        # Aliases
-
-        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
-            aliasesPath = "INDIVIDUAL_ALIAS"
-        else:
-            aliasesPath = "ENTITY_ALIAS"
-
-        for alias in listEntry.findall(aliasesPath, namespaces=self.ns):            
-            aliasName = self.lxmlFindText(alias, "ALIAS_NAME", self.ns)
-            aliasName = self.stripAdvance(aliasName)
-            if len(aliasName) > 0:
-                quality = self.lxmlFindText(alias, "QUALITY", self.ns)
-                strong = False if quality == "Low" else True                
-                names.append(
-                    {
-                        "whole_name": aliasName.upper(),
-                        "strong": strong, 
-                        "first_name": "", 
-                        "last_name": ""
-                    }
-                )
-
-        return self.dedupDictsList(names)
-    
-    def getAddresses(self, listEntry):
-
-        addresses = []
-
-        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
-            addressesPath = "INDIVIDUAL_ADDRESS"
-        else:
-            addressesPath = "ENTITY_ADDRESS"
-
-        for address in listEntry.findall(addressesPath, namespaces = self.ns):
-            street = self.lxmlFindText(address, "STREET", self.ns)
-            city = self.lxmlFindText(address, "CITY", self.ns)
-            country_subdivision = self.lxmlFindText(address, "STATE_PROVINCE", self.ns)
-            country_ori =  self.lxmlFindText(address, "COUNTRY", self.ns)
-            country_ori = self.stripAdvance(country_ori).upper()
-            address = " ".join(
-                [
-                    street,
-                    city,
-                    country_subdivision,
-                    country_ori   
-                ]
-            )
-            address = self.stripAdvance(address)
-            if len(address) > 0:
-                country_ISO_code = self.getISOCodeFromCountryName(country_ori)
-                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
-                addresses.append(
-                    {
-                        "address": address.upper(),
-                        "street": self.stripAdvance(street).upper(),
-                        "city": self.stripAdvance(city).upper(),
-                        "country_subdivision": self.stripAdvance(country_subdivision).upper(),
-                        "country_ori": country_ori,
-                        "country_ISO_code": country_ISO_code,
-                        "country_desc": country_desc
-                    }
-                )
-        return self.dedupDictsList(addresses)
-    
-    def getNationalities(self, listEntry):
-
-        nationalities = []
-
-        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
-            for nationalityEl in listEntry.findall("NATIONALITY/VALUE", namespaces = self.ns):
-                if nationalityEl.text is not None:
-                    nationality_ori = nationalityEl.text 
-                    nationality_ori = self.stripAdvance(nationality_ori).upper()
-                else:
-                    nationality_ori = ""
-                if len(nationality_ori) > 0:
-                    country_ISO_code = self.getISOCodeFromCountryName(nationality_ori)
-                    country_desc = self.getCountryNameFromISOCode(country_ISO_code)
-                    nationalities.append(
-                         {
-                            "country_ori": nationality_ori,
-                            "country_ISO_code": country_ISO_code,
-                            "country_desc": country_desc
-                        }
-                    )
-
-        return self.dedupDictsList(nationalities)
-
-    def getDatesOfBirth(self, listEntry):
-
-        datesOfBirth = []
-
-        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
-            for dobEl in listEntry.findall("INDIVIDUAL_DATE_OF_BIRTH", namespaces = self.ns):
-
-                yearIni = self.lxmlFindText(dobEl, "FROM_YEAR", self.ns)
-                yearEnd = self.lxmlFindText(dobEl, "TO_YEAR", self.ns)
-
-                if len(yearIni) > 0 and len(yearEnd) > 0:
-
-                    for year in range(int(yearIni), int(yearEnd) + 1, 1):
-                        datesOfBirth.append(
-                            {
-                                "date_of_birth": "",
-                                "year": str(year),
-                                "month": "",
-                                "day": ""
-                            }
-                        )
-
-                else:
-
-                    date_of_birth = self.lxmlFindText(dobEl, "DATE", self.ns)
-                    if len(date_of_birth) > 0:
-                        date_of_birthParts = date_of_birth.split("-")
-                        day = date_of_birthParts[2]
-                        month = date_of_birthParts[1]
-                        year = date_of_birthParts[0]
-                    else:
-                        day = ""
-                        month = ""
-                        year = self.lxmlFindText(dobEl, "YEAR", self.ns)
-                    if len(date_of_birth) > 0 or \
-                       len(day) > 0 or \
-                       len(month) > 0 or \
-                       len(year) > 0:
-                        datesOfBirth.append(
-                            {
-                                "date_of_birth": date_of_birth,
-                                "year": year,
-                                "month": month,
-                                "day": day
-                            }
-                        )
-
-        return self.dedupDictsList(datesOfBirth)
-    
-    def getPlacesOfBirth(self, listEntry):
-
-        placesOfBirth = []
-
-        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
-
-            for pobEl in listEntry.findall("INDIVIDUAL_PLACE_OF_BIRTH", namespaces = self.ns):
-
-                street = self.lxmlFindText(pobEl, "STREET", self.ns)
-                city = self.lxmlFindText(pobEl, "CITY", self.ns)
-                country_subdivision = self.lxmlFindText(pobEl, "STATE_PROVINCE", self.ns)
-                country_ori = self.lxmlFindText(pobEl, "COUNTRY", self.ns)
-                country_ori = self.stripAdvance(country_ori).upper()
-                pob = " ".join(
-                    [
-                        street,
-                        city,
-                        country_subdivision,
-                        country_ori
-                    ]
-                )               
-                pob = self.stripAdvance(pob)
-                if len(pob) > 0:
-                    country_ISO_code = self.getISOCodeFromCountryName(country_ori)
-                    country_desc = self.getCountryNameFromISOCode(country_ISO_code)
-                    placesOfBirth.append(
-                        {
-                            "place_of_birth": pob.upper(),
-                            "street": self.stripAdvance(street).upper(),
-                            "city": self.stripAdvance(city).upper(),
-                            "country_subdivision": self.stripAdvance(country_subdivision).upper(),
-                            "country_ori": country_ori,
-                            "country_ISO_code": country_ISO_code,
-                            "country_desc": country_desc
-                        }
-                    )
-
-        return self.dedupDictsList(placesOfBirth)
-    
-    def getIdentifications(self, listEntry):
-
-        identifications = []
-
-        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
-
-            for IdEl in listEntry.findall("INDIVIDUAL_DOCUMENT", namespaces = self.ns):
-                idNumber = self.lxmlFindText(IdEl, "NUMBER", self.ns)
-                if len(idNumber) > 0:
-                    idType = self.lxmlFindText(IdEl, "TYPE_OF_DOCUMENT", self.ns)
-                    country1 = self.lxmlFindText(IdEl, "COUNTRY_OF_ISSUE", self.ns)
-                    country1 = self.stripAdvance(country1).upper()
-                    country2 = self.lxmlFindText(IdEl, "ISSUING_COUNTRY", self.ns)
-                    country2 = self.stripAdvance(country2).upper()
-                    if country1 == country2:
-                        country_ori = country1
-                    else:
-                        if len(country1) > 0:
-                            country_ori = country1
-                        else:
-                            country_ori = country2
-                    country_ISO_code = self.getISOCodeFromCountryName(country_ori)
-                    country_desc = self.getCountryNameFromISOCode(country_ISO_code)
-                    identifications.append(
-                        {
-                            "type": self.stripAdvance(idType).upper(),
-                            "id": idNumber,
-                            "country_ori": country_ori,
-                            "country_ISO_code": country_ISO_code,
-                            "country_desc": country_desc
-                        }
-                    )
-
-        return self.dedupDictsList(identifications)
-    
-    def getPrograms(self, listEntry):
-
-        listType = self.lxmlFindText(listEntry, "UN_LIST_TYPE", ns=self.ns)
-        listType = self.stripAdvance(listType)        
-        
-        if len(listType) > 0:
-            return [listType]
-        else:
-            return []
-        
-    def getAddtionalInformation(self, listEntry):
-
-        result = {}
-        
-        remarks = [self.lxmlFindText(listEntry, "COMMENTS1", ns=self.ns)]
-        for designationEl in listEntry.findall("DESIGNATION/VALUE", namespaces=self.ns):
-            if designationEl.text is not None:
-                remarks.append(designationEl.text)
-
-        remark = " ".join(remarks)
-        remark = self.stripAdvance(remark)
-
-        if len(remark) > 0:
-            result["remarks"] = remark
-
-        gender = self.lxmlFindText(listEntry, "GENDER", ns=self.ns)
-        gender = self.stripAdvance(gender)
-        if len(gender) > 0:                     
-            result["gender"] = gender
-        
-        return result
-    
-def load(data, loader=Loader, description=""):
+import lxml.etree as ET
+import csv
+from pathlib import Path
+import requests
+import os
+from datetime import datetime
+
+__all__ = [
+    "load",
+    "Loader",
+    "LoaderXML",
+    "LoaderOFACXML",
+    "LoaderEUXML",
+    "LoaderUNXML"    
+]
+
+_modulePath = Path(os.path.dirname(__file__))
+
+class Loader():
+
+    def __init__(self, description):        
+        self.meta = {
+            "description": description
+        }        
+        self.countryNames = {}
+        with open(Path(_modulePath, "country_names.csv"), 
+                  mode="r", 
+                  encoding="utf-8") as f:
+            reader = csv.DictReader(f, delimiter="\t")
+            for row in reader:
+                self.countryNames[row["COUNTRY_NAME"]] = row["ISO2_CODE"]
+        self.countryISOCodes = {}
+        with open(Path(_modulePath, "country_ISO_codes.csv"),
+                    mode="r", 
+                    encoding="utf-8") as f:
+            reader = csv.DictReader(f, delimiter="\t")
+            for row in reader:
+                self.countryISOCodes[row["ISO2_CODE"]] = row["COUNTRY_NAME"]
+
+    def load(self, data):
+        pass
+
+    def loadListEntry(self, listEntry):
+        result = {            
+            "id": self.getId(listEntry),
+            "type": self.getType(listEntry),
+            "names": self.getNames(listEntry)
+        }
+        addresses = self.getAddresses(listEntry)
+        if len(addresses) > 0:
+            result["addresses"] = addresses
+        nationalities = self.getNationalities(listEntry)
+        if len(nationalities) > 0:
+            result["nationalities"] = nationalities
+        dates_of_birth = self.getDatesOfBirth(listEntry)
+        if len(dates_of_birth) > 0:
+            result["dates_of_birth"] = dates_of_birth
+        places_of_birth = self.getPlacesOfBirth(listEntry)
+        if len(places_of_birth) > 0:
+            result["places_of_birth"] = places_of_birth
+        identifications = self.getIdentifications(listEntry)
+        if len(identifications) > 0:
+            result["identifications"] = identifications
+        programs = self.getPrograms(listEntry)
+        if len(programs) > 0:
+            result["programs"] = programs
+        additionalInformation = self.getAddtionalInformation(listEntry)
+        if bool(additionalInformation):
+            result["additional_information"] = additionalInformation
+
+        return result
+    
+    def getId(self, listEntry):
+        return ""
+    
+    def getType(self, listEntry):
+        return ""
+
+    def getNames(self, listEntry):
+        return []
+
+    def getAddresses(self, listEntry):
+        return []
+
+    def getNationalities(self, listEntry):
+        return []
+
+    def getDatesOfBirth(self, listEntry):
+        return []
+
+    def getPlacesOfBirth(self, listEntry):
+        return []
+
+    def getIdentifications(self, listEntry):
+        return []
+    
+    def getPrograms(self, listEntry):
+        return []
+    
+    def getAddtionalInformation(self, listEntry):
+        pass
+    
+    def getISOCodeFromCountryName(self, countryName):
+        return self.countryNames.get(countryName, "00")
+    
+    def getCountryNameFromISOCode(self, ISOCode):
+        return self.countryISOCodes.get(ISOCode, "UNKNOWN")
+    
+    @staticmethod
+    def lxmlFindText(element, path: str, ns: dict):
+        pathText = element.findtext(path, namespaces = ns)
+        return "" if pathText is None else pathText.strip()
+
+    @staticmethod
+    def lxmlGetAttribValue(element, attribName: str):
+        return element.attrib.get(attribName, "").strip()
+
+    @staticmethod
+    def dedupDictsList(dictsList: dict):
+        return [i for n, i in enumerate(dictsList) if i not in dictsList[:n]]
+
+    @staticmethod
+    def dedupList(dupList: list):
+        return list(dict.fromkeys(dupList))
+    
+    @staticmethod
+    def stripAdvance(string: str):
+        return " ".join(string.split()).strip()
+
+class LoaderXML(Loader):
+
+    def load(self, data_source):        
+        try:
+            if isinstance(data_source, str):
+                if data_source.startswith(('https://', 'http://')):
+                    r = requests.get(data_source)
+                    if r.status_code == 200:
+                        self.data = ET.fromstring(r.content)
+                        self.meta["source"] = data_source
+                    else:
+                        r.raise_for_status()
+                elif os.path.exists(data_source):                    
+                    self.data = ET.parse(data_source).getroot()
+                    self.meta["source"] = data_source
+                else:
+                    self.data = ET.fromstring(data_source)
+                    self.meta["source"] = "String flow"
+            elif isinstance(data_source, Path):
+                self.data = ET.parse(data_source).getroot()
+                self.meta["source"] = str(data_source.resolve())
+            else:
+                raise Exception("Data source not allowed")
+        except Exception as err:
+            print(f"{err=}, {type(err)=}")
+            
+        self.ns = self.data.nsmap
+
+class LoaderOFACXML(LoaderXML):
+
+    def __init__(self, description):
+        super().__init__(description)        
+        self.allowedIdTypes = []
+        with open(Path(_modulePath, "./OFAC_id_Types.csv"), 
+                  mode="r", 
+                  encoding="utf-8") as f:
+            reader = csv.DictReader(f)
+            for row in reader:
+                self.allowedIdTypes.append(row["OFAC_ID_TYPE"])
+
+    def load(self, data_source):        
+        super().load(data_source)
+        listDateTxt = self.lxmlFindText(
+                        self.data, 
+                        "publshInformation/Publish_Date",
+                        self.ns
+                    )
+        try:
+            listDateDt = datetime.strptime(listDateTxt, '%m/%d/%Y').date()
+            self.meta["list_date"] = listDateDt.isoformat()
+            listEntries = []
+        except Exception as err:
+            print(f"{err=}, {type(err)=}")
+            self.meta["list_date"] = ""
+        for listEntry in self.data.findall(".//sdnEntry", namespaces = self.ns):
+            listEntries.append(self.loadListEntry(listEntry))
+        return {
+            "meta": self.meta,
+            "list_entries": listEntries
+        }
+    
+    def getId(self, listEntry):
+        return self.lxmlFindText(listEntry, "uid", self.ns)    
+    
+    def getType(self, listEntry):
+        
+        sdnType = self.lxmlFindText(listEntry, "sdnType", self.ns)
+
+        if sdnType == "Entity":
+            return "O"
+        elif sdnType == "Individual":
+            return "I"
+        elif sdnType == "Vessel":
+            return "V"
+        elif sdnType == "Aircraft":
+            return "A"
+        else:
+            return "U"
+    
+    def getNames(self, listEntry):
+
+        names = []
+
+        entityType = self.getType(listEntry)
+
+        # Main Name
+
+        first_nameOFAC = self.lxmlFindText(listEntry, "firstName", self.ns)
+        last_nameOFAC = self.lxmlFindText(listEntry, "lastName", self.ns)        
+        names.append(self.getNameOFAC("strong", first_nameOFAC, last_nameOFAC, entityType))
+
+        # Aliases
+                
+        for aliasEl in listEntry.findall("akaList/aka", namespaces = self.ns):            
+            category = self.lxmlFindText(aliasEl, "category", self.ns) 
+            first_nameOFAC = self.lxmlFindText(aliasEl, "firstName", self.ns)
+            last_nameOFAC = self.lxmlFindText(aliasEl, "lastName", self.ns)            
+            names.append(self.getNameOFAC(category, first_nameOFAC, last_nameOFAC, entityType))
+
+        return self.dedupDictsList(names)    
+    
+    def getNameOFAC(self, category, first_nameOFAC, last_nameOFAC, entitytype):
+        strong = True if category == "strong" else False
+        if entitytype == "I":
+            first_name = first_nameOFAC
+            last_name = last_nameOFAC
+            whole_name = " ".join([first_name, last_name])            
+        else:
+            first_name = ""
+            last_name = ""
+            whole_name = last_nameOFAC        
+        return {
+            "whole_name": self.stripAdvance(whole_name).upper(),
+            "strong": strong,
+            "first_name": self.stripAdvance(first_name).upper(),
+            "last_name": self.stripAdvance(last_name).upper()          
+        }
+    
+    def getAddresses(self, listEntry):
+
+        addresses = []
+
+        for addressEl in listEntry.findall("addressList/address", namespaces = self.ns):            
+            
+            street1 = self.lxmlFindText(addressEl, "address1", self.ns)
+            street2 = self.lxmlFindText(addressEl, "address2", self.ns)
+            street3 = self.lxmlFindText(addressEl, "address2", self.ns)
+            street = " ".join([street1, street2, street3])            
+            city = self.lxmlFindText(addressEl, "city", self.ns)
+            country_subdivision = self.lxmlFindText(addressEl, "stateOrProvince", self.ns)
+            country_ori = self.lxmlFindText(addressEl, "country", self.ns)
+            country_ori= self.stripAdvance(country_ori).upper()
+            country_ISO_code = self.getISOCodeFromCountryName(country_ori)
+            country_desc = self.getCountryNameFromISOCode(country_ISO_code)
+            address = " ".join(
+                [
+                    street,
+                    city,
+                    country_subdivision,
+                    country_ori   
+                ]
+            )            
+            address = self.stripAdvance(address)
+            if len(address) > 0:
+                addresses.append(
+                    {
+                        "address": address.upper(),
+                        "street": self.stripAdvance(street).upper(),
+                        "city": self.stripAdvance(city).upper(),
+                        "country_subdivision": self.stripAdvance(country_subdivision).upper(),
+                        "country_ori": country_ori,
+                        "country_ISO_code": country_ISO_code,
+                        "country_desc": country_desc 
+                    }
+                )
+
+        return self.dedupDictsList(addresses)
+    
+    def getNationalities(self, listEntry):
+
+        nationalitiesPaths = [
+            "nationalityList/nationality",
+            "citizenshipList/citizenship"
+        ]
+
+        nationalities = []
+
+        for nationalitiesPath in nationalitiesPaths:
+            for nationalityEL in listEntry.findall(nationalitiesPath, namespaces = self.ns):
+                nationality_ori = self.lxmlFindText(nationalityEL, "country", self.ns)
+                nationality_ori = self.stripAdvance(nationality_ori).upper()
+                if len(nationality_ori) > 0:
+                    country_ISO_code = self.getISOCodeFromCountryName(nationality_ori)
+                    country_desc = self.getCountryNameFromISOCode(country_ISO_code)
+                    nationalities.append(
+                        {
+                            "country_ori": nationality_ori,
+                            "country_ISO_code": country_ISO_code,
+                            "country_desc": country_desc
+                        }
+                    )
+
+        return self.dedupDictsList(nationalities)
+    
+    def getDatesOfBirth(self, listEntry):
+
+        datesOfBirth = []
+        xpath = "dateOfBirthList/dateOfBirthItem"
+
+        for dobEl in listEntry.findall(xpath, namespaces = self.ns):            
+            dobOFAC = self.lxmlFindText(dobEl, "dateOfBirth", self.ns)
+            dob =  self.getISODateFromOFACDate(dobOFAC)
+            if dob is not None:            
+                dobParts = dob.split("-")
+                datesOfBirth.append(
+                    {
+                        "date_of_birth": dob if len(dobParts) == 3 else "",
+                        "year": dobParts[0],
+                        "month": dobParts[1] if len(dobParts) == 3 else "",
+                        "day": dobParts[2] if len(dobParts) == 3 else ""
+                    }
+                )
+        
+        return self.dedupDictsList(datesOfBirth)
+
+    @staticmethod
+    def getISODateFromOFACDate(OFACDate):
+
+        OFACMonths = {
+            "Jan": "01",
+            "Feb": "02",
+            "Mar": "03",
+            "Apr": "04",            
+            "May": "05",
+            "Jun": "06",
+            "Jul": "07",
+            "Aug": "08",
+            "Sep": "09",
+            "Oct": "10",
+            "Nov": "11",
+            "Dec": "12"
+        }
+        OFACDateParts = OFACDate.split(" ")
+        if len(OFACDateParts) == 0:
+            return None
+        elif len(OFACDateParts) == 1:
+            return f'{OFACDateParts[0]}'
+        elif len(OFACDateParts) == 3:
+            month = OFACMonths.get(OFACDateParts[1],"")
+            if len(month) == 0:
+                return f'{OFACDateParts[2]}'                
+            else:                
+                return f'{OFACDateParts[2]}-{month}-{OFACDateParts[0]}'
+        else:
+            return None
+        
+    def getPlacesOfBirth(self, listEntry):
+
+        placesOfBirth = []
+        xpath = "placeOfBirthList/placeOfBirthItem"
+
+        for pobEl in listEntry.findall(xpath, namespaces = self.ns):
+            pob = self.lxmlFindText(pobEl, "placeOfBirth", self.ns)
+            pob =  self.stripAdvance(pob)
+            if len(pob) > 0:
+                countryOfBirth = self.getCountryOfBirthOFAC(pob)
+                placesOfBirth.append(
+                    {
+                            "place_of_birth": pob.upper(),
+                            "street": "",
+                            "city": "",
+                            "country_subdivision": "",
+                            "country_ori": countryOfBirth["country_ori"],
+                            "country_ISO_code": countryOfBirth["country_ISO_code"],
+                            "country_desc": countryOfBirth["country_desc"]
+                    }
+                )
+
+        return self.dedupDictsList(placesOfBirth)
+    
+    def getCountryOfBirthOFAC(self, pob):
+        pobParts = pob.split(",")
+        country_ori = self.stripAdvance(pobParts[-1]).upper()
+        country_ISO_code = self.getISOCodeFromCountryName(country_ori)
+        country_desc = self.getCountryNameFromISOCode(country_ISO_code)        
+        return {
+            "country_ori": "" if country_ISO_code == "00" else country_ori,
+            "country_ISO_code": country_ISO_code,
+            "country_desc": country_desc
+        }        
+    
+    def getIdentifications(self, listEntry):        
+        
+        identifications = []
+
+        for IdEl in listEntry.findall("idList/id", namespaces = self.ns):
+            idType = self.lxmlFindText(IdEl, "idType", self.ns)
+            idNumber = self.lxmlFindText(IdEl, "idNumber", self.ns)
+            if idType in self.allowedIdTypes and len(idNumber) > 0:
+                country_ori = self.lxmlFindText(IdEl, "idCountry", self.ns)
+                country_ori = self.stripAdvance(country_ori).upper()
+                country_ISO_code = self.getISOCodeFromCountryName(country_ori)
+                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
+                identifications.append(
+                    {
+                        "type": self.stripAdvance(idType).upper(),
+                        "id": idNumber,
+                        "country_ori": country_ori,
+                        "country_ISO_code": country_ISO_code,
+                        "country_desc": country_desc
+                    }
+                )
+
+        return self.dedupDictsList(identifications)
+    
+    def getPrograms(self, listEntry):
+         
+         programs = []
+         for prEl in listEntry.findall("programList/program", namespaces = self.ns):
+             if prEl.text is not None:
+                programs.append(self.stripAdvance(prEl.text))
+
+         return self.dedupList(programs)
+    
+    def getAddtionalInformation(self, listEntry):
+
+        result = {}
+
+        remark = self.stripAdvance(
+                self.lxmlFindText(
+                    listEntry, 
+                    "remarks", 
+                    self.ns
+                )
+            )
+        if len(remark) > 0:
+            result["remarks"] = remark
+        
+        for IdEl in listEntry.findall("idList/id", namespaces = self.ns):
+            idType = self.lxmlFindText(IdEl, "idType", self.ns)
+            idNumber = self.stripAdvance(
+                            self.lxmlFindText(
+                                IdEl, 
+                                "idNumber", 
+                                self.ns
+                            )
+                        )
+            if idType not in self.allowedIdTypes and len(idNumber) > 0:                
+                idType = self.stripAdvance(idType)
+                idType = idType.replace(" ", "_")
+                idType = idType.replace(":", "")
+                if len(idNumber) > 0:
+                    result[idType.lower()] = idNumber
+        
+        return result
+
+class LoaderEUXML(LoaderXML):
+
+    def load(self, data_source):
+        super().load(data_source)
+        self.meta["list_date"] = self.lxmlGetAttribValue(self.data, "generationDate")        
+        listEntries = []
+        for listEntry in self.data.findall(".//sanctionEntity", namespaces = self.ns):
+            listEntries.append(self.loadListEntry(listEntry))
+        return {
+            "meta": self.meta,
+            "list_entries": listEntries
+        }
+    
+    def getId(self, listEntry):
+        return self.lxmlGetAttribValue(listEntry, "euReferenceNumber")
+    
+    def getType(self, listEntry):
+
+        euTypeEl = listEntry.find("subjectType", namespaces = self.ns)        
+        if euTypeEl is not None:            
+            euType = self.lxmlGetAttribValue(euTypeEl, "classificationCode")
+        else:
+            euType = ""
+
+        if euType == "P":
+            return "I"
+        elif euType == "E":
+            return "O"
+        else:
+            return "U"
+        
+    def getNames(self, listEntry):
+
+        names = []
+
+        for nameEl in listEntry.findall("nameAlias", namespaces = self.ns):            
+            strong = True if self.lxmlGetAttribValue(nameEl, "strong") == "true" else False
+            first_nameEU = self.lxmlGetAttribValue(nameEl, "firstName")
+            middle_nameEU = self.lxmlGetAttribValue(nameEl, "middleName")
+            last_nameEU = self.lxmlGetAttribValue(nameEl, "lastName")
+            whole_nameEU = self.lxmlGetAttribValue(nameEl, "wholeName")
+            first_name = " ".join([first_nameEU, middle_nameEU])            
+            names.append(
+                {                    
+                    "whole_name": self.stripAdvance(whole_nameEU).upper(),
+                    "strong": strong,
+                    "first_name": self.stripAdvance(first_name).upper(),
+                    "last_name": self.stripAdvance(last_nameEU).upper()                    
+                }
+            )
+
+        return self.dedupDictsList(names)
+    
+    def getAddresses(self, listEntry):
+
+        addresses = []
+
+        for addressEl in listEntry.findall("address", namespaces = self.ns):
+            street = self.lxmlGetAttribValue(addressEl, "street")
+            city = " ".join(
+                [
+                    self.lxmlGetAttribValue(addressEl, "place") , 
+                    self.lxmlGetAttribValue(addressEl, "city")
+                ]
+            )            
+            country_subdivision = self.lxmlGetAttribValue(addressEl, "region")
+            country_ori = self.lxmlGetAttribValue(addressEl, "countryDescription")
+            country_ori = self.stripAdvance(country_ori).upper()
+            address = " ".join(
+                [
+                    street,
+                    city,
+                    country_subdivision,
+                    "" if country_ori == "UNKNOWN" else country_ori
+                ]
+            )
+            address = self.stripAdvance(address)
+            if len(address) > 0:
+                country_ISO_code = self.getISOCodeFromCountryName(country_ori)
+                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
+                addresses.append(
+                    {
+                        "address": address.upper(),
+                        "street": self.stripAdvance(street).upper(),
+                        "city": self.stripAdvance(city).upper(),
+                        "country_subdivision": self.stripAdvance(country_subdivision).upper(),
+                        "country_ori": country_ori,
+                        "country_ISO_code": country_ISO_code,
+                        "country_desc": country_desc
+                    }
+                )
+
+        return self.dedupDictsList(addresses)
+    
+    def getNationalities(self, listEntry):
+
+        nationalities = []
+
+        for nationalityEl in listEntry.findall("citizenship", namespaces = self.ns):
+            nationality_ori = self.lxmlGetAttribValue(nationalityEl, "countryDescription")
+            nationality_ori = self.stripAdvance(nationality_ori).upper()
+            if len(nationality_ori) > 0 and nationality_ori != "UNKNOWN":
+                country_ISO_code = self.getISOCodeFromCountryName(nationality_ori)
+                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
+                nationalities.append(
+                    {
+                        "country_ori": nationality_ori,
+                        "country_ISO_code": country_ISO_code,
+                        "country_desc": country_desc
+                    }
+                )
+
+        return self.dedupDictsList(nationalities)
+    
+    def getDatesOfBirth(self, listEntry):
+
+        datesOfBirth = []
+
+        for dobEl in listEntry.findall("birthdate", namespaces = self.ns):
+
+            yearIni = self.lxmlGetAttribValue(dobEl, "yearRangeFrom")
+            yearEnd = self.lxmlGetAttribValue(dobEl, "yearRangeTo")
+
+            if len(yearIni) > 0 and len(yearEnd) > 0:
+                for year in range(int(yearIni), int(yearEnd) + 1, 1):
+                    datesOfBirth.append(
+                        {
+                            "date_of_birth": "",
+                            "year": str(year),
+                            "month": "",
+                            "day": ""
+                        }
+                    )
+            else:
+                date_of_birth = self.lxmlGetAttribValue(dobEl, "birthdate")
+                monthOri = self.lxmlGetAttribValue(dobEl, "monthOfYear")
+                month = "{:02d}".format(int(monthOri)) if len(monthOri) > 0 else ""
+                dayOri = self.lxmlGetAttribValue(dobEl, "dayOfMonth")
+                day = "{:02d}".format(int(dayOri)) if len(dayOri) > 0 else ""
+                year = self.lxmlGetAttribValue(dobEl, "year")                
+
+                if len(date_of_birth) > 0 or \
+                   len(month) > 0  or \
+                   len(day) > 0 or \
+                   len(year) > 0:
+                    
+                    datesOfBirth.append(
+                        {
+                            "date_of_birth": date_of_birth,
+                            "year": year,
+                            "month": month,
+                            "day": day
+                        }
+                    )
+
+        return self.dedupDictsList(datesOfBirth)
+    
+    def getPlacesOfBirth(self, listEntry):
+
+        placesOfBirth = []
+
+        for pobEl in listEntry.findall("birthdate", namespaces = self.ns):
+            street = ""
+            city = " ".join(
+                [
+                    self.lxmlGetAttribValue(pobEl, "place"), 
+                    self.lxmlGetAttribValue(pobEl, "city")
+                ]
+            )
+            country_subdivision = self.lxmlGetAttribValue(pobEl, "region")            
+            country_ori = self.lxmlGetAttribValue(pobEl, "countryDescription")
+            country_ori = self.stripAdvance(country_ori).upper()
+            pob = " ".join(
+                    [
+                        street,
+                        city,
+                        country_subdivision,
+                        "" if country_ori == "UNKNOWN"  else country_ori
+                    ]
+                )               
+            pob = self.stripAdvance(pob)
+            if len(pob) > 0:
+                country_ISO_code = self.getISOCodeFromCountryName(country_ori)
+                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
+                placesOfBirth.append(
+                    {
+                        "place_of_birth": pob.upper(),
+                        "street": self.stripAdvance(street).upper(),
+                        "city": self.stripAdvance(city).upper(),
+                        "country_subdivision": self.stripAdvance(country_subdivision).upper(),
+                        "country_ori": country_ori,
+                        "country_ISO_code": country_ISO_code,
+                        "country_desc": country_desc
+                    }
+                )
+
+        return self.dedupDictsList(placesOfBirth)
+    
+    def getIdentifications(self, listEntry):
+
+        identifications = []
+
+        for IdEl in listEntry.findall("identification", namespaces = self.ns):
+            idNumber =  self.lxmlGetAttribValue(IdEl, "number")
+            if len(idNumber) > 0:
+                idType = self.lxmlGetAttribValue(IdEl, "identificationTypeDescription")
+                country_ori = self.lxmlGetAttribValue(IdEl, "countryDescription")
+                country_ori = self.stripAdvance(country_ori).upper()
+                country_ISO_code = self.getISOCodeFromCountryName(country_ori)
+                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
+                identifications.append(
+                    {
+                        "type": self.stripAdvance(idType).upper(),
+                        "id": idNumber,
+                        "country_ori": country_ori,
+                        "country_ISO_code": country_ISO_code,
+                        "country_desc": country_desc
+                    }
+                )
+
+        return self.dedupDictsList(identifications)
+    
+    def getPrograms(self, listEntry):
+         
+        regulationEl = listEntry.find("regulation", namespaces = self.ns)
+        if regulationEl is not None:
+            program = self.stripAdvance(
+                self.lxmlGetAttribValue(regulationEl, "programme")
+            )
+        else:
+            program = ""
+        if len(program) > 0:
+            return [program]
+        else:
+            return []
+        
+    def getAddtionalInformation(self, listEntry):
+
+        result = {}
+        
+        remarks = []
+        for remarkEL in listEntry.findall("remark", namespaces = self.ns):
+            if remarkEL is not None:
+                remarks.append(remarkEL.text)
+
+        remark = " ".join(remarks)
+        remark = self.stripAdvance(remark)
+        
+        if len(remark) > 0:
+            result["remarks"] = remark
+
+        return result
+    
+class LoaderUNXML(LoaderXML):
+    
+    def load(self, data_source):
+        super().load(data_source)
+        self.listEntryPath = ""
+        self.meta["list_date"] = self.lxmlGetAttribValue(self.data, "dateGenerated")
+        
+        listEntries = []
+        listEntryPaths = [
+            ".//INDIVIDUALS/INDIVIDUAL",
+            ".//ENTITIES/ENTITY"
+        ]
+        for listEntryPath in listEntryPaths:
+            self.listEntryPath = listEntryPath
+            for listEntry in self.data.findall(
+                listEntryPath,
+                namespaces=self.ns):
+                listEntries.append(self.loadListEntry(listEntry))
+
+        return {
+            "meta": self.meta,
+            "list_entries": listEntries
+        }
+    
+    def getId(self, listEntry):
+        return self.lxmlFindText(listEntry, "REFERENCE_NUMBER", self.ns)
+    
+    def getType(self, listEntry):
+        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
+            return "I"
+        elif self.listEntryPath == ".//ENTITIES/ENTITY":
+            return "O"
+        else:
+            return "U"
+        
+    def getNames(self, listEntry):
+        
+        names = []
+
+        entityType = self.getType(listEntry)
+        
+        # Main Name        
+
+        first_nameUN = self.lxmlFindText(listEntry, "FIRST_NAME", self.ns)
+        second_nameUN = self.lxmlFindText(listEntry, "SECOND_NAME", self.ns)
+        third_nameUN = self.lxmlFindText(listEntry, "THIRD_NAME", self.ns)
+        fourth_nameUN = self.lxmlFindText(listEntry, "FOURTH_NAME", self.ns)
+
+        if entityType == "I":
+            whole_name = " ".join(
+                [
+                    first_nameUN, 
+                    second_nameUN, 
+                    third_nameUN, 
+                    fourth_nameUN
+                ]
+            )            
+            names.append(
+                {
+                    "whole_name": self.stripAdvance(whole_name).upper(),
+                    "strong": True, 
+                    "first_name": "", 
+                    "last_name": ""
+                }
+            )
+        else:
+            names.append(
+                {
+                    "whole_name": self.stripAdvance(first_nameUN).upper(),
+                    "strong": True, 
+                    "first_name": "", 
+                    "last_name": ""
+                }
+            )
+
+        # Main Name Original Script
+        
+        name_original_script = self.lxmlFindText(listEntry, "NAME_ORIGINAL_SCRIPT", self.ns)
+        if len(name_original_script) > 0:
+            names.append(
+                {
+                    "whole_name": self.stripAdvance(name_original_script).upper(),
+                    "strong": True, 
+                    "first_name": "", 
+                    "last_name": ""
+                }
+            )
+
+        # Aliases
+
+        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
+            aliasesPath = "INDIVIDUAL_ALIAS"
+        else:
+            aliasesPath = "ENTITY_ALIAS"
+
+        for alias in listEntry.findall(aliasesPath, namespaces=self.ns):            
+            aliasName = self.lxmlFindText(alias, "ALIAS_NAME", self.ns)
+            aliasName = self.stripAdvance(aliasName)
+            if len(aliasName) > 0:
+                quality = self.lxmlFindText(alias, "QUALITY", self.ns)
+                strong = False if quality == "Low" else True                
+                names.append(
+                    {
+                        "whole_name": aliasName.upper(),
+                        "strong": strong, 
+                        "first_name": "", 
+                        "last_name": ""
+                    }
+                )
+
+        return self.dedupDictsList(names)
+    
+    def getAddresses(self, listEntry):
+
+        addresses = []
+
+        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
+            addressesPath = "INDIVIDUAL_ADDRESS"
+        else:
+            addressesPath = "ENTITY_ADDRESS"
+
+        for address in listEntry.findall(addressesPath, namespaces = self.ns):
+            street = self.lxmlFindText(address, "STREET", self.ns)
+            city = self.lxmlFindText(address, "CITY", self.ns)
+            country_subdivision = self.lxmlFindText(address, "STATE_PROVINCE", self.ns)
+            country_ori =  self.lxmlFindText(address, "COUNTRY", self.ns)
+            country_ori = self.stripAdvance(country_ori).upper()
+            address = " ".join(
+                [
+                    street,
+                    city,
+                    country_subdivision,
+                    country_ori   
+                ]
+            )
+            address = self.stripAdvance(address)
+            if len(address) > 0:
+                country_ISO_code = self.getISOCodeFromCountryName(country_ori)
+                country_desc = self.getCountryNameFromISOCode(country_ISO_code)
+                addresses.append(
+                    {
+                        "address": address.upper(),
+                        "street": self.stripAdvance(street).upper(),
+                        "city": self.stripAdvance(city).upper(),
+                        "country_subdivision": self.stripAdvance(country_subdivision).upper(),
+                        "country_ori": country_ori,
+                        "country_ISO_code": country_ISO_code,
+                        "country_desc": country_desc
+                    }
+                )
+        return self.dedupDictsList(addresses)
+    
+    def getNationalities(self, listEntry):
+
+        nationalities = []
+
+        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
+            for nationalityEl in listEntry.findall("NATIONALITY/VALUE", namespaces = self.ns):
+                if nationalityEl.text is not None:
+                    nationality_ori = nationalityEl.text 
+                    nationality_ori = self.stripAdvance(nationality_ori).upper()
+                else:
+                    nationality_ori = ""
+                if len(nationality_ori) > 0:
+                    country_ISO_code = self.getISOCodeFromCountryName(nationality_ori)
+                    country_desc = self.getCountryNameFromISOCode(country_ISO_code)
+                    nationalities.append(
+                         {
+                            "country_ori": nationality_ori,
+                            "country_ISO_code": country_ISO_code,
+                            "country_desc": country_desc
+                        }
+                    )
+
+        return self.dedupDictsList(nationalities)
+
+    def getDatesOfBirth(self, listEntry):
+
+        datesOfBirth = []
+
+        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
+            for dobEl in listEntry.findall("INDIVIDUAL_DATE_OF_BIRTH", namespaces = self.ns):
+
+                yearIni = self.lxmlFindText(dobEl, "FROM_YEAR", self.ns)
+                yearEnd = self.lxmlFindText(dobEl, "TO_YEAR", self.ns)
+
+                if len(yearIni) > 0 and len(yearEnd) > 0:
+
+                    for year in range(int(yearIni), int(yearEnd) + 1, 1):
+                        datesOfBirth.append(
+                            {
+                                "date_of_birth": "",
+                                "year": str(year),
+                                "month": "",
+                                "day": ""
+                            }
+                        )
+
+                else:
+
+                    date_of_birth = self.lxmlFindText(dobEl, "DATE", self.ns)
+                    if len(date_of_birth) > 0:
+                        date_of_birthParts = date_of_birth.split("-")
+                        day = date_of_birthParts[2]
+                        month = date_of_birthParts[1]
+                        year = date_of_birthParts[0]
+                    else:
+                        day = ""
+                        month = ""
+                        year = self.lxmlFindText(dobEl, "YEAR", self.ns)
+                    if len(date_of_birth) > 0 or \
+                       len(day) > 0 or \
+                       len(month) > 0 or \
+                       len(year) > 0:
+                        datesOfBirth.append(
+                            {
+                                "date_of_birth": date_of_birth,
+                                "year": year,
+                                "month": month,
+                                "day": day
+                            }
+                        )
+
+        return self.dedupDictsList(datesOfBirth)
+    
+    def getPlacesOfBirth(self, listEntry):
+
+        placesOfBirth = []
+
+        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
+
+            for pobEl in listEntry.findall("INDIVIDUAL_PLACE_OF_BIRTH", namespaces = self.ns):
+
+                street = self.lxmlFindText(pobEl, "STREET", self.ns)
+                city = self.lxmlFindText(pobEl, "CITY", self.ns)
+                country_subdivision = self.lxmlFindText(pobEl, "STATE_PROVINCE", self.ns)
+                country_ori = self.lxmlFindText(pobEl, "COUNTRY", self.ns)
+                country_ori = self.stripAdvance(country_ori).upper()
+                pob = " ".join(
+                    [
+                        street,
+                        city,
+                        country_subdivision,
+                        country_ori
+                    ]
+                )               
+                pob = self.stripAdvance(pob)
+                if len(pob) > 0:
+                    country_ISO_code = self.getISOCodeFromCountryName(country_ori)
+                    country_desc = self.getCountryNameFromISOCode(country_ISO_code)
+                    placesOfBirth.append(
+                        {
+                            "place_of_birth": pob.upper(),
+                            "street": self.stripAdvance(street).upper(),
+                            "city": self.stripAdvance(city).upper(),
+                            "country_subdivision": self.stripAdvance(country_subdivision).upper(),
+                            "country_ori": country_ori,
+                            "country_ISO_code": country_ISO_code,
+                            "country_desc": country_desc
+                        }
+                    )
+
+        return self.dedupDictsList(placesOfBirth)
+    
+    def getIdentifications(self, listEntry):
+
+        identifications = []
+
+        if self.listEntryPath == ".//INDIVIDUALS/INDIVIDUAL":
+
+            for IdEl in listEntry.findall("INDIVIDUAL_DOCUMENT", namespaces = self.ns):
+                idNumber = self.lxmlFindText(IdEl, "NUMBER", self.ns)
+                if len(idNumber) > 0:
+                    idType = self.lxmlFindText(IdEl, "TYPE_OF_DOCUMENT", self.ns)
+                    country1 = self.lxmlFindText(IdEl, "COUNTRY_OF_ISSUE", self.ns)
+                    country1 = self.stripAdvance(country1).upper()
+                    country2 = self.lxmlFindText(IdEl, "ISSUING_COUNTRY", self.ns)
+                    country2 = self.stripAdvance(country2).upper()
+                    if country1 == country2:
+                        country_ori = country1
+                    else:
+                        if len(country1) > 0:
+                            country_ori = country1
+                        else:
+                            country_ori = country2
+                    country_ISO_code = self.getISOCodeFromCountryName(country_ori)
+                    country_desc = self.getCountryNameFromISOCode(country_ISO_code)
+                    identifications.append(
+                        {
+                            "type": self.stripAdvance(idType).upper(),
+                            "id": idNumber,
+                            "country_ori": country_ori,
+                            "country_ISO_code": country_ISO_code,
+                            "country_desc": country_desc
+                        }
+                    )
+
+        return self.dedupDictsList(identifications)
+    
+    def getPrograms(self, listEntry):
+
+        listType = self.lxmlFindText(listEntry, "UN_LIST_TYPE", ns=self.ns)
+        listType = self.stripAdvance(listType)        
+        
+        if len(listType) > 0:
+            return [listType]
+        else:
+            return []
+        
+    def getAddtionalInformation(self, listEntry):
+
+        result = {}
+        
+        remarks = [self.lxmlFindText(listEntry, "COMMENTS1", ns=self.ns)]
+        for designationEl in listEntry.findall("DESIGNATION/VALUE", namespaces=self.ns):
+            if designationEl.text is not None:
+                remarks.append(designationEl.text)
+
+        remark = " ".join(remarks)
+        remark = self.stripAdvance(remark)
+
+        if len(remark) > 0:
+            result["remarks"] = remark
+
+        gender = self.lxmlFindText(listEntry, "GENDER", ns=self.ns)
+        gender = self.stripAdvance(gender)
+        if len(gender) > 0:                     
+            result["gender"] = gender
+        
+        return result
+    
+def load(data, loader=Loader, description=""):
     return loader(description).load(data)
```

### Comparing `inoutlists-0.0.2/tests/lists_mapper.py` & `inoutlists-1.0.0/tests/lists_mapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from pathlib import Path
-import os
-import context
-from inoutlists import load, LoaderOFACXML, LoaderEUXML, LoaderUNXML
-from inoutlists import dump, DumperJSON, DumperPandas, DumperCSV
-
-
-_modulePath = Path(os.path.realpath(__file__)).parent
-
-filesInfo = {
-    "OFACSDN": {
-        "input": {
-            "localPath": Path(_modulePath, "./.data/sdn.xml"),
-            "url": "https://sanctionslistservice.ofac.treas.gov/api/PublicationPreview/exports/SDN.XML",            
-            "loader": LoaderOFACXML
-        },
-        "output": {
-            "json": Path(_modulePath, "./.data/ofac_sdn.json"),
-            "csv": Path(_modulePath, "./.data/ofac_sdn.csv")
-        }
-    }   ,
-    "OFACCONS": {
-        "input": {
-            "localPath": Path(_modulePath, "./.data/consolidated.xml"),
-            "url": "https://sanctionslistservice.ofac.treas.gov/api/PublicationPreview/exports/CONSOLIDATED.XML",
-            "loader": LoaderOFACXML
-        },
-        "output": {
-            "json": Path(_modulePath, "./.data/ofac_consolidated.json"),
-            "csv": Path(_modulePath, "./.data/ofac_consolidated.csv")
-        }
-    },
-    "EU": {
-        "input": {            
-            "localPath": Path(_modulePath, "./.data/20240513-FULL-1_1(xsd).xml"),
-            "url": "https://webgate.ec.europa.eu/fsd/fsf/public/files/xmlFullSanctionsList_1_1/content?token=dG9rZW4tMjAxNw",                    
-            "loader": LoaderEUXML
-        },
-        "output": {
-            "json": Path(_modulePath, "./.data/eu.json"),
-            "csv": Path(_modulePath, "./.data/eu.csv")
-        }
-    },
-    "UN": {
-        "input": {
-            "localPath": Path(_modulePath, "./.data/un_consolidated.xml"),
-            "url": "https://scsanctions.un.org/resources/xml/en/consolidated.xml",
-            "loader": LoaderUNXML
-        },
-        "output": {
-            "json": Path(_modulePath, "./.data/un.json"),
-            "csv": Path(_modulePath, "./.data/un.csv")
-        }
-    }
-}
-
-lists = {}
-dfs = {}
-
-for description, sourceInfo in filesInfo.items():
-    if description in ["EU", "OFACSDN", "OFACCONS", "UN"]:
-        list = load(
-            #sourceInfo["input"]["localPath"],
-            sourceInfo["input"]["url"],
-            sourceInfo["input"]["loader"],
-            description
-        )     
-        lists[description] = list
-        fileJSON = sourceInfo["output"]["json"]        
-        dump(
-            list, 
-            DumperJSON, 
-            file=fileJSON, 
-            indent=2, 
-            ensure_ascii=False
-        )
-        dfs[description] = dump(list, DumperPandas)
-        fileCSV = sourceInfo["output"]["csv"]
-        dump(
-            list, 
-            DumperCSV, 
-            output=fileCSV, 
-            index=False, 
-            sep="\t", 
-            lineterminator = "\n"
-        )
-
-    else:
+from pathlib import Path
+import os
+import context
+from inoutlists import load, LoaderOFACXML, LoaderEUXML, LoaderUNXML
+from inoutlists import dump, DumperJSON, DumperPandas, DumperCSV
+
+
+_modulePath = Path(os.path.realpath(__file__)).parent
+
+filesInfo = {
+    "OFACSDN": {
+        "input": {
+            "localPath": Path(_modulePath, "./.data/sdn.xml"),
+            "url": "https://sanctionslistservice.ofac.treas.gov/api/PublicationPreview/exports/SDN.XML",            
+            "loader": LoaderOFACXML
+        },
+        "output": {
+            "json": Path(_modulePath, "./.data/ofac_sdn.json"),
+            "csv": Path(_modulePath, "./.data/ofac_sdn.csv")
+        }
+    }   ,
+    "OFACCONS": {
+        "input": {
+            "localPath": Path(_modulePath, "./.data/consolidated.xml"),
+            "url": "https://sanctionslistservice.ofac.treas.gov/api/PublicationPreview/exports/CONSOLIDATED.XML",
+            "loader": LoaderOFACXML
+        },
+        "output": {
+            "json": Path(_modulePath, "./.data/ofac_consolidated.json"),
+            "csv": Path(_modulePath, "./.data/ofac_consolidated.csv")
+        }
+    },
+    "EU": {
+        "input": {            
+            "localPath": Path(_modulePath, "./.data/20240513-FULL-1_1(xsd).xml"),
+            "url": "https://webgate.ec.europa.eu/fsd/fsf/public/files/xmlFullSanctionsList_1_1/content?token=dG9rZW4tMjAxNw",                    
+            "loader": LoaderEUXML
+        },
+        "output": {
+            "json": Path(_modulePath, "./.data/eu.json"),
+            "csv": Path(_modulePath, "./.data/eu.csv")
+        }
+    },
+    "UN": {
+        "input": {
+            "localPath": Path(_modulePath, "./.data/un_consolidated.xml"),
+            "url": "https://scsanctions.un.org/resources/xml/en/consolidated.xml",
+            "loader": LoaderUNXML
+        },
+        "output": {
+            "json": Path(_modulePath, "./.data/un.json"),
+            "csv": Path(_modulePath, "./.data/un.csv")
+        }
+    }
+}
+
+lists = {}
+dfs = {}
+
+for description, sourceInfo in filesInfo.items():
+    if description in ["EU", "OFACSDN", "OFACCONS", "UN"]:
+        list = load(
+            #sourceInfo["input"]["localPath"],
+            sourceInfo["input"]["url"],
+            sourceInfo["input"]["loader"],
+            description
+        )     
+        lists[description] = list
+        fileJSON = sourceInfo["output"]["json"]        
+        dump(
+            list, 
+            DumperJSON, 
+            output=fileJSON, 
+            indent=2, 
+            ensure_ascii=False
+        )
+        dfs[description] = dump(list, DumperPandas)
+        fileCSV = sourceInfo["output"]["csv"]
+        dump(
+            list, 
+            DumperCSV, 
+            output=fileCSV, 
+            index=False, 
+            sep="\t", 
+            lineterminator = "\n"
+        )
+
+    else:
         print(f"Unknown description: {description}. Only allowed EU, OFACSDN and OFACCONS")
```

### Comparing `inoutlists-0.0.2/LICENSE` & `inoutlists-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Eusebio José de la Torre Niño
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2024 Eusebio José de la Torre Niño
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

