# Version 0.2

Version 0.2 is the second alpha release.
It focuses on institutions and province development system.

----

## New Features

- Integrated **Eurocentric Institutions** mod that makes the institution system heavily favor European countries.[^1]
- Free leaders are now granted proportional to land and naval force limit.[^2]

----

## Game Balance

### Development

- Development now decreases Supply Limit Modifier by -0.01 <sup>(0.02)</sup> per development level.[^3]
- Development now increases Local Monthly Autonomy by 0.006 per development level.[^4]
- Development no longer increases Local Trade Power per development level.[^5]

#### Base Tax

- *Base Tax* development is now called *Local Commerce* and has a new icon.

- <details>
	  <summary>Changed provincial modifiers per Base Tax development level.</summary>
	  <ul>
		  <li><code><s>Local Recruitment Time: -1.0%</s></code></li>
		  <li><code>Local Trade Power: +0.60</code></li>
		  <li><code>State Maintenance: +0.4%</code></li>
		  <li><code>Trade Value: +0.10</code></li>
		  <li><code>Institution Spread: +1.0%</code></li>
	  </ul>
  </details>

#### Base Production

- *Base Production* is now called *Local Production* and has a new icon.

- <details>
	  <summary>Changed provincial modifiers per Base Production development level.</summary>
	<ul>
		  <li><code>Manpower Increase: +100</code></li>
		  <li><code>Local Construction Time: -1.5%</code></li>
		  <li><code>Local Shipbuilding Time: -1.5% <sup>(-1.0%)</sup></code></li>
		  <li><code>Local Ship Repair: +1.5%</code></li>
		  <li><code>Supply Limit Modifier: +10.0%</code></li>
	  </ul>
  </details>

#### Base Manpower

- *Base Manpower* is now called *Local Militia* and has a new icon.

- <details>
	  <summary>Changed provincial modifiers per Base Manpower development level.</summary>
	  <ul>
		  <li><code>Local Unrest: -0.20</code></li>
		  <li><code>Local Recruitment Time: -1.5%</code></li>
		  <li><code>Garrison Growth: +3.0% <sup>(+1.0%)</sup></code></li>
		  <li><code>Local Defensiveness: +1.3%</code></li>
		  <li><code>Monthly Autonomy Change: -0.03</code></li>
	  </ul>
  </details>

### Economy

- Cost of raising war taxes is now 35 <sup>(50)</sup> administrative power.

- Local unrest now decreases local tax modifier by 2% per 1 unrest.

- <details>
	  <summary>Changed war exhaustion static modifiers.</summary>
	  <ul>
		  <li><code>Recruitment Speed: +3.0% <sup>(+2.0%)</sup></code></li>
		  <li><code>Shipbuilding Time: +3.0% <sup>(+2.0%)</sup></code></li>
		  <li><code>War Taxes Cost: 50.0%</code></li>
		  <li><code>Institution Spread: -4.0%</code></li>
		  <li><code>Manpower Recovery Speed: -2.5% <sup>(-1.0%)</sup></code></li>
		  <li><code>Sailor Recovery Speed: -2.5% <sup>(-1.0%)</sup></code></li>
		  <li><code>Morale of Armies: -1.0%</code></li>
		  <li><code>Army Drill Gain Modifier: -4.0%</code></li>
	  </ul>
  </details>

#### War Taxes

- War taxes no longer increase possible mercenaries pool.
- War taxes now increase war exhaustion by 0.06.<sup>(0.065)</sup>
- High war taxes<span title="WE >= 5 & WE < 10"><sup>?</sup></span> now increases national unrest by 2.5 and war exhaustion by 0.04.
- Very high war taxes<span title="WE >= 10"><sup>?</sup></span> now increases national unrest by 5 and war exhaustion by 0.08.

#### Stability

- Stability now affects monthly autonomy change by 0.05 per stability level.[^6]
- Positive stability now affects yearly corruption by -0.05 <sup>(-0.02)</sup> per stability level.
- Negative stability now affects yearly corruption by 0.05 per stability level.

### Autonomy

