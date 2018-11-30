# Units mod

## [English Longbowman](http://civilopedia.serenity.pw/civilopedia/en-us/UNIT_ENGLISH_LONGBOWMAN.php)

- Moved to class *UNITCLASS_COMPOSITE_BOWMAN*;
- Weakened slightly.

Mod in *CIV5Units*

```xml
	<Units>
		<Row>
			<Class>UNITCLASS_COMPOSITE_BOWMAN</Class><!-- UNITCLASS_CROSSBOWMAN -->
			<Type>UNIT_ENGLISH_LONGBOWMAN</Type>
			<PrereqTech>TECH_CONSTRUCTION</PrereqTech><!-- TECH_MACHINERY -->
			<Combat>7</Combat><!-- 13 -->
			<RangedCombat>11</RangedCombat><!-- 18 -->
			<Cost>75</Cost><!-- 120 -->
			<FaithCost>150</FaithCost><!-- 240 -->
			<GoodyHutUpgradeUnitClass>UNITCLASS_CROSSBOWMAN</GoodyHutUpgradeUnitClass><!-- UNITCLASS_GATLINGGUN -->
		</Row>
	</Units>
	<Unit_ClassUpgrades>
		<Row>
			<UnitType>UNIT_ENGLISH_LONGBOWMAN</UnitType>
			<UnitClassType>UNITCLASS_CROSSBOWMAN</UnitClassType><!-- UNITCLASS_GATLINGGUN -->
		</Row>
	</Unit_ClassUpgrades>
```

Mod in *CIV5Civilizations*

```xml
	<Civilization_UnitClassOverrides>
		<Row>
			<CivilizationType>CIVILIZATION_ENGLAND</CivilizationType>
			<UnitClassType>UNITCLASS_COMPOSITE_BOWMAN</UnitClassType><!-- UNITCLASS_CROSSBOWMAN -->
			<UnitType>UNIT_ENGLISH_LONGBOWMAN</UnitType>
		</Row>
	</Civilization_UnitClassOverrides>
```

## [Winged Hussar](http://civilopedia.serenity.pw/civilopedia/en-us/UNIT_POLISH_WINGED_HUSSAR.php)

- Moved to class *UNITCLASS_KNIGHT*;
- Enhanced slightly.

Mod in *CIV5Civilizations_Expansion2*

```xml
	<Civilization_UnitClassOverrides>
		<Row>
			<CivilizationType>CIVILIZATION_POLAND</CivilizationType>
			<UnitClassType>UNITCLASS_KNIGHT</UnitClassType><!-- UNITCLASS_LANCER -->
			<UnitType>UNIT_POLISH_WINGED_HUSSAR</UnitType>
		</Row>
	</Civilization_UnitClassOverrides>
```

Mod in *CIV5Units_Expansion2*

```xml
		<Row>
			<Class>UNITCLASS_KNIGHT</Class><!-- UNITCLASS_LANCER -->
			<Type>UNIT_POLISH_WINGED_HUSSAR</Type>
			<PrereqTech>TECH_CHIVALRY</PrereqTech><!-- TECH_METALLURGY -->
			<Combat>23</Combat><!-- 28 -->
			<Cost>120</Cost><!-- 185 -->
			<FaithCost>240</FaithCost><!-- 370 -->
			<GoodyHutUpgradeUnitClass>UNITCLASS_CAVALRY</GoodyHutUpgradeUnitClass><!-- UNITCLASS_ANTI_TANK_GUN -->
		</Row>
	<Unit_ClassUpgrades>
		<Row>
			<UnitType>UNIT_POLISH_WINGED_HUSSAR</UnitType>
			<UnitClassType>UNITCLASS_CAVALRY</UnitClassType><!-- UNITCLASS_ANTI_TANK_GUN -->
		</Row>
	</Unit_ClassUpgrades>
```

## [Samurai](http://civilopedia.serenity.pw/civilopedia/en-us/UNIT_JAPANESE_SAMURAI.php)

- ClassUpgrade to Musketman rather than Rifleman

Mod in *CIV5Units*

