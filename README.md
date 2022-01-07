# Vaja-6-ADC-scan-mode-conversion-Nucleo

Določila in aktivirala tri analogne vhode za kanale IN1, IN2 in IN3 za zunanje potenciometre kot Single-ended vhod. To bodo pini PC0,PC1 in PC2. Izbrani pini so v grupi C. Poleg pinov se izpiše ADC_IN1, ADC_IN2 in ADC_IN3.V Parameter settings izbereva ločljivost pretvorbe na 8-bitno, torej je območje vrednosti od 0 ÷ 255. Clock Prescaler nastaviva tako, da bo izračunana frekvenca vzorčenja 4 MHz.Izbrana vrednost parametra bo 4. Privzeta vrednost paramtera Number of Conversions je pa 1. Čas vzorčenja Sampling Time izbereva 92.5 cikla.Čas vzorčenja v mikro sekundah je 26,153 μs. Enačba za izračun: tvz = (tvz_cik + 12) / ftakta_pretvorbe.
Dolžina podatka pretvorbe bo 1 Byte, zato ustrezno popravimo izbirno polje Data Width:byte. Kratica DMA pomeni Direct Memory Access, kar v Slovenščini pomeni direktni dostop do pomnilnika.


KOMENTAR NA DELOVANJE:
Projekt žal ne deluje tako kot bi moral in sicer bere vrednost samo iz enega od treh potrnciometrov, kar je razvidno tudi v zgoraj priloženem gradivu.