- Every country now has a base autonomy change rate of 0.03.[^7]
- Kingdom and Empire government ranks now decrease autonomy by -0.05 <sup>(-0.025)</sup> and -0.1 <sup>(-0.05)</sup> respectively.
- **Self Governance** modifiers are now incremented by 100 <sup>(50)</sup> to a maximum of 1000 distance units with minimum local autonomy scaling from 5 to 75 and local autonomy change scaling from 0.05 to 0.25.
- **Administrative Center** province modifier now decreases minimum local autonomy by -15.<sup>(-10)</sup>
- **State Jurisdiction** province modifier now decreases minimum local autonomy by -10.<sup>(-5)</sup>

### Advisors

- **Commandant** now increases discipline by 5% <sup>(4%)</sup>  and army drill gain by 20%.<sup>(25%)</sup>

### Terrain

- <details>
	  <summary>Winter terrain modifiers now increases development cost and decreases unit movement speed.</summary>
	  <ul><br>
		  <li><b>Mild Winter</b></li>
		  <ul>
			  <li><code>Local Development Cost: +3.0%</code></li>
			  <li><code>Friendly Movement Speed: -20.0%</code></li>
			  <li><code>Hostile Movement Speed: -20.0%</code></li>
		  </ul><br>
		  <li><b>Normal Winter</b></li>
		  <ul>
			  <li><code>Local Development Cost: +5.0%</code></li>
			  <li><code>Friendly Movement Speed: -25.0%</code></li>
			  <li><code>Hostile Movement Speed: -25.0%</code></li>
		  </ul><br>
		  <li><b>Severe Winter</b></li>
		  <ul>
			  <li><code>Local Development Cost: +10.0%</code></li>
			  <li><code>Friendly Movement Speed: -50.0%</code></li>
			  <li><code>Hostile Movement Speed: -50.0%</code></li>
		  </ul>
	  </ul>
  </details>

### Military

- <span title="Army Professionalism >= 20%">Salaried Soldiers<sup>?</sup></span> from army professionalism now also increases manpower recovery speed by 10%.
- Countries can now maintain up to 1 <sup>(2)</sup> military leaders without incurring a penalty to military power.[^8]
- Military technology level 1 and 3 now grant 25% increase in flanking range.[^9]

#### Army Drill

- Reverted yearly army drill gain for regiments to vanilla value: 10.<sup>(12)</sup>
- Army drill now increases unit movement speed by 25%<span title="Scaled value"><sup>↗️</sup></span><sup>(20%)</sup> for armies drilled at 100%.
- Army drill now increases discipline by 5%<span title="Scaled value"><sup>↗️</sup></span> for regiments drilled at 100%.

### Institutions

-  Institution gain from manually developing provinces is now 2.<sup>(5)</sup>

#### Feudalism

- Maximum technology penalty for not embracing institution is now 80%.<sup>(50%)</sup>
- Reduced institution spread factor for Steppe Nomad, Siberian Clan Council, and Native Council governments by 0.2.

#### Renaissance

- Before 1550, only provinces on the continent of Europe, provinces belonging to countries with a European capital, or provinces in the Near East, Egypt, Persia, East Africa and Maghreb regions may gain this institution.
- Institution spread from nearby friendly provinces and adjacent provinces reduced by half.
- Institution will now never spread to provinces owned by Tribal, Siberian and Native Council governments.

#### Colonialism

- Institution will now always spawn in a European province.
- Reduced institution spread factor in the Near East, Egypt and Maghreb regions by 1.0.[^10]
- Institution will now never spread to provinces owned by Tribal governments, including Siberian and Native Councils.

#### Printing Press

- Institution will never spread to Confucian or Shinto provinces owned by Chinese tech group countries[^11] with one exception being *"Kirishitan Realm"* countries.[^12]
- Institution will now never spread to countries within Central African, North American, South American, or Andean tech group.[^13]

#### Global Trade

- Institution will now always spawn in a European province owned by a country within a Western tech group that has at least one province in a Trade Company.[^14]
- Institution will now never spread to provinces owned by Tribal governments, including Siberian and Native Councils.

#### Manufactories

- Institution will now always spawn in a European province.
- Institution can now start in a province that has a Farm Estate manufactory.
- Reduced institution spread factor in countries within Muslim and East African tech group by 0.35.[^15]
- Reduced institution spread factor in countries within Indian tech group by 0.65.[^15]
- Reduced institution spread factor in Shinto provinces owned by countries within Chinese tech group by 0.65.[^15]
- Reduced institution spread factor in non-Shinto provinces owned by countries within Chinese tech group by 1.35.[^16]
- Institution will now never spread to provinces owned by country within West African, Central African, Mesoamerican, Andean, North American, or South American tech group.
- Institution will now never spread to provinces owned by Tribal governments, including Siberian and Native Councils.

