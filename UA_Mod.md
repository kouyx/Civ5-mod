# UA mod

Spoiler WARNING!

## Mod in *CIV5Traits_Polynesia*

```xml
		<Row>
			<Type>TRAIT_WAYFINDING</Type>
			<Description>TXT_KEY_TRAIT_WAYFINDING</Description>
			<ShortDescription>TXT_KEY_TRAIT_WAYFINDING_SHORT</ShortDescription>
			<EmbarkedAllWater>true</EmbarkedAllWater>
			<NearbyImprovementCombatBonus>10</NearbyImprovementCombatBonus>
			<NearbyImprovementBonusRange>2</NearbyImprovementBonusRange>
			<CombatBonusImprovement>IMPROVEMENT_MOAI</CombatBonusImprovement>
		<!-- START TEST -->
			<CityStateBonusModifier>25</CityStateBonusModifier>
			<FreeUnit>UNITCLASS_ENGINEER</FreeUnit>
			<FreeUnitPrereqTech>TECH_WRITING</FreeUnitPrereqTech>
			<FightWellDamaged>true</FightWellDamaged>
			<NavalUnitMaintenanceModifier>-33</NavalUnitMaintenanceModifier>
			<GreatPersonGiftInfluence>45</GreatPersonGiftInfluence>
			<DOFGreatPersonModifier>5</DOFGreatPersonModifier>
			<TradeRouteResourceModifier>50</TradeRouteResourceModifier>
			<AbleToAnnexCityStates>true</AbleToAnnexCityStates>
			<RazeSpeedModifier>50</RazeSpeedModifier>
			<UniqueLuxuryCities>4</UniqueLuxuryCities>
			<UniqueLuxuryQuantity>1</UniqueLuxuryQuantity>
			<UniqueLuxuryRequiresNewArea>false</UniqueLuxuryRequiresNewArea>
			<GoldenAgeGreatArtistRateModifier>35</GoldenAgeGreatArtistRateModifier>
			<GoldenAgeGreatMusicianRateModifier>15</GoldenAgeGreatMusicianRateModifier>
			<GoldenAgeGreatWriterRateModifier>25</GoldenAgeGreatWriterRateModifier>
			<FreeSocialPoliciesPerEra>1</FreeSocialPoliciesPerEra>
			<CrossesMountainsAfterGreatGeneral>true</CrossesMountainsAfterGreatGeneral>
			<FreeBuilding>BUILDING_IRONWORKS</FreeBuilding>
			<BonusReligiousBelief>true</BonusReligiousBelief>
			<NaturalWonderFirstFinderGold>200</NaturalWonderFirstFinderGold>
			<NaturalWonderSubsequentFinderGold>100</NaturalWonderSubsequentFinderGold>
			<NaturalWonderYieldModifier>50</NaturalWonderYieldModifier>
			<NaturalWonderHappinessModifier>50</NaturalWonderHappinessModifier>
			<CityUnhappinessModifier>50</CityUnhappinessModifier>
			<PopulationUnhappinessModifier>-25</PopulationUnhappinessModifier>
			<GoldenAgeDurationModifier>25</GoldenAgeDurationModifier>
			<GoldenAgeMoveChange>1</GoldenAgeMoveChange>
			<GoldenAgeCombatModifier>5</GoldenAgeCombatModifier>
			<CapitalBuildingModifier>10</CapitalBuildingModifier>
			<CityStateFriendshipModifier>50</CityStateFriendshipModifier>
			<PlotBuyCostModifier>-25</PlotBuyCostModifier>
			<WonderProductionModifier>10</WonderProductionModifier>
			<ExtraEmbarkMoves>1</ExtraEmbarkMoves>
			<EmbarkedToLandFlatCost>true</EmbarkedToLandFlatCost>
			<ExtraSpies>1</ExtraSpies>
			<GreatGeneralRateModifier>25</GreatGeneralRateModifier>
			<GreatGeneralExtraBonus>5</GreatGeneralExtraBonus>
			<LandUnitMaintenanceModifier>-10</LandUnitMaintenanceModifier>
			<MoveFriendlyWoodsAsRoad>true</MoveFriendlyWoodsAsRoad>
			<CultureFromKills>50</CultureFromKills>
			<CapitalThemingBonusModifier>50</CapitalThemingBonusModifier>
			<LandTradeRouteRangeBonus>3</LandTradeRouteRangeBonus>
			<TradeReligionModifier>50</TradeReligionModifier>
			<NumTradeRoutesModifier>50</NumTradeRoutesModifier>
			<LevelExperienceModifier>-10</LevelExperienceModifier>
			<ExtraFoundedCityTerritoryClaimRange>4</ExtraFoundedCityTerritoryClaimRange>
			<FasterInHills>true</FasterInHills>
			<ImprovementMaintenanceModifier>-25</ImprovementMaintenanceModifier>
			<NoHillsImprovementMaintenance>true</NoHillsImprovementMaintenance>
			<!--<TechBoostFromCapitalScienceBuildings>true</TechBoostFromCapitalScienceBuildings>-->
			<FaithFromUnimprovedForest>true</FaithFromUnimprovedForest>
			<CityCultureBonus>1</CityCultureBonus>
		<!-- END TEST -->
		</Row>
```

