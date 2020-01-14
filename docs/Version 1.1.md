# Version 1.1

Version 1.1 aka "Lex Terrae" is the initial mod release version.

***

## Contents

* [New Features](#new-features)
* [Game Balance](#game-balance)
   * [Economy](#economy)
      * [Capital](#capital)
      * [Development](#development)
   * [Diplomacy](#diplomacy)
   * [Buildings](#buildings)
      * [Administrative](#administrative)
   * [Advisors](#advisors)
   * [Military](#military) 
      * [Army Professionalism](#army-professionalism)
      * [Army Drilling](#army-drilling)
      * [Power Projection](#power-projection)
   * [Ideas](#ideas)
   * [Technology](#technology)
   * [Estates](#estates)
      * [Burghers](#burghers)
      * [Clergy](#clergy)
      * [Nobility](#nobility)
      * [Dhimmi](#dhimmi)
* [Script](#script)
   * [Decisions](#decisions)
   * [Events](#events)
* [Modding](#modding)

***

## New Features

- The peasantry has learned the art of self-governance making sprawling empires more difficult to manage.
- Terrain once again reduces combat width making smaller nations playable again.
- Overlords can now negotiate tax rates with their vassals.󠀡

***

## Game Balance

### Economy

- War taxes now decrease land and naval maintenance by -25%<sup>(-15%)</sup> and increases war exhaustion by +0.065 for player countries and +0.015 for AI countries.
- *Centralization Edict* now decreases local monthly autonomy by -0.05.<sup>(-0.03)</sup>

#### Capital

- Nation's capital provinces now increases local taxes by +30%.
- Nation's capital state now lowers local autonomy by -15% and local unrest by -1.5.

#### Development

- Province development now increases local defensiveness by +1.5% per development level invested in manpower.
- Developing provinces that belong to estates now increases monthly estate loyalty for a while.

### Diplomacy

- Each royal marriage now increases yearly legitimacy gain by +0.15.<sup>(+0.10)</sup>

### Buildings

- **Dock** now increases provincial trade modifier by +15%.

- **Regimental Camp** now reduces local recruitment speed by +35%.

- <details>
  <summary>Changed <b>Courthouse</b> local province modifiers.</summary>
  <ul>
  	<li><code>State Maintenance: -60% <sup>(-50%)</sup></code></li>
  	<li><code>Local Unrest: -3</code></li>
  	<li><code>Local Culture Conversion Cost: -30%</code></li>
  </ul>
  </details>
- <details>
  <summary>Changed <b>Town Hall</b> local province modifiers.</summary>
  <ul>
  	<li><code>State Maintenance: -30% <sup>(-25%)</sup></code></li>
    <li><code>Local Unrest: -2</code></li>
 	<li><code>Monthly Autonomy Change: -0.1</code></li>
  </ul>
  </details>

#### Administrative

- Courthouse and Town Hall are now considered *administrative buildings*.
- <details>
  <summary>Administrative buildings unlock a unique mechanic that provides state-wide governance modifiers.</summary>
  Having this type of building in a province turns that province into a <i>State Administrative Center</i> that in addition to standard building modifiers provides additional bonuses:
      <ul>
      	<br><li>In the province in which it was built:</li>
  			<ul>
  				<li><code>Local development cost: -5.0%</code></li>
  				<li><code>Minimum local autonomy: -10</code></li>
              </ul>
  		<br><li>In each province that is part of the state in which the administrative building is built:</li>
  		<ul>
                <li><code>State maintenance: -20%</code></li>
  				<li><code>Minimum local autonomy: -5</code></li>
  				<li><code>Monthly autonomy change: -0.05</code></li>
  				<li><code>Local unrest: -1</code></li>
      		</ul>
      	</ul>
  </details>

- Administrative buildings get removed when the province it is built on is no longer part of a state, for example when a country abandons the state or the province changes ownership to a country that has not established a state in that region. In addition to this each state can now have <u>only one</u> administrative building.


### Advisors

All advisor types now have secondary modifiers (some also having hidden tertiary modifiers) to increase their usefulness in more diverse scenarios beyond just providing monarch points.

- <details>
	<summary><b>Philosopher</b> now also lowers idea cost by -5%.</summary>
	<ul>
		<li>This advisor is more likely to join court if the country has completed the Humanist idea group or has taken <i>Patron of the Arts</i> idea from the Innovativeness idea group.</li>
		<li>AI is more likely to hire this advisor if it has low prestige.</li>
	    <li>Also grants a hidden modifier that increases innovativeness gain by +15%.</li>
</ul>
</details>
- <details>
	<summary><b>Natural scientist</b> now also increases innovativeness gain by +25%.</summary>
	<ul>
		<li>This advisor is more likely to join court if the country has taken <i>Scientific Revolution</i> idea from the Innovativeness idea group.</li>
		<li>AI is more likely to hire this advisor if it's production income percentage is +30% or higher.</li>
	</ul>
</details>
	
- <details>
	<summary><b>Artist</b> now also slows prestige decay by -1%.</summary>
	<ul>
		<li>This advisor is more likely to join court if the country has taken <i>Patron of the Arts</i> idea from the Innovativeness idea group or is Papal State and has taken <i>The Vatican Museums</i> national idea.</li>
		<li>AI is proportionately more likely to hire this advisor when it has negative stability.</li>
      <li>Also grants a hidden modifier that increases innovativeness gain by +15%.</li>
	</ul>
	</details>
	
- <details>
	<summary><b>Treasurer</b> now also decreases build cost by -5%.</summary>
	<ul>
		<li>This advisor is more likely to join court if the country has taken <i>Debt and Loans</i> or <i>Bureaucracy</i> idea from the Economic idea group.</li>
		<li>AI is more likely to hire this advisor when its tax income percentage is 30% or higher.</li>
	</ul>
</details>
	
- <details>
	<summary><b>Theologian</b> now also increases tolerance of heretics by +1.</summary>
	<ul>
		<li>This advisor is more likely to join court if the country is either Papal State or a Theocracy, or has completed the Religious idea group.</li>
		<li>AI is proportionally more likely to hire this advisor if it's average national unrest is 4 or lower.</li>
	</ul>
</details>
	
- <details>
	<summary><b>Master of Mint</b> now also lowers inflation reduction cost by -20%.</summary>
	<ul>
		<li>This advisor is more likely to join court if the country has taken <i>National Bank</i> idea from the Economic idea group.</li>
		<li>AI is proportionally more likely to hire this advisor if it's inflation rate is 5% or higher.</li>
	</ul>
</details>
	
- <details>
	<summary><b>Inquisitor</b> now increases missionary strength by +1% <sup>(+2%)</sup> and decreases national unrest by -1.</summary>
	<ul>
	    <li>
	        <details>
	            <summary>In addition to those listed above this advisor grants more hidden modifiers.</summary>
		<ul>
            <li><code>Tolerance of Heretics: -1</code></li>
	            <li><code>Missionary Strength vs Heretics: -0.01</code></li>
	            <li><code>Innovativeness Gain: -0.3</code></li><br>
	    	</ul>
	    </li>
		<li>This advisor is more likely to join court in the age of reformation and less likely to join court if the country has completed the <i>Humanist</i> idea group.</li>
		<li>AI is more likely to hire this advisor in the age of reformation.</li>
	</ul>
	</details>
	
- <details>
	<summary><b>Statesman</b> now also increases administrative efficiency by -5%.</summary>
	<ul>
		<li>Also grants a hidden modifier that reduces Administrative Technology Cost by -3%.</li>
	</ul>
</details>

- <details>
	<summary><b>Naval Reformer</b> now increases sailor recovery speed by +15%.</summary>
	<ul>
		<li>Also grants a hidden modifier that reduces Diplomatic Technology Cost by -3%.</li>
	</ul>
</details>

- **Trader** now also improves trade steering by +10%.

- **Spymaster** now also increases global spy defense by +15%.

- **Diplomat** now also increases diplomatic relations cap by +1.

- **Navigator** now also decreases naval attrition by -25%.

- **Army Reformer** now also increases yearly army professionalism gain by +0.5.

- **Commandant** now increases discipline by +4% <sup>(+5%)</sup> and monthly drill gain by +25%.

- <details>
      <summary><b>Army organizer</b> now increases manpower recovery speed by +20% and reinforcement speed by +25%.</summary>
      Previously increased land force limit by 10%.
  </details>

- <details>
      <summary><b>Quartermaster</b> now increases army moral recovery speed by +5% and decreases army land attrition by -20%.</summary>
      Previously increased reinforcement speed by 33%.
  </details>
  
- <details>
	<summary><b>Military Engineer</b> now increases province defensiveness by +25% <sup>(+20%)</sup> and army siege ability by 10%.</summary>
	<ul>
		<li>This advisor is more likely to join court if the country has taken <i>Defensive Mentality</i> idea from the Defensive idea group. AI is more likely to hire this advisor if losing a war.</li>
	    <li>Also grants a hidden modifier that reduces Military Technology Cost by -3%.</li>
</ul>
</details>

- **Master Recruiter** now increases regiment recruitment speed by +20%.

- **Grand Captain** now increases prestige gain from land battle by +20%.

### Military 

- Countries can now maintain up to 2 <sup>(1)</sup> military leaders without incurring a penalty to military power.
- Average number of months for increasing general pips when drilling 100% of force limit decreased to 90.<sup>(120)</sup>

#### Army Professionalism

- Conscription Army `(AP>=0.6)` now also decreases regiment reinforce cost by -20%.
- Permanent Army `(AP>=0.8)` now also decreases general cost by -50% .
- Professional Army `(AP=1.0)` now increases leader siege by +1.0, increases army drill gain by +50% and no longer decreases general cost by 50% (this was moved to Permanent Army level).
- Individual regiments now gain reduced land attrition by -25% when drilled at 100%.
- <details>
   <summary>Changed national effects of having low and high army professionalism.</summary>
      <ul><br>
          <li>Effect of low army professionalism:</li>
          <ul>
              <li><code><s>Mercenary Cost: -15.0%</s></code></li>
              <li><code>Land Attrition: +20.0%</code></li>
              <li><code>Possible Mercenaries: +15.0%</code></li>
          </ul><br>
          <li>Effects of high army professionalism:</li>
          <ul>
              <li><code>Land Maintenance Modifier: +30.0%</code></li>
              <li><code>Recruitment Time: +50.0%</code></li>
              <li><code>Siege Ability: +15.0% <sup>(+20.0%)</sup></code></li>
              <li><code>Land Fire Damage: +10.0%</code></li>
              <li><code>Shock Damage: +10.0%</code></li>
              <li><code>Drill Gain Modifier: +50.0%</code></li>
          </ul>
     </ul>
  </details>
  

#### Army Drilling

- Yearly army drill decay for regiments decreased to -1.7.<sup>(-2.5)</sup>
- Yearly army drill gain for regiments increased to 12.<sup>(10)</sup>

#### Power Projection

- <details>
		<summary>Most power projection yearly decay values are now reduced by 50%.</summary>
       <sub>See list of changes to <code>common/powerprojection/00_static.txt</code><a href="https://github.com/yooksi/eu4-EVE/commit/eb6b6333cabf5259f5c4e867ac5ff5d32d05e077#diff-88b96238a175258be5eb88b61001238e"></a>📝</sub>
	</details>
- Warning rivals now gives 5 <sup>(0)</sup> power projection.
- Guaranteeing independence of countries that are neighboring your rivals now gives 5 <sup>(0)</sup> power projection.

### Ideas

- Quality idea group bonus now also increases yearly army drill gain by +50%.
- Some [idea group bonuses](#estates) now increase estate influence and monthly loyalty gain.

### Technology

- Innovativeness penalty from being behind neighbors in tech decreased to 0.025.<sup>(0.03)</sup>
- Innovativeness bonus from being ahead of time in tech increased to 0.025 <sup>(0.005)</sup> to match the penalty value.
- Both penalty and bonus to innovativeness will now be applied for each technology types by additively stacking. For example, if a country is behind in all 3 tech types it will incur `0.075 (0.025 x 3)` penalty to innovativeness.
- <details>
      <summary>Changed national effects given by innovativeness at 100.</summary>
      <ul>
          <li><code>Yearly Army Tradition Decay: -1.3% <sup>(-1.0%)</sup></code></li>
          <li><code>Yearly Navy Tradition Decay: -1.3% <sup>(-1.0%)</sup></code></li>
          <li><code>All Power Costs: -20.0% <sup>(-10.0%)</sup></code></li>
          <li><code>Institution Embracement Cost: -35.0%</code></li>
          <li><code>Institution Spread: +50.0%</code></li>
      </ul>
  </details>

### Estates

- Minimum autonomy in estate provinces lowered to 20.<sup>(25)</sup>
- Estate loyalty gain from granting provinces increased to 2.5.<sup>(1.0)</sup>
- Maximum estate loyalty decay per year increased to 2.5.<sup>(2.0)</sup>
- Developing an estate province increases monthly loyalty gain by `x2.5` for 3 months.
- Cooldown from granting provinces to estates increased to 5 <sup>(1)</sup> years.
- Single estate seizing control of the nation now lowers monthly estate loyalty gain for -30%.<sup>(+20%)</sup>

#### Burghers

- Plutocratic idea group bonus now increases estate influence for +5% and monthly loyalty gain by +20%.<sup>(+10%)</sup>
- Completing the Trade idea group now increases Burghers estate monthly loyalty gain for +10%.
- <details>
  <summary>Changed Burghers nationwide and province modifiers.</summary>
  <ul>
  <br><li>
  <details>
  	<summary>Modifiers when estate is <span style="color:green">loyal</span>:</summary>			<br><ul>
  		<li><b>National modifiers</b>:</li>
         		<ul>
          		<li><code>Development Cost: -10.0%</code></li>
        			<li><code>Trade Efficiency: +25.0% <sup>(+20.0%)</sup></code></li>
      			<li><code>Production Efficiency: +10.0%</code></li>
        			<li><code>Institution Spread: +6.0%</code></li>
        		</ul><br>
        	<li><b>Province modifiers</b>:</li>
        		<ul>
                  <li><code>Local Construction Cost: -25.0%</code></li>
        			<li><code>Local Trade Power: +70.0% <sup>(+50.0%)</sup></code></li>
        			<li><code>Local Goods Produced: +15.0% <sup>(+10.0%)</sup></code></li>
        		</ul>
         </ul>
  	</details>
    	</li><br><li>
  	<details>
  	<summary>Modifiers when estate is neutral:</summary>
   	<br><ul>
         	<li><b>National modifiers</b>:</li>
         		<ul>
          		<li><code>Trade Efficiency: +20.0%</code></li>
        			<li><code>Production Efficiency: +5.0%</code></li>
              </ul>
         	  <br>
        	<li><b>Province modifiers</b>:</li>
        		<ul>
                  <li><code>Local Trade Power: +50.0%</code></li>
        			<li><code>Local Goods Produced: +10.0%</code></li>
  			</ul>
         </ul>
    </details>
    </li><br><li>
    <details>
        <summary>Modifiers when estate is <span style="color:red">disloyal</span>:</summary>
        <br><ul>
         	<li><b>National modifiers</b>:</li>
         		<ul>
        			<li><code>Development Cost: +20.0% <sup>(-10.0%)</sup></code></li>
        			<li><code>Trade Efficiency: -30.0% <sup>(-10.0%)</sup></code></li>
        			<li><code>Production Efficiency: -20.0%</code></li>
       			<li><code>Yearly Corruption: +0.32</code></li>
       		</ul>
         	  <br>
  		<li><b>Province modifiers</b>:</li>
        		<ul>
                  <li><code>Local Construction Cost: +30.0%</code></li>
                  <li><code>Local Construction Time: +30.0%</code></li>
                  <li><code>Local Shipbuilding Time: +30.0%</code></li>
        			<li><code>Monthly Autonomy Change: +0.10</code></li>
        			<li><code>Local Unrest: +4.0 <sup>(+5.0)</sup></code></li>
  			</ul>
         </ul>
    </details>
  </details>

#### Clergy

- Religious idea group bonus now increases estate influence for +5% and monthly loyalty gain for +20%.<sup>(+10%)</sup>

- Protestant state religion now increases monthly estate loyalty gain for +20%.<sup>(+10%)</sup>

- Papal controller country now increases monthly estate loyalty gain for +20%.<sup>(+10%)</sup>

- <details>
  <summary>Changed Clergy nationwide and province modifiers.</summary>
  <ul>
  	<br><li>
  	<details>
  	<summary>Modifiers when estate is <span style="color:green">loyal</span>:</summary>			<br><ul>
  		<li><b>National modifiers</b>:</li>
  			<ul>
  				<li><code>National Tax Modifier: +20.0%</code></li>
  				<li><code>Stability Cost Modifier: -20.0% <sup>(-10.0%)</sup></code></li>
  				<li><code>Yearly Legitimacy: +0.20</code></li>
  				<li><code>Yearly Devotion: +0.50</code></li>
                  <li><code>Yearly Papal Influence: +1.0</code></li>
  				<li><code>Church Power: +0.10</code></li>
  				<li><code>Monthly Fervor: +1.0</code></li>
  			</ul>
  		  <br>
  		<li><b>Province modifiers</b>:</li>
  			<ul>
  				<li><code>Local Tax Modifier: +15.0% <sup>(+10.0%)</sup></code></li>
				<li><code><s>Local Missionary Maintenance Cost: -25.0%</s></code></li>
  				<li><code>Local Missionary Strength: +2.0%</code></li>
  				<li><code>Local Unrest: -3.5 <sup>(-2.0)</sup></code></li>
  			</ul>
   		</ul>
  	</details>
  	</li><br><li>
  	<details>
  	<summary>Modifiers when estate is neutral:</summary>
  	<br><ul>
  		<li><b>National modifiers</b>:</li>
  			<ul>
  				<li><code>National Tax Modifier: +15.0% <sup>(+20.0%)</sup></code></li>
  				<li><code>Stability Cost Modifier: -10.0%</code></li>
  		  	</ul>
  		  <br>
  		<li><b>Province modifiers</b>:</li>
  			<ul>
  				<li><code>Local Tax Modifier: +10.0%</code></li>
				<li><code><s>Local Missionary Maintenance Cost: -10.0%</s></code></li>
  				<li><code>Local Missionary Strength: +1.0%</code></li>
  				<li><code>Local Unrest: -2.0</code></li>
  			</ul>
  	 	</ul>
  	</details>
  	</li><br><li>
  	<details>
  	<summary>Modifiers when estate is <span style="color:red">disloyal</span>:</summary>
  	<br><ul>
  		<li><b>National modifiers</b>:</li>
  			<ul>
				<li><code><s>Local Tax Modifier: -10.0%</s></code></li>
  				<li><code>Stability Cost Modifier: +30.0% <sup>(10.0%)</sup></code></li>
  				<li><code>Yearly Legitimacy: -0.30</code></li>
  				<li><code>Yearly Devotion: -0.50</code></li>
                  <li><code>Yearly Papal Influence: -1.5 <sup>(-1.0)</sup></code></li>
  				<li><code>Church Power: -0.20 <sup>(-0.25)</sup></code></li>
  				<li><code>Monthly Fervor: -1.0</code></li>
  				<li><code>Yearly Corruption: +0.20</code></li>
  		</ul><br>
  		<li><b>Province modifiers</b>:</li>
  			<ul>
  				<li><code>Institution Spread: -20.0%</code></li>
  				<li><code>Monthly Autonomy Change: +0.10</code></li>
  				<li><code>Local Unrest: +7.0 <sup>(+5.0)</sup></code></li>
  			</ul>
  	 	</ul>
  	</details>
  </details>

#### Nobility

- Aristocratic idea group bonus now increases influence for +5% and monthly loyalty gain for +20%.<sup>(+10%)</sup>

- High legitimacy `(>= 95)` now increases monthly estate loyalty gain for +15% *(+10%)*.

- Medium legitimacy `(>= 70 & < 94)` now increases monthly estate loyalty gain for +10% *(+5%)*.

- Low legitimacy `(>= 25 & < 49)` now lowers monthly estate loyalty gain for -10% *(-5%)*.

- Very low legitimacy `(< 25)` now lowers monthly estate loyalty gain for -20% *(-10%)*.

- <details>
     <summary>Changed Nobility nationwide and province modifiers.</summary>
       	<ul>
       	<br><li>
       	<details>
       		<summary>Modifiers when estate is <span style="color:green">loyal</span>:</summary>			<br><ul>
       			<li><b>National modifiers</b>:</li>
       	       		<ul>
       	        		<li><code>Manpower Recovery Speed: +25.0% <sup>(+20.0%)</sup></code></li>
       	      			<li><code>Land Maintenance Modifier: -10.0%</code></li>
					<li><code><s>Monthly Heir Support Gain: +0.33</s></code></li>
       	    			<li><code>Yearly Army Tradition: +0.40</code></li>
       	      			<li><code>Reinforce Speed: +20.0%</code></li>
       	      		</ul>
       	       	  <br>
       	      	<li><b>Province modifiers</b>:</li>
       	      		<ul>
       	                <li><code>Local Manpower Modifier: +25.0% <sup>(+20.0%)</sup></code></li>
       	      			<li><code>Garrison Growth: +10.0%</code></li>
       	      			<li><code>Local Defensiveness: +15.0%</code></li>
                         <li><code>Local Regiment Cost: -25.0%</code></li>
       	      			<li><code>Local Unrest: -2.0</code></li>
       	      		</ul>
       	       </ul>
       		</details>
       	  	</li><br><li>
       		<details>
       		<summary>Modifiers when estate is neutral:</summary>
       	 		<br><ul>
       	       	<li><b>National modifiers</b>:</li>
       	       		<ul>
       	        		<li><code>Manpower Recovery Speed: +20.0%</code></li>
       	      			<li><code>Land Maintenance Modifier: -5.0%</code></li>
       	            </ul>
       	       	  <br>
       	      	<li><b>Province modifiers</b>:</li>
       	      		<ul>
       	                <li><code>Local Manpower Modifier: +15.0% <sup>(+20.0%)</sup></code></li>
       	      			<li><code>Local Recruitment Time: -15.0%</code></li>
                         <li><code>Local Defensiveness: +10.0%</code></li>
       	      			<li><code>Local Unrest: -1.0</code></li>
       				</ul>
       	       </ul>
       	  </details>
       	  </li><br><li>
       	  <details>
       	      <summary>Modifiers when estate is <span style="color:red">disloyal</span>:</summary>
       	      <br><ul>
       	       	<li><b>National modifiers</b>:</li>
       	       		<ul>
     					<li><code>Manpower Recovery Speed: -30.0% <sup>(-10.0%)</sup></code></li>
       	      			<li><code>Land Maintenance Modifier: +15.0% <sup>(+10.0%)</sup></code></li>
       	      			<li><code>Reinforce Speed: -25.0%</code></li>
     					<li><code>Yearly Corruption: +0.16</code></li>
       	     		</ul>
       	       	  <br>
       			<li><b>Province modifiers</b>:</li>
       	      		<ul>
       	                <li><code>Local Manpower Modifier: -30.0%</code></li>
       	                <li><code>Local Regiment Cost: -30.0%</code></li>
       	                <li><code>Monthly Autonomy Change: +0.10</code></li>
       	      			<li><code>Local Unrest: +5.0</code></li>
       				</ul>
       	       </ul>
       	  </details>
       	</details>

#### Dhimmi

- Religious idea group bonus now increases monthly estate loyalty gain for +35%.

***

## Script

### Decisions

- <details>
	<summary>Changed <i>Elite Regiments</i> event modifier to make the associated decision more appealing.</summary>
	<ul>
		<li><code>Yearly Army Drill Gain: +50.0% <sup>(+40.0%)</sup></code>
		<li><code>Land Maintenance Modifier: +10.0% <sup>(+15.0%)</sup></code>
	    <li><code>Global Regiment Recruitment Speed: +50.0%</code></li>
	</ul>
</details>
	
- <details>
  <summary>Changed <i>Standardized Uniforms</i> event modifier to make the associated decision more flexible.</summary>
  <ul>
  	<li><code>Yearly Army Drill Gain: 25.0% <sup>(+40.0%)</sup></code>
  	<li><code>Land Morale: +10.0%</code>
  	<li><code>Land Attrition: -50.0%</code>
  </ul>
  </details>

### Events 

- *Commedia dell'Arte* event modifier now also lowers -0.5 national unrest.
- Accepting *Commedia dell'Arte* event now costs 15 <sup>(10)</sup> administrative power.
- *Rightful Ownership* event no longer triggers when overlord has a claim on subject's province (triggers only on cores now) and no longer removes overlord's claims when accepted.

## Modding

This will result in all provinces far away from the capital receiving a penalty to minimum local autonomy and monthly autonomy change proportional to relative distance from the capital.

[1]: https://github.com/yooksi/eu4-EVE/wiki/Mechanics#estate-loyalty "Estate loyalty mechanics"