#### Enlightenment

- Institution will now always spawn in a European province.
- Maximum technology penalty for not embracing institution is now 100%.<sup>(50%)</sup>
- Institution will now never spread to provinces owned by Tribal governments, including Siberian and Native Councils.

### Estates

#### Burghers

- Provinces granted to Burghers now have minimum local autonomy reduced by -15.[^17]

- Employing Trader advisor now increases estate influence by 5.

- <details>
	  <summary>Changed Burghers nationwide modifiers.</summary><br>
	<ul>
		<li>
			<details>
				<summary>Modifiers when estate is <span style="color:green">loyal</span>:</summary><br>
				<ul>
					<li><b>National modifiers:</b></li>
					<ul>
						<li><code><s>Production Efficiency: +10.0%</s></code></li>
						<li><code>National Tax Modifier: +10.0%</code></li>
					</ul><br>
					<li><b>Province modifiers:</b></li>
					<ul>
						<li><code>Minimum Local Autonomy: -15.0</code></li>
						<li><code><s>Local Goods Produced Modifier: +15.0%</s></code></li>
						<li><code>Trade Value Modifier: +15.0%</code></li>
						  <li><code>Local Development Cost: -5.0%</code></li>
						<li><code>Local Trade Power: +60.0% <sup>(+70.0%)</sup></code></li>
						  <li><code>Local Construction Cost: -20.0% <sup>(-25.0%)</sup></code></li>
				</ul><br>
			</details>
		</li>
		<li>
			<details>
				  <summary>Modifiers when estate is <span style="color:yellow">neutral</span>:</summary><br>
				<ul>
					<li><b>National modifiers:</b></li>
					<ul>
						<li><code><s>Production Efficiency: +5.0%</s></code></li>
						<li><code>National Tax Modifier: +5.0%</code></li>
					</ul><br>
					<li><b>Province modifiers:</b></li>
					<ul>
						<li><code>Minimum Local Autonomy: -15.0</code></li>
						<li><code><s>Local Goods Produced Modifier: +10.0%</s></code></li>
						<li><code>Trade Value Modifier: +10.0%</code></li>
					</ul>
				</ul><br>
			</details>
		</li>
		<li>
			<details>
				<summary>Modifiers when estate is <span style="color:red">disloyal</span>:</summary><br>
				<ul>
					<li><b>National modifiers:</b></li>
					<ul>
						  <li><code>Local Development Cost: +20.0% <sup>(+15.0%)</sup></code></li>
						  <li><code>Yearly Corruption: +0.32% <sup>(+0.10)</sup></code></li>
					</ul><br>
					<li><b>Province modifiers:</b></li>
					<ul>
						<li><code>Minimum Local Autonomy: -15.0</code></li>
							<li><code>Local Construction Time: +20.0% <sup>(+30.0%)</sup></code></li>
						  <li><code><s>Local Construction Cost: +30.0%</s></code></li>
						  <li><code><s>Local Shipbuilding Time: +30.0%</s></code></li>
							<li><code>Local Unrest: +5.0 <sup>(+4.0)</sup></code></li>
					</ul>
				</ul><br>
			</details>
		</li>
	</ul>
  </details>

#### Clergy

- Provinces granted to Burghers now have minimum local autonomy reduced by -15.[^17]

- Employing Inquisitor or Theologian advisor now increases estate influence by 5.