### Promotions mod

See *UA Promotions* in [Grant_free_pro_Mod](./Grant_free_pro_Mod.md)

### Improvement mod

```xml
	<Trait_ImprovementYieldChanges>
	<!-- START TEST -->
		<Row>
			<TraitType>TRAIT_WAYFINDING</TraitType>
			<ImprovementType>IMPROVEMENT_MINE</ImprovementType>
			<YieldType>YIELD_FOOD</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<TraitType>TRAIT_WAYFINDING</TraitType>
			<ImprovementType>IMPROVEMENT_FARM</ImprovementType>
			<YieldType>YIELD_PRODUCTION</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<TraitType>TRAIT_WAYFINDING</TraitType>
			<ImprovementType>IMPROVEMENT_PLANTATION</ImprovementType>
			<YieldType>YIELD_CULTURE</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<TraitType>TRAIT_WAYFINDING</TraitType>
			<ImprovementType>IMPROVEMENT_PASTURE</ImprovementType>
			<YieldType>YIELD_CULTURE</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<TraitType>TRAIT_WAYFINDING</TraitType>
			<ImprovementType>IMPROVEMENT_CAMP</ImprovementType>
			<YieldType>YIELD_CULTURE</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<TraitType>TRAIT_WAYFINDING</TraitType>
			<ImprovementType>IMPROVEMENT_TRADING_POST</ImprovementType>
			<YieldType>YIELD_CULTURE</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<TraitType>TRAIT_WAYFINDING</TraitType>
			<ImprovementType>IMPROVEMENT_FISHING_BOATS</ImprovementType>
			<YieldType>YIELD_CULTURE</YieldType>
			<Yield>1</Yield>
		</Row>
	<!-- END TEST -->
	</Trait_ImprovementYieldChanges>
```

## Mod in *CIV5Civilizations_Expansion2*

### UB

```xml
	<Civilization_BuildingClassOverrides>
	<!-- START TEST-->
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_WATERMILL</BuildingClassType>
			<BuildingType>BUILDING_FLOATING_GARDENS</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_BARRACKS</BuildingClassType>
			<BuildingType>BUILDING_KREPOST</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_LIBRARY</BuildingClassType>
			<BuildingType>BUILDING_ROYAL_LIBRARY</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_SHRINE</BuildingClassType>
			<BuildingType>BUILDING_MAYA_PYRAMID</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_MONUMENT</BuildingClassType>
			<BuildingType>BUILDING_STELE</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_WALLS</BuildingClassType>
			<BuildingType>BUILDING_WALLS_OF_BABYLON</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_MARKET</BuildingClassType>
			<BuildingType>BUILDING_BAZAAR</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_STABLE</BuildingClassType>
			<BuildingType>BUILDING_DUCAL_STABLE</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_TEMPLE</BuildingClassType>
			<BuildingType>BUILDING_MUD_PYRAMID_MOSQUE</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_GARDEN</BuildingClassType>
			<BuildingType>BUILDING_CANDI</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_WORKSHOP</BuildingClassType>
			<BuildingType>BUILDING_LONGHOUSE</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_CASTLE</BuildingClassType>
			<BuildingType>BUILDING_MUGHAL_FORT</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_UNIVERSITY</BuildingClassType>
			<BuildingType>BUILDING_WAT</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_WINDMILL</BuildingClassType>
			<BuildingType>BUILDING_COFFEE_HOUSE</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_OPERA_HOUSE</BuildingClassType>
			<BuildingType>BUILDING_CEILIDH_HALL</BuildingType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<BuildingClassType>BUILDINGCLASS_BANK</BuildingClassType>
			<BuildingType>BUILDING_HANSE</BuildingType>
		</Row>
	<!-- END TEST -->
	</Civilization_BuildingClassOverrides>
```