```xml
	<Unit_ClassUpgrades>
		<Row>
			<UnitType>UNIT_JAPANESE_SAMURAI</UnitType>
			<UnitClassType>UNITCLASS_MUSKETMAN</UnitClassType><!-- UNITCLASS_RIFLEMAN -->
		</Row>
	</Unit_ClassUpgrades>
```

## [Battleship](http://civilopedia.serenity.pw/civilopedia/en-us/UNIT_BATTLESHIP.php)

- Enable ClassUpgrade to MISSILE CRUISER

Add in *CIV5Units*

```xml
	<Units>
		<Row>
			<Class>UNITCLASS_BATTLESHIP</Class>
			<Type>UNIT_BATTLESHIP</Type>
			<GoodyHutUpgradeUnitClass>UNITCLASS_MISSILE_CRUISER</GoodyHutUpgradeUnitClass><!-- UPGRADE TO MISSILE CRUISER-->
		</Row>
	</Units>
	<Unit_ClassUpgrades>
		<Row><!-- BATTLESHIP UPGRADE TO MISSILE CRUISER-->
			<UnitType>UNIT_BATTLESHIP</UnitType>
			<UnitClassType>UNITCLASS_MISSILE_CRUISER</UnitClassType>
		</Row>
```

## [Marine](http://civilopedia.serenity.pw/civilopedia/en-us/UNIT_MARINE.php)

- Enable ClassUpgrade to XCOM

Add in *CIV5Units_Inherited_Expansion2*

```xml
	<Units>
		<Replace>
			<Class>UNITCLASS_MARINE</Class>
			<Type>UNIT_MARINE</Type>
			<GoodyHutUpgradeUnitClass>UNITCLASS_XCOM_SQUAD</GoodyHutUpgradeUnitClass><!-- UPGRADE TO XCOM-->
	</Units>
	<Unit_ClassUpgrades>
		<Row><!-- UPGRADE TO XCOM-->
			<UnitType>UNIT_MARINE</UnitType>
			<UnitClassType>UNITCLASS_XCOM_SQUAD</UnitClassType>
		</Row>
	</Unit_ClassUpgrades>
```

## ADDITIONAL STRATEGIC RESOURCE REQUIREMENTS

### Affected Resource view

- IRON
  1. CANNON
  1. ARTILLERY
  1. ANTI_AIRCRAFT_GUN
  1. BATTLESHIP
  1. CARRIER
  1. DESTROYER
  1. SUBMARINE
  1. ANTI_TANK_GUN
  1. MOBILE_SAM
  1. TANK
  1. GERMAN_PANZER
  1. GUIDED_MISSILE
  1. MISSILE_CRUISER
  1. MODERN_ARMOR
  1. TRIPLANE
  1. WWI_BOMBER
- OIL
  1. CARRIER
  1. JET_FIGHTER
  1. MISSILE_CRUISER
  1. STEALTH_BOMBER
- ALUMINUM
  1. CARRIER
  1. SUBMARINE
  1. AMERICAN_B17
  1. BOMBER
  1. FIGHTER
  1. JAPANESE_ZERO
  1. MISSILE_CRUISER
  1. NUCLEAR_SUBMARINE
  1. Giant Death Robot
  1. JET_FIGHTER
  1. XCOM_SQUAD
  1. BAZOOKA
- URANIUM
  1. NUCLEAR_SUBMARINE
  1. ATOMIC_BOMB
  1. NUCLEAR_MISSILE

### Affected Units view (multiple resource)

- BATTLESHIP
  - 2 IRON
- CARRIER
  - 2 IRON
  - ALUMINUM
  - OIL
- SUBMARINE
  - IRON
  - ALUMINUM
- MISSILE_CRUISER
  - IRON
  - OIL
  - ALUMINUM
- JET_FIGHTER
  - OIL
  - 2 ALUMINUM
- STEALTH_BOMBER
  - 2 OIL
- NUCLEAR_SUBMARINE
  - ALUMINUM
  - URANIUM
- Giant Death Robot
  - 2 ALUMINUM
- ATOMIC_BOMB
  - 2 URANIUM
- NUCLEAR_MISSILE
  - 3 URANIUM

### Code

Add in *CIV5Units*