- <details>
	  <summary>Changed Clergy nationwide modifiers.</summary><br>
	<ul>
		<li>
			<details>
				<summary>Modifiers when estate is <span style="color:green">loyal</span>:</summary><br>
				<ul>
					<li><b>Province modifiers:</b></li>
					<ul>
						  <li><code>Minimum Local Autonomy: -15.0</code></li>
						<li><code>Local Tax Modifier: +10.0% <sup>(+15.0%)</sup></code></li>
						<li><code>Local Unrest: -4.0 <sup>(-3.5)</sup></code></li>
						<li><code>Resistance to Reformation: +40.0%</code></li>
				</ul><br>
			</details>
		</li>
		<li>
			<details>
				  <summary>Modifiers when estate is <span style="color:yellow">neutral</span>:</summary><br>
				<ul>
					<li><b>Province modifiers:</b></li>
					<ul>
						<li><code>Minimum Local Autonomy: -15.0</code></li>
						<li><code><s>Local Tax Modifier: +10.0%</s></code></li>
						<li><code>Resistance to Reformation: +20.0%</code></li>
					</ul>
				</ul><br>
			</details>
		</li>
		<li>
			<details>
				<summary>Modifiers when estate is <span style="color:red">disloyal</span>:</summary><br>
				<ul>
					<li><b>National modifiers:</b></li>
					<ul>
						  <li><code>Yearly Corruption: +0.1 <sup>(0.2)</sup></code></li>
					</ul><br>
					<li><b>Province modifiers:</b></li>
					<ul>
						  <li><code>Minimum Local Autonomy: -15.0</code></li>
						<li><code><s>Institution Spread: -20.0%</s></code></li>
						<li><code>Local Missionary Maintenance: +20.0%</code></li>
						  <li><code>Local Unrest: +5.0 <sup>(+7.0)</sup></code></li>
					</ul>
				</ul><br>
			</details>
		</li>
	</ul>
  </details>

#### Nobility

- Provinces granted to Burghers now have minimum local autonomy reduced by -15.[^17]

- Employing Grand Captain advisor now increases estate influence by 5.

- <details>
	  <summary>Changed Burghers nationwide modifiers.</summary><br>
	<ul>
		<li>
			<details>
				<summary>Modifiers when estate is <span style="color:green">loyal</span>:</summary><br>
				<ul>
					<li><b>National modifiers:</b></li>
					<ul>
						<li><code>Monthly Heir Support Gain: +33.0%</code></li>
					</ul><br>
					<li><b>Province modifiers:</b></li>
					<ul>
						<li><code>Minimum Local Autonomy: -15.0</code></li>
						<li><code>Local Manpower Modifier: 20.0% <sup>(25.0%)</sup></code></li>
						  <li><code><s>Local Regiment Cost: -25.0%</s></code></li>
						  <li><code>Garrison Growth: +25.0% <sup>(+10.0%)</sup></code></li>
				</ul><br>
			</details>
		</li>
		<li>
			<details>
				  <summary>Modifiers when estate is <span style="color:yellow">neutral</span>:</summary><br>
				<ul>
					<li><b>Province modifiers:</b></li>
					<ul>
						<li><code>Minimum Local Autonomy: -15.0</code></li>
						<li><code>Local Manpower Modifier: +10.0% <sup>(+15.0%)</sup></code></li>
						<li><code><s>Local Recruitment Time: -15.0%</s></code></li>
					</ul>
				</ul><br>
			</details>
		</li>
		<li>
			<details>
				<summary>Modifiers when estate is <span style="color:red">disloyal</span>:</summary><br>
				<ul>
					<li><b>National modifiers:</b></li>
					<ul>
						  <li><code>Yearly Corruption: +0.16 <sup>(+0.10)</sup></code></li>
					</ul><br>
					<li><b>Province modifiers:</b></li>
					<ul>
						  <li><code>Minimum Local Autonomy: -15.0</code></li>
						<li><code><s>Local Manpower Modifier: -30.0%</s></code></li>
						  <li><code><s>Local Regiment Cost: +30.0%</s></code></li>
						  <li><code>Local Recruitment Time: +20.0%</code></li>
					</ul>
				</ul><br>
			</details>
		</li>
	</ul>
  </details>

### Buildings

- **Courthouse** now costs 150 <sup>(100)</sup> ducats.
- **Town Hall** now costs 250 <sup>(200)</sup> ducats.

----

## Script

### AI

- AI will now consider building administrative buildings based on state distance from capital.[^18]
- Development cap base for AI logic is now 15 <sup>(10)</sup> which will make AI develop more.
- Bonus to *war readiness* gained from drilled regiments is now 0.10.<sup>(0.08)</sup> [^19]

#### War Exhaustion

- AI now has reduced war exhaustion cost by 33%.
- Disabled war taxes for AI countries with medium<span title="War exhaustion >= 7"><sup>?</sup></span> war exhaustion.