### UU

```xml
	<Civilization_UnitClassOverrides>
	<!-- START TEST -->
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_COMPOSITE_BOWMAN</UnitClassType><!-- UNITCLASS_CROSSBOWMAN -->
			<UnitType>UNIT_ENGLISH_LONGBOWMAN</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_CROSSBOWMAN</UnitClassType>
			<UnitType>UNIT_CHINESE_CHUKONU</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_SCOUT</UnitClassType>
			<UnitType>UNIT_SHOSHONE_PATHFINDER</UnitType>
		</Row>
		<!-- <Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_WARRIOR</UnitClassType>
			<UnitType>UNIT_AZTEC_JAGUAR</UnitType>
		</Row> -->
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_SWORDSMAN</UnitClassType>
			<UnitType>UNIT_ROMAN_LEGION</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_LONGSWORDSMAN</UnitClassType>
			<UnitType>UNIT_JAPANESE_SAMURAI</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_MUSKETMAN</UnitClassType>
			<UnitType>UNIT_FRENCH_MUSKETEER</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_RIFLEMAN</UnitClassType>
			<UnitType>UNIT_DANISH_SKI_INFANTRY</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_GREAT_WAR_INFANTRY</UnitClassType>
			<UnitType>UNIT_FRENCH_FOREIGNLEGION</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_INFANTRY</UnitClassType>
			<UnitType>UNIT_BRAZILIAN_PRACINHA</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_SPEARMAN</UnitClassType>
			<UnitType>UNIT_PERSIAN_IMMORTAL</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_PIKEMAN</UnitClassType>
			<UnitType>UNIT_GERMAN_LANDSKNECHT</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_LANCER</UnitClassType>
			<UnitType>UNIT_OTTOMAN_SIPAHI</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_TRIREME</UnitClassType>
			<UnitType>UNIT_BYZANTINE_DROMON</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_GALLEASS</UnitClassType>
			<UnitType>UNIT_VENETIAN_GALLEASS</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_FRIGATE</UnitClassType>
			<UnitType>UNIT_ENGLISH_SHIPOFTHELINE</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_CARAVEL</UnitClassType>
			<UnitType>UNIT_PORTUGUESE_NAU</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_PRIVATEER</UnitClassType>
			<UnitType>UNIT_DUTCH_SEA_BEGGAR</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_CHARIOT_ARCHER</UnitClassType>
			<UnitType>UNIT_INDIAN_WARELEPHANT</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_HORSEMAN</UnitClassType>
			<UnitType>UNIT_GREEK_COMPANIONCAVALRY</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_KNIGHT</UnitClassType>
			<UnitType>UNIT_POLISH_WINGED_HUSSAR</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_CAVALRY</UnitClassType>
			<UnitType>UNIT_AUSTRIAN_HUSSAR</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_TANK</UnitClassType>
			<UnitType>UNIT_GERMAN_PANZER</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_CATAPULT</UnitClassType>
			<UnitType>UNIT_ASSYRIAN_SIEGE_TOWER</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_TREBUCHET</UnitClassType>
			<UnitType>UNIT_KOREAN_HWACHA</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_BOMBER</UnitClassType>
			<UnitType>UNIT_AMERICAN_B17</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_FIGHTER</UnitClassType>
			<UnitType>UNIT_JAPANESE_ZERO</UnitType>
		</Row>
		<Row>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType>
			<UnitClassType>UNITCLASS_GREAT_GENERAL</UnitClassType>
			<UnitType>UNIT_MONGOLIAN_KHAN</UnitType>
		</Row>
	<!-- END TEST -->
	</Civilization_UnitClassOverrides>
```

## MARBLE, IVORY, JEWELRY, PORCELAIN in first 4 cities built

Add in *CIV5Resources*

```xml
		<Row>
			<Type>RESOURCE_MARBLE</Type>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType><!-- MOD -->
		</Row>
		<Row>
			<Type>RESOURCE_IVORY</Type>
			<CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType><!-- MOD -->
		</Row>
```

Add in *CIV5Resources_Inherited_Expansion2*

```xml
    <InsertOrAbort>
      <Type>RESOURCE_JEWELRY</Type>
      <CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType><!-- MOD -->
    </InsertOrAbort>
    <InsertOrAbort>
      <Type>RESOURCE_PORCELAIN</Type>
      <CivilizationType>CIVILIZATION_POLYNESIA</CivilizationType><!-- MOD -->
    </InsertOrAbort>
```
