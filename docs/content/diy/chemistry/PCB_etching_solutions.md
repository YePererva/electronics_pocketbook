# PCB etching solutions


!!! warning "Safety disclaimer" 
	Enlisted solutions are corrosive and appropriate PPE (personal protection equipment) such as googles and gloves should be used

!!! tip "General Suggestions"
	- Don't work with these solutions in metal containers, glass or plastic only
	- Some mixing speeds up the process and prevent deposition/precipitation on the surface of etched copper 
## Hydrogen Peroxide in acids

Prepare the solution that contains:

- 100 ml of 3% Hydrogen Peroxide (H₂O₂)
- 30 g of citric acid
- 5 g of kitchen (table) salt

Don't store nor reuse this solution, and don't heat above 45 °C


??? note "Chemistry behind the process"
	
	$$
	\ce{Cu + H2O2 + H3[Cit] -> H[CuCit] + H2O}
	$$
	
	where, $\ce{Cit}$ is short for _citrate_ $\ce{[(CH2)2C(OH)(COO)3]^3-}$. 

## Ferric Chloride

Can be prepared from dry chemical by mixing with water in 1:3 ratio. Dissolving process is very self-heating. 

Also available on market as:

- 30-60% solution RadioShack PCB Etchant Solution [MSDS](https://cdn.shopify.com/s/files/1/2082/9857/files/SDS-E-2761535_v30.pdf)  
- 37-42% solution MG Chemicals 415 [MSDS](https://mgchemicals.com/downloads/msds/01%20English%20UK%20SDS/sds-415-l%20en%20uk.pdf)
- 25-50% solution C.I.F. AR412 [MSDS](https://www.farnell.com/datasheets/3210222.pdf)

The etching process can be speed-up if solution is warmed-up, but not above 50°C.

??? note "Chemistry behind the process"
	$$
	\ce{2FeCl3 + Cu -> 2FeCl2 + CuCl2 }
	$$
	
	$$
	\ce{Cu -> Cu^2+ + 2e^-}
	$$
	
	$$
	\ce{Fe^3+ + e-  -> Fe^2+}
	$$


## Persulfates (Persulphates)

There are available:

- Sodium Persulfate Na₂S₂O₈
- Ammonium Persulphate (NH₄)₂S₂O₈

Chemical reaction and mechanism is the same, but working concentration are different. 

??? note "Chemistry behind the process"
	$$
	\ce{Cu + S2O8^2- -> Cu^2+ + 2 SO4^2-}
	$$

!!! example "Storage" 
	Persulfate solutions should not be stored not places in air-tight containers 

### Ammonium Persulphate 

Dissolve 10 g of Ammonium Persulfate in 90 ml of water. For faster etching, the solution can be heat-up to 45-50 °C.

Crystaline powder is available on market as:

- MG Chemicals 410 [MSDS](https://mgchemicals.com/downloads/msds/01%20English%20UK%20SDS/sds-410%20en%20uk.pdf)
- C.I.F. AR44 [MSDS](https://www.farnell.com/datasheets/3210223.pdf)

### Sodium Persulphate

Recipe is referring to [Sodium persulfate B327](https://termopasty.com/en/products/sodium-persulfate-b327) instructions from [AG TermoPasty](https://termopasty.com/) 

Dissolve 50 g of Sodium persulfate in 250 ml of water at ~40...50°C.

## Nice to take a look at

- Nice demonstration and visual comparison [published](https://www.youtube.com/watch?v=Q4tWEse2rDI) by NurdRage on YouTube 