### Decisions

- <details>
  <summary>Slightly decreased effects of <i>Elite Regiments</i> event modifier.</summary>
  <ul>
	<li><code>Yearly Army Drill Gain: +40.0% <sup>(+50.0%)</sup></code>
	  <li><code>Global Regiment Recruitment Speed: +40.0% <sup>(+50.0%)</sup></code></li>
  </ul>
  </details>

### Events

- *Crisis of the Maghreb* event now lasts for 50 <sup>(5)</sup> years.[^20]
- <details>
	  <summary>Changed <i>Crisis of the Maghreb</i> event modifier effects.</summary>
	  <ul>
		  <li><code>Global Trade Power: -5.0% <sup>(-2.5%)</sup></code></li>
		  <li><code>Stability Cost Modifier: +10.0% <sup>(+5.0%)</sup></code></li>
		  <li><code>Institution Spread: -5.0% <sup>(-2.5%)</sup></code></li>
		<li><code>Technology Cost: +15.0%</code></li>
	  </ul>
  </details>
- *A Kirishitan Realm* event tooltip now informs the player that Printing Press may now appear in their provinces.

----

[^1]: Integrated the [updated version](https://steamcommunity.com/sharedfiles/filedetails/?id=1881890980) (1.29) of the [original mod](https://steamcommunity.com/sharedfiles/filedetails/?id=1388492593) from the Steam Workshop.
[^2]: One additional free leader is granted for every 20 land and naval units that can be supported by force limit up to a maximum of 10 free leaders granted for 100/100 land/naval force limit. Read more information from issue [#49](https://github.com/yooksi/eu4-EVE/issues/49) in project repository.
[^3]: This represents the supply limit weight of local population.
[^4]: This represents the increasing demand for autonomy from population growth.
[^5]: This modifier was moved to Local Commerce development.
[^6]: This modifier will be negative when stability is negative and vice versa.
[^7]: This compensates for autonomy reduction from local militia at minimum development (3).
[^8]: Reverted back to vanilla value to accommodate for leaders from force limit change.
[^9]: This is an experimental change that attempts to improve the viability of cavalry in the early game since flanking has very limited functionality in combat. Learn more about cavalry viability: [Why they are bad and what would make them good](https://www.youtube.com/watch?v=h-62B7GiwDw).
[^10]: This is intended to balance the Berbers against the Iberians and represent traditional Near East trade routes being circumvented by European explorers.
[^11]: This is meant to represent the unpopularity of movable type in East Asian countries during this period due to logographic languages with thousands of characters, differences in ink technology, etc. The impact of Printing Press in East Asia was not the same as in the rest of  the world.
[^12]: In the 1590s, Jesuit missionaries introduced the Gutenberg press to Japan, and used it to print religious texts in a romanized form of Japanese. If you are playing a Shinto country and choose "A Kirishitan Realm" result of the Spread of Christianity incident, Printing Press will spread in your provinces. The country does not have to actually convert to Christianity, they just have to choose the most Open result of that incident which involves protecting and patronizing missionaries.
[^13]: Illiterate cultures would have no use for printing press technology.
[^14]: For owners of "Wealth of Nations" or "Dharma" the province has to be part of a trade company, otherwise it just has to be located in a trade company region.
[^15]: Passive spread is no longer enough to spread this institution, provinces now must have a manufactory before it can spread.
[^16]: Passive spread is no longer enough to spread this institution, provinces now must have a manufactory and border a friendly province with Manufactories institution embraced before it can spread.
[^17]: This will greatly benefit distant provinces and the rationale for this is that provinces in distant lands granted to estates were granted with expectations that the government would see more control exerted over those provinces. Note that only autonomy above the minimum value imposed by estates will be reduced because autonomy cannot go lower then the base min autonomy defined in estate files regardless of the modifiers applied to the province.
[^18]: *"State distance from capital"* is a calculated average distance of all provinces in that state from the nation's capital province. For example, if province A, B and C were part of state D and they had the following distances from capital: 100, 200 and 150 respectively, then the state distance from capital would be 150 `((100 + 200 + 150) / 3)`.
[^19]: This should make AI more likely to wage war when having drilled regiments.
[^20]: This makes it an actual crisis, and increases chances that the Iberians survive.