```xml
	<Unit_ResourceQuantityRequirements>
	<!--  TEMPLATE
		<Row>
			<UnitType>NAME</UnitType>
			<ResourceType>RESOURCE</ResourceType>
			DEFAULT COST IS 1
			<Cost>2</Cost>
		</Row>
	-->
	<!-- ADDITIONAL STRATEGIC RESOURCE REQUIREMENTS -->
		<!-- RENAISSANCE ERA -->
		<Row>
			<UnitType>UNIT_CANNON</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<!-- INDUSTRIAL ERA -->
		<Row>
			<UnitType>UNIT_ARTILLERY</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<!-- MODERN ERA -->
		<Row>
			<UnitType>UNIT_ANTI_AIRCRAFT_GUN</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_BATTLESHIP</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
			<Cost>2</Cost>
		</Row>
		<Row>
			<UnitType>UNIT_CARRIER</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
			<Cost>2</Cost>
		</Row>
		<Row>
			<UnitType>UNIT_CARRIER</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_CARRIER</UnitType>
			<ResourceType>RESOURCE_OIL</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_DESTROYER</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_SUBMARINE</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_SUBMARINE</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
		</Row>
		<!-- ATOMIC ERA -->
		<Row>
			<UnitType>UNIT_ANTI_TANK_GUN</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_AMERICAN_B17</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_BOMBER</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_FIGHTER</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_JAPANESE_ZERO</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_MOBILE_SAM</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_TANK</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_GERMAN_PANZER</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<!-- INFORMATION ERA -->
		<Row>
			<UnitType>UNIT_GUIDED_MISSILE</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_JET_FIGHTER</UnitType>
			<ResourceType>RESOURCE_OIL</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_MISSILE_CRUISER</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_MISSILE_CRUISER</UnitType>
			<ResourceType>RESOURCE_OIL</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_MISSILE_CRUISER</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
			<Cost>2</Cost>
		</Row>
		<Row>
			<UnitType>UNIT_MODERN_ARMOR</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_NUCLEAR_SUBMARINE</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_NUCLEAR_SUBMARINE</UnitType>
			<ResourceType>RESOURCE_URANIUM</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_STEALTH_BOMBER</UnitType>
			<ResourceType>RESOURCE_OIL</ResourceType>
			<Cost>2</Cost>
		</Row>
		<Row>
			<UnitType>UNIT_MECH</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
			<Cost>2</Cost>
		</Row>
	<!-- END ADDITIONAL STRATEGIC RESOURCE REQUIREMENTS -->
		<Row>
			<UnitType>UNIT_ATOMIC_BOMB</UnitType>
			<ResourceType>RESOURCE_URANIUM</ResourceType>
			<Cost>2</Cost><!-- 1 -->
		</Row>
		<Row>
			<UnitType>UNIT_NUCLEAR_MISSILE</UnitType>
			<ResourceType>RESOURCE_URANIUM</ResourceType>
			<Cost>3</Cost><!-- 2 -->
		</Row>
		<Row>
			<UnitType>UNIT_JET_FIGHTER</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
			<Cost>2</Cost><!-- 1 -->
		</Row>
	</Unit_ResourceQuantityRequirements>
```

Mod in *CIV5Units_Expansion2*

```xml
	<Unit_ResourceQuantityRequirements>
	<!-- ADDITIONAL STRATEGIC RESOURCE REQUIREMENTS -->
		<Row>
			<UnitType>UNIT_XCOM_SQUAD</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_BAZOOKA</UnitType>
			<ResourceType>RESOURCE_ALUMINUM</ResourceType>
		</Row>
	<!-- END ADDITIONAL STRATEGIC RESOURCE REQUIREMENTS -->
	</Unit_ResourceQuantityRequirements>
```

Mod in *CIV5Units_Inherited_Expansion2*

```xml
	<Unit_ResourceQuantityRequirements>
	<!-- ADDITIONAL STRATEGIC RESOURCE REQUIREMENTS -->
		<Row>
			<UnitType>UNIT_TRIPLANE</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_WWI_BOMBER</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
		<Row>
			<UnitType>UNIT_WWI_TANK</UnitType>
			<ResourceType>RESOURCE_IRON</ResourceType>
		</Row>
	<!-- END ADDITIONAL STRATEGIC RESOURCE REQUIREMENTS -->
	</Unit_ResourceQuantityRequirements>
```