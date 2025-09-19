# Unciv-mod-example

An example mod for Unciv, that adds one new Civilization.

For information on how to build and use mods, please refer to [the setup instructions](https://yairm210.github.io/Unciv/Modders/Making-a-new-Civilization/)



UNITà

[
/* All Eras */
     {
    "name": "Sacerdotessa Lupa",
    "unitType": "Civilian",
    "uniqueTo": "Nikelino",
    "cost": 300,
    "movement": 2,
    "strength": 0,
    "requiredTech": "Pottery",
    "actions": [],
    "uniques": [
      "Unbuildable by other Civilizations",
      "Only buildable in capital",
      "When this unit is present, player gains +1 Happiness per turn",
      "Can be captured (like a Settler)"
       ]
       },
/* Ancient Era */
	    {
		"name": "Tracio", /* Immagine Brute */
		"unitType": "Sword",
		"uniqueTo": "Nikelino",
		"movement": 2,
		"strength": 6,
		"cost": 30,
		"obsoleteTech": "Metal Casting",
		"upgradesTo": "Swordsman",
		"attackSound": "nonmetalhit"
	},
	{
		"name": "Guerriera amazzone",
		 "icon": "Guerriera amazzone",
		"unitType": "Sword",
		"uniqueTo": "Nikelino",
		"movement": 2,
		"strength": 12,
		"cost": 30,
		"obsoleteTech": "Metal Casting",
		"upgradesTo": "Swordsman",
		"attackSound": "nonmetalhit"
	},
	{
		"name": "Arcere amazzone", /* Immagine ADULT */
		"unitType": "Archery",
		"uniqueTo": "Nikelino",
		"movement": 2,
		"strength": 7,
		"rangedStrength": 7,
		"cost": 60,
		"requiredTech": "Archery",
		"obsoleteTech": "Construction",
		"upgradesTo": "Composite Bowman",
		"attackSound": "arrow"
	},
		{
		"name": "Dacio", /* Immagine Skirmisher */
		"unitType": "Archery",
		"uniqueTo": "Nikelino",
		"movement": 2,
		"strength": 3,
		"rangedStrength": 7,
		"cost": 30,
		"requiredTech": "Archery",
		"obsoleteTech": "Machinery",
		"upgradesTo": "Crossbowman",
		"attackSound": "arrow"
	},
		{
		"name": "Unno", /* Immagine Horse Archer */
		"unitType": "Archery",
		"uniqueTo": "Nikelino",
		"movement": 4,
		"strength": 7,
		"rangedStrength": 10,
		"cost": 56,
		"requiredTech": "The Wheel",
		"upgradesTo": "Knight",
		"obsoleteTech": "Chivalry",
		"uniques": ["No defensive terrain bonus"],
		"promotions": ["Accuracy I"],
		"attackSound": "arrow"
	},
	{
		"name": "Oplite siracusano", /* Immagine Hoplite*/
		"unitType": "Sword",
		"uniqueTo": "Nikelino",
		"movement": 2,
		"strength": 13,
		"cost": 56,
		"requiredTech": "Bronze Working",
		"obsoleteTech": "Civil Service",
		"upgradesTo": "Pikeman",
		"uniques": ["[+50]% Strength <vs [Mounted] units>"],
		"attackSound": "metalhit"
	},
	{
		"name": "Guerriero Taurino", /* Immagine Pictish Warrior*/
		"unitType": "Sword",
		"uniqueTo": "Nikelino",
		"movement": 2,
		"strength": 11,
		"cost": 56,
		"requiredTech": "Bronze Working",
		"obsoleteTech": "Civil Service",
		"upgradesTo": "Pikeman",
		"uniques": ["Earn [50]% of killed [Military] unit's [Strength] as [Faith]"],
		"promotions": ["Pictish Courage"],
		"attackSound": "metalhit"
	},
	{
		"name": "Germano", /* Immagine Marauder*/
		"unitType": "Sword",
		"uniqueTo": "Nikelino",
		"movement": 2,
		"strength": 8,
		"cost": 36,
		"requiredTech": "Bronze Working",
		"obsoleteTech": "Civil Service",
		"upgradesTo": "Pikeman",
		"uniques": ["[+50]% Strength <vs [Mounted] units>"],
		"attackSound": "metalhit"
	},
	{
		"name": "Lanciere Nubiano", /* Immagine DA FARE*/
		"unitType": "Sword",
		"movement": 2,
		"strength": 13,
		"cost": 66,
		"requiredTech": "Bronze Working",
		"obsoleteTech": "Civil Service",
		"upgradesTo": "Pikeman",
		"uniques": ["[+50]% Strength <vs [Mounted] units>"],
		"attackSound": "metalhit"
	},
	{
		"name": "Guerriero sardo", /* Immagine DA FARE*/
		"unitType": "Sword",
		"uniqueTo": "Shardana",
		"replaces": "Warrior",
		"movement": 2,
		"strength": 10,
		"cost": 30,
		"obsoleteTech": "Metal Casting",
		"promotions": ["Sangue di Drago"],
		"upgradesTo": "Swordsman",
		"attackSound": "nonmetalhit"
	},
	{
		"name": "Trireme sarda", /* Immagine DA FARE*/
		"unitType": "Melee Water",
		"uniqueTo": "Shardana",
		"replaces": "Trireme",
		"movement": 5,
		"strength": 13,
		"cost": 55,
		"requiredTech": "Sailing",
		"upgradesTo": "Caravel",
		"obsoleteTech": "Astronomy",
		"attackSound": "nonmetalhit"
	},
	/* Classical Era */
	{
		"name": "Ballista nikelinese", /* Immagine Ballista */
		"unitType": "Siege",
		"replaces": "Catapult",
		"uniqueTo": "Nikelino",
		"movement": 2,
		"strength": 10,
		"rangedStrength": 10,
		"cost": 75,
		"requiredTech": "Mathematics",
		"obsoleteTech": "Physics",
		"upgradesTo": "Trebuchet",
		"uniques": ["[+200]% Strength <vs cities> <when attacking>", "No defensive terrain bonus",
			"Must set up to ranged attack", "[-1] Sight"],
		"hurryCostModifier": 20,
		"attackSound": "throw"
	},
	{
		"name": "Legionario di Paolo", /* Immagine Legion */
		"unitType": "Sword",
		"uniqueTo": "Nikelino",
		"replaces": "Swordsman",
		"movement": 2,
		"strength": 17,
		"cost": 75,
		"requiredTech": "Iron Working",
		"upgradesTo": "Longswordsman",
		"obsoleteTech": "Gunpowder",
		"requiredResource": "Iron",
		"uniques": ["Can build [Road] improvements on tiles", "Can build [Fort] improvements on tiles"],
		"hurryCostModifier": 20,
		"attackSound": "metalhit"
	},
	{
		"name": "Amazzone a cavallo", /* Immagine ADULT */
		"unitType": "Mounted",
		"movement": 5,
		"strength": 14,
		"cost": 85,
		"requiredTech": "Horseback Riding",
		"requiredResource": "Horses",
		"upgradesTo": "Knight",
		"obsoleteTech": "Chivalry",
		"uniques": ["Can move after attacking","No defensive terrain bonus","[-33]% Strength <vs cities> <when attacking>" ],
		"hurryCostModifier": 20,
		"attackSound": "horse"
	},
	{
		"name": "Elefante africano", /* Immagine African Forest Elephant*/
		"unitType": "Mounted",
		"uniqueTo": "Nikelino",
		"movement": 3,
		"strength": 14,
		"cost": 100,
		"requiredTech": "Horseback Riding",
		"upgradesTo": "Knight",
		"obsoleteTech": "Chivalry",
		"promotions": ["Great Generals II"],
		"uniques": ["Can move after attacking", "No defensive terrain bonus", "[-33]% Strength <vs cities> <when attacking>",
			"[-10]% Strength for enemy [Military] units in adjacent [All] tiles"],
		"hurryCostModifier": 20,
		"attackSound": "elephant"
	},
	
]
