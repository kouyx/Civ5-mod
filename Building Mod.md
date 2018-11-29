# Buildings Mod in Civ5

## Buildings in Civ5

### CIV5Buildings

```xml
	<Buildings>
		<Row>
			<Type>BUILDING_STONE_WORKS</Type>
			<ProhibitedCityTerrain>NULL</ProhibitedCityTerrain><!-- TERRAIN_PLAINS -->
		</Row>
	</Buildings>
	<Building_YieldChanges>
		<Row>
			<BuildingType>BUILDING_LONGHOUSE</BuildingType>
			<YieldType>YIELD_PRODUCTION</YieldType>
			<Yield>3</Yield><!-- 2 -->
		</Row>
	</Building_YieldChanges>
	<Building_LocalResourceOrs>
		<Row><!-- Resource - Mint Include Copper -->
			<BuildingType>BUILDING_MINT</BuildingType>
			<ResourceType>RESOURCE_COPPER</ResourceType>
		</Row>
	</Building_LocalResourceOrs>
	<Building_ResourceYieldChanges>
		<!-- START -->
		<Row><!-- Resource - Mint Include Copper -->
			<BuildingType>BUILDING_MINT</BuildingType>
			<ResourceType>RESOURCE_COPPER</ResourceType>
			<YieldType>YIELD_GOLD</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<BuildingType>BUILDING_MINT</BuildingType>
			<ResourceType>RESOURCE_GOLD</ResourceType>
			<YieldType>YIELD_GOLD</YieldType>
			<Yield>3</Yield><!-- 2 -->
		</Row>
		<Row><!-- Resource - SEAPORT ENHANCE CITRUS -->
			<BuildingType>BUILDING_SEAPORT</BuildingType>
			<ResourceType>RESOURCE_CITRUS</ResourceType>
			<YieldType>YIELD_GOLD</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row><!-- Resource - Granary Includes Bison -->
			<BuildingType>BUILDING_GRANARY</BuildingType>
			<ResourceType>RESOURCE_BISON</ResourceType>
			<YieldType>YIELD_FOOD</YieldType>
			<Yield>1</Yield>
		</Row>		
		<!-- END -->
	</Building_ResourceYieldChanges>
```
## Improved Caravansary

Caravansary now provides:

- Food and Production Trade Routes
- +1% Gold from City Connections (each Caravansary stacks)
- +50% Land Trade Route range
- +1 Gold from Salt.

The production cost has been increased from 120 to 150 as well.

### CIV5Buildings

```xml
		<Row>
			<Type>BUILDING_GRANARY</Type>
			<AllowsFoodTradeRoutes>false</AllowsFoodTradeRoutes><!-- true -->
		</Row>
		<Row>
			<Type>BUILDING_WORKSHOP</Type>
			<AllowsProductionTradeRoutes>false</AllowsProductionTradeRoutes><!-- true -->
		</Row>
```

### CIV5BuildingClasses_Expansion2

```xml
		<Row>
			<Type>BUILDINGCLASS_CARAVANSARY</Type>
			<DefaultBuilding>BUILDING_CARAVANSARY</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_CARAVANSARY</Description>
			<MaxPlayerInstances>10</MaxPlayerInstances><!-- ADD -->
		</Row>
```

### CIV5Buildings_Expansion2

```xml
		<Row>
			<Type>BUILDING_CARAVANSARY</Type>
			<Cost>150</Cost><!-- DEFAULT 120 -->
			<GoldMaintenance>1</GoldMaintenance><!-- ADD -->
			<CityConnectionTradeRouteModifier>1</CityConnectionTradeRouteModifier><!-- ADD -->
			<AllowsFoodTradeRoutes>true</AllowsFoodTradeRoutes><!-- ADD -->
			<AllowsProductionTradeRoutes>true</AllowsProductionTradeRoutes><!-- ADD -->
			<!--<TradeRouteLandGoldBonus>200</TradeRouteLandGoldBonus>-->
		</Row>
	<Building_ResourceYieldChanges>
		<!-- START -->
		<Row>
			<BuildingType>BUILDING_CARAVANSARY</BuildingType>
			<ResourceType>RESOURCE_SALT</ResourceType>
			<YieldType>YIELD_GOLD</YieldType>
			<Yield>1</Yield>
		</Row>
		<!-- END -->
	</Building_ResourceYieldChanges>
```

## BUILDING UPGRADE SYSTEM

### CIV5BuildingClasses_Expansion2

```xml
	<BuildingClasses>

	<!-- BUILDING UPGRADE SYSTEM -->
	<!-- START -->
		<!--  Cultural  -->
		<Row>
			<Type>BUILDINGCLASS_MONUMENT_UP</Type>
			<DefaultBuilding>BUILDING_MONUMENT_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_MONUMENT_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_AMPHITHEATER_UP</Type>
			<DefaultBuilding>BUILDING_AMPHITHEATER_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_AMPHITHEATER_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_OPERA_HOUSE_UP</Type>
			<DefaultBuilding>BUILDING_OPERA_HOUSE_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_OPERA_HOUSE_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_MUSEUM_UP</Type>
			<DefaultBuilding>BUILDING_MUSEUM_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_MUSEUM_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_BROADCAST_TOWER_UP</Type>
			<DefaultBuilding>BUILDING_BROADCAST_TOWER_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_BROADCAST_TOWER_UP</Description>
		</Row>

		<!--  Growth  -->
		<Row>
			<Type>BUILDINGCLASS_GRANARY_UP</Type>
			<DefaultBuilding>BUILDING_GRANARY_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_GRANARY_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_AQUEDUCT_UP</Type>
			<DefaultBuilding>BUILDING_AQUEDUCT_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_AQUEDUCT_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_HOSPITAL_UP</Type>
			<DefaultBuilding>BUILDING_HOSPITAL_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_HOSPITAL_UP</Description>
		</Row>
		
		<!--  Military  -->
		<Row>
			<Type>BUILDINGCLASS_BARRACKS_UP</Type>
			<DefaultBuilding>BUILDING_BARRACKS_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_BARRACKS_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_ARMORY_UP</Type>
			<DefaultBuilding>BUILDING_ARMORY_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_ARMORY_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_MILITARY_ACADEMY_UP</Type>
			<DefaultBuilding>BUILDING_MILITARY_ACADEMY_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_MILITARY_ACADEMY_UP</Description>
		</Row>
		
		<!--  Faith  -->
		<Row>
			<Type>BUILDINGCLASS_SHRINE_UP</Type>
			<DefaultBuilding>BUILDING_SHRINE_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_SHRINE_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_TEMPLE_UP</Type>
			<DefaultBuilding>BUILDING_TEMPLE_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_TEMPLE_UP</Description>
		</Row>
		
		<!--  City Def  -->
		<Row>
			<Type>BUILDINGCLASS_WALLS_UP</Type>
			<DefaultBuilding>BUILDING_WALLS_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_WALLS_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_CASTLE_UP</Type>
			<DefaultBuilding>BUILDING_CASTLE_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_CASTLE_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_ARSENAL_UP</Type>
			<DefaultBuilding>BUILDING_ARSENAL_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_ARSENAL_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_MILITARY_BASE_UP</Type>
			<DefaultBuilding>BUILDING_MILITARY_BASE_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_MILITARY_BASE_UP</Description>
		</Row>

		<!--  Sciences  -->
		<Row>
			<Type>BUILDINGCLASS_LIBRARY_UP</Type>
			<DefaultBuilding>BUILDING_LIBRARY_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_SHRINE_UP</Description>
		</Row>
		<Row>
			<Type>BUILDINGCLASS_UNIVERSITY_UP</Type>
			<DefaultBuilding>BUILDING_UNIVERSITY_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_UNIVERSITY_UP</Description>
		</Row>
		

		<!--  Prod  -->
		<Row>
			<Type>BUILDINGCLASS_WORKSHOP_UP</Type>
			<DefaultBuilding>BUILDING_WORKSHOP_UP</DefaultBuilding>
			<Description>TXT_KEY_BUILDING_WORKSHOP_UP</Description>
		</Row>
	<!-- END -->
	</BuildingClasses>
```

### CIV5Buildings_Expansion2

```xml
	<Buildings>
	<!-- BUILDING UPGRADE SYSTEM -->
	<!-- START -->
		<!--  Cultural  -->
		<Row>
			<Type>BUILDING_MONUMENT_UP</Type>
			<BuildingClass>BUILDINGCLASS_MONUMENT_UP</BuildingClass>
			<FreeStartEra>ERA_MEDIEVAL</FreeStartEra>
			<Cost>40</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<Help>TXT_KEY_BUILDING_MONUMENT_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_MONUMENT_UP</Description>
			<Civilopedia>TXT_KEY_BUILDING_MONUMENT_PEDIA</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_MONUMENT_UP_STRATEGY</Strategy>
			<ArtDefineTag>MONUMENT</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<HurryCostModifier>40</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>21</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_AMPHITHEATER_UP</Type>
			<BuildingClass>BUILDINGCLASS_AMPHITHEATER_UP</BuildingClass>
			<FreeStartEra>ERA_INDUSTRIAL</FreeStartEra>
			<Cost>100</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_DRAMA</PrereqTech>
			<Help>TXT_KEY_BUILDING_AMPHITHEATER_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_AMPHITHEATER_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_AMPHITHEATER_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_AMPHITHEATER_UP_STRATEGY</Strategy>
			<ArtDefineTag>COLESSEUM</ArtDefineTag>
			<SpecialistType>SPECIALIST_ARTIST</SpecialistType>
			<SpecialistCount>0</SpecialistCount>
			<MinAreaSize>-1</MinAreaSize>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>EXPANSION_BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>0</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_OPERA_HOUSE_UP</Type>
			<BuildingClass>BUILDINGCLASS_OPERA_HOUSE_UP</BuildingClass>
			<Cost>200</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_ACOUSTICS</PrereqTech>
			<Help>TXT_KEY_BUILDING_OPERA_HOUSE_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_OPERA_HOUSE_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_OPERA_HOUSE_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_OPERA_HOUSE_UP_STRATEGY</Strategy>
			<ArtDefineTag>OPERA_HOUSE</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<HurryCostModifier>10</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>49</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_MUSEUM_UP</Type>
			<BuildingClass>BUILDINGCLASS_MUSEUM_UP</BuildingClass>
			<Cost>300</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_ARCHAEOLOGY</PrereqTech>
			<Help>TXT_KEY_BUILDING_MUSEUM_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_MUSEUM_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_MUSEUM_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_MUSEUM_UP_STRATEGY</Strategy>
			<ArtDefineTag>MUSEUM</ArtDefineTag>
			<SpecialistType>SPECIALIST_ARTIST</SpecialistType>
			<SpecialistCount>0</SpecialistCount>
			<MinAreaSize>-1</MinAreaSize>
			<HurryCostModifier>0</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>22</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_BROADCAST_TOWER_UP</Type>
			<BuildingClass>BUILDINGCLASS_BROADCAST_TOWER_UP</BuildingClass>
			<Cost>500</Cost>
			<GoldMaintenance>3</GoldMaintenance>
			<PrereqTech>TECH_RADIO</PrereqTech>
			<Help>TXT_KEY_BUILDING_BROADCAST_TOWER_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_BROADCAST_TOWER_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_BROADCASTTOWER_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_BROADCAST_TOWER_UP_STRATEGY</Strategy>
			<ArtDefineTag>RADIO TOWER</ArtDefineTag>
			<SpecialistType>SPECIALIST_ARTIST</SpecialistType>
			<SpecialistCount>0</SpecialistCount>
			<MinAreaSize>-1</MinAreaSize>
			<CultureRateModifier>17</CultureRateModifier>
			<HurryCostModifier>0</HurryCostModifier>
			<DisplayPosition>2</DisplayPosition>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>35</PortraitIndex>
		</Row>
		
		<!--  Growth  -->
		<Row>
			<Type>BUILDING_GRANARY_UP</Type>
			<BuildingClass>BUILDINGCLASS_GRANARY_UP</BuildingClass>
			<FreeStartEra>ERA_RENAISSANCE</FreeStartEra>
			<Cost>60</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_POTTERY</PrereqTech>
			<Help>TXT_KEY_BUILDING_GRANARY_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_GRANARY_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_GRANARY_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_GRANARY_UP_STRATEGY</Strategy>
			<ArtDefineTag>ART_DEF_BUILDING_GRANARY</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<ConquestProb>66</ConquestProb>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<PortraitIndex>0</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_AQUEDUCT_UP</Type>
			<BuildingClass>BUILDINGCLASS_AQUEDUCT_UP</BuildingClass>
			<Cost>100</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_ENGINEERING</PrereqTech>
			<Help>TXT_KEY_BUILDING_AQUEDUCT_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_AQUEDUCT_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_AQUEDUCT_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_AQUEDUCT_UP_STRATEGY</Strategy>
			<ArtDefineTag>ART_DEF_BUILDING_HOSPITAL</ArtDefineTag>
			<FoodKept>10</FoodKept>
			<MinAreaSize>-1</MinAreaSize>
			<ConquestProb>66</ConquestProb>
			<HurryCostModifier>0</HurryCostModifier>
			<IconAtlas>NEW_BLDG_ATLAS2_DLC</IconAtlas>
			<PortraitIndex>0</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_HOSPITAL_UP</Type>
			<BuildingClass>BUILDINGCLASS_HOSPITAL_UP</BuildingClass>
			<Cost>360</Cost>
			<GoldMaintenance>2</GoldMaintenance>
			<PrereqTech>TECH_BIOLOGY</PrereqTech>
			<Help>TXT_KEY_BUILDING_HOSPITAL_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_HOSPITAL_UP</Description>
			<Civilopedia>TXT_KEY_BUILDING_HOSPITAL_PEDIA</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_HOSPITAL_UP_STRATEGY</Strategy>
			<ArtDefineTag>ART_DEF_BUILDING_HOSPITAL</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<ConquestProb>66</ConquestProb>
			<HurryCostModifier>0</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<PortraitIndex>45</PortraitIndex>
		</Row>


		<!--  Military  -->
		<Row>
			<Type>BUILDING_BARRACKS_UP</Type>
			<BuildingClass>BUILDINGCLASS_BARRACKS_UP</BuildingClass>
			<FreeStartEra>ERA_INDUSTRIAL</FreeStartEra>
			<Cost>75</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_BRONZE_WORKING</PrereqTech>
			<Help>TXT_KEY_BUILDING_BARRACKS_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_BARRACKS_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_BARRACKS_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_BARRACKS_UP_STRATEGY</Strategy>
			<ArtDefineTag>ART_DEF_BUILDING_BARRACKS</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>5</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_ARMORY_UP</Type>
			<BuildingClass>BUILDINGCLASS_ARMORY_UP</BuildingClass>
			<Cost>160</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_STEEL</PrereqTech>
			<Help>TXT_KEY_BUILDING_ARMORY_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_ARMORY_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_ARMORY_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_ARMORY_UP_STRATEGY</Strategy>
			<ArtDefineTag>ART_DEF_BUILDING_BARRACKS</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>6</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_MILITARY_ACADEMY_UP</Type>
			<BuildingClass>BUILDINGCLASS_MILITARY_ACADEMY_UP</BuildingClass>
			<Cost>300</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_MILITARY_SCIENCE</PrereqTech>
			<Help>TXT_KEY_BUILDING_MILITARY_ACADEMY_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_MILITARY_ACADEMY_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_MILITARYACADEMY_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_MILITARY_ACADEMY_UP_STRATEGY</Strategy>
			<ArtDefineTag>ART_DEF_BUILDING_MILITARY_ACADEMY</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<HurryCostModifier>0</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>8</PortraitIndex>
		</Row>

		<!--  Faith  -->
		<Row>
			<Type>BUILDING_SHRINE_UP</Type>
			<BuildingClass>BUILDINGCLASS_SHRINE_UP</BuildingClass>
			<FreeStartEra>ERA_MEDIEVAL</FreeStartEra>
			<MaxStartEra>ERA_RENAISSANCE</MaxStartEra>
			<Cost>40</Cost>
			<GoldMaintenance>2</GoldMaintenance>
			<PrereqTech>TECH_POTTERY</PrereqTech>
			<Help>TXT_KEY_BUILDING_SHRINE_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_SHRINE_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_SHRINE_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_SHRINE_UP_STRATEGY</Strategy>
			<ArtDefineTag>TEMPLE</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>EXPANSION_BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>9</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_TEMPLE_UP</Type>
			<BuildingClass>BUILDINGCLASS_TEMPLE_UP</BuildingClass>
			<MaxStartEra>ERA_RENAISSANCE</MaxStartEra>
			<Cost>100</Cost>
			<GoldMaintenance>2</GoldMaintenance>
			<PrereqTech>TECH_PHILOSOPHY</PrereqTech>
			<Help>TXT_KEY_BUILDING_TEMPLE_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_TEMPLE_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_TEMPLE_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_TEMPLE_UP_STRATEGY</Strategy>
			<ArtDefineTag>TEMPLE</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>37</PortraitIndex>
		</Row>

		<!--  City Def  -->
		<Row>
			<Type>BUILDING_WALLS_UP</Type>
			<BuildingClass>BUILDINGCLASS_WALLS_UP</BuildingClass>
			<Cost>75</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_MASONRY</PrereqTech>
			<Help>TXT_KEY_BUILDING_WALLS_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_WALLS_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_WALLS_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_WALLS_UP_STRATEGY</Strategy>
			<ArtDefineTag>ART_DEF_BUILDING_WALLS</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<AllowsRangeStrike>true</AllowsRangeStrike>
			<Defense>250</Defense>
			<ExtraCityHitPoints>25</ExtraCityHitPoints>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>32</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_CASTLE_UP</Type>
			<BuildingClass>BUILDINGCLASS_CASTLE_UP</BuildingClass>
			<Cost>160</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_CHIVALRY</PrereqTech>
			<Help>TXT_KEY_BUILDING_CASTLE_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_CASTLE_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_CASTLE_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_CASTLE_UP_STRATEGY</Strategy>
			<ArtDefineTag>CASTLE</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<AllowsRangeStrike>true</AllowsRangeStrike>
			<Defense>350</Defense>
			<ExtraCityHitPoints>13</ExtraCityHitPoints>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<DisplayPosition>1</DisplayPosition>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>33</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_ARSENAL_UP</Type>
			<BuildingClass>BUILDINGCLASS_ARSENAL_UP</BuildingClass>
			<Cost>300</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_METALLURGY</PrereqTech>
			<Help>TXT_KEY_BUILDING_ARSENAL_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_ARSENAL_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_ARSENAL_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_ARSENAL_UP_STRATEGY</Strategy>
			<ArtDefineTag>ART_DEF_BUILDING_MILITARY_ACADEMY</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<AllowsRangeStrike>true</AllowsRangeStrike>
			<Defense>450</Defense>
			<ExtraCityHitPoints>13</ExtraCityHitPoints>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>9</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_MILITARY_BASE_UP</Type>
			<BuildingClass>BUILDINGCLASS_MILITARY_BASE_UP</BuildingClass>
			<Cost>500</Cost>
			<GoldMaintenance>2</GoldMaintenance>
			<PrereqTech>TECH_REPLACEABLE_PARTS</PrereqTech>
			<Help>TXT_KEY_BUILDING_MILITARY_BASE_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_MILITARY_BASE_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_MILITARYBASE_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_MILITARY_BASE_UP_STRATEGY</Strategy>
			<ArtDefineTag>MILITARY BASE</ArtDefineTag>
			<NukeImmune>true</NukeImmune>
			<MinAreaSize>-1</MinAreaSize>
			<ConquestProb>66</ConquestProb>
			<AllowsRangeStrike>true</AllowsRangeStrike>
			<Defense>600</Defense>
			<ExtraCityHitPoints>13</ExtraCityHitPoints>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<DisplayPosition>2</DisplayPosition>
			<NeverCapture>true</NeverCapture>
			<PortraitIndex>10</PortraitIndex>
		</Row>

		<!--  Sciences  -->
		<Row>
			<Type>BUILDING_LIBRARY_UP</Type>
			<BuildingClass>BUILDINGCLASS_LIBRARY_UP</BuildingClass>
			<FreeStartEra>ERA_INDUSTRIAL</FreeStartEra>
			<Cost>75</Cost>
			<GoldMaintenance>1</GoldMaintenance>
			<PrereqTech>TECH_WRITING</PrereqTech>
			<Help>TXT_KEY_BUILDING_LIBRARY_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_LIBRARY_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_LIBRARY_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_LIBRARY_UP_STRATEGY</Strategy>
			<ArtDefineTag>ART_DEF_BUILDING_LIBRARY</ArtDefineTag>
			<MinAreaSize>-1</MinAreaSize>
			<ConquestProb>66</ConquestProb>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<PortraitIndex>11</PortraitIndex>
		</Row>
		<Row>
			<Type>BUILDING_UNIVERSITY_UP</Type>
			<BuildingClass>BUILDINGCLASS_UNIVERSITY_UP</BuildingClass>
			<Cost>160</Cost>
			<GoldMaintenance>2</GoldMaintenance>
			<PrereqTech>TECH_EDUCATION</PrereqTech>
			<Help>TXT_KEY_BUILDING_UNIVERSITY_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_UNIVERSITY_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_UNIVERSITY_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_UNIVERSITY_UP_STRATEGY</Strategy>
			<ArtDefineTag>ART_DEF_BUILDING_UNIVERSITY</ArtDefineTag>
			<SpecialistType>SPECIALIST_SCIENTIST</SpecialistType>
			<SpecialistCount>1</SpecialistCount>
			<MinAreaSize>-1</MinAreaSize>
			<ConquestProb>66</ConquestProb>
			<HurryCostModifier>15</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<PortraitIndex>13</PortraitIndex>
		</Row>
		

		<!--  Prod  -->
		<Row>
			<Type>BUILDING_WORKSHOP_UP</Type>
			<BuildingClass>BUILDINGCLASS_WORKSHOP_UP</BuildingClass>
			<FreeStartEra>ERA_INDUSTRIAL</FreeStartEra>
			<Cost>120</Cost>
			<GoldMaintenance>2</GoldMaintenance>
			<PrereqTech>TECH_METAL_CASTING</PrereqTech>
			<Help>TXT_KEY_BUILDING_WORKSHOP_UP_STRATEGY</Help>
			<Description>TXT_KEY_BUILDING_WORKSHOP_UP</Description>
			<Civilopedia>TXT_KEY_CIV5_BUILDINGS_WORKSHOP_TEXT</Civilopedia>
			<Strategy>TXT_KEY_BUILDING_WORKSHOP_UP_STRATEGY</Strategy>
			<ArtDefineTag>ART_DEF_BUILDING_FORGE</ArtDefineTag>
			<SpecialistType>SPECIALIST_ENGINEER</SpecialistType>
			<SpecialistCount>1</SpecialistCount>
			<MinAreaSize>-1</MinAreaSize>
			<ConquestProb>66</ConquestProb>
			<HurryCostModifier>25</HurryCostModifier>
			<IconAtlas>BW_ATLAS_1</IconAtlas>
			<PortraitIndex>28</PortraitIndex>
		</Row>
	<!-- END -->
	</Buildings>
	<Building_ClassesNeededInCity>
	<!-- BUILDING UPGRADE SYSTEM -->
	<!-- START -->
		<!--  Cultural  -->
		<Row>
			<BuildingType>BUILDING_MONUMENT_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_MONUMENT</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_AMPHITHEATER_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_AMPHITHEATER</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_OPERA_HOUSE_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_OPERA_HOUSE</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_MUSEUM_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_MUSEUM</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_BROADCAST_TOWER_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_BROADCAST_TOWER</BuildingClassType>
		</Row>
		
		<!--  Growth  -->
		<Row>
			<BuildingType>BUILDING_GRANARY_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_GRANARY</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_AQUEDUCT_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_AQUEDUCT</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_HOSPITAL_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_HOSPITAL</BuildingClassType>
		</Row>

		
		<!--  Military  -->
		<Row>
			<BuildingType>BUILDING_BARRACKS_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_BARRACKS</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_ARMORY_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_ARMORY</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_MILITARY_ACADEMY_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_MILITARY_ACADEMY</BuildingClassType>
		</Row>

		

		<!--  Faith  -->
		<Row>
			<BuildingType>BUILDING_SHRINE_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_SHRINE</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_TEMPLE_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_TEMPLE</BuildingClassType>
		</Row>
		
		<!--  City Def  -->
		<Row>
			<BuildingType>BUILDING_WALLS_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_WALLS</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_CASTLE_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_CASTLE</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_ARSENAL_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_ARSENAL</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_MILITARY_BASE_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_MILITARY_BASE</BuildingClassType>
		</Row>

		<!--  Sciences  -->
		<Row>
			<BuildingType>BUILDING_LIBRARY_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_LIBRARY</BuildingClassType>
		</Row>
		<Row>
			<BuildingType>BUILDING_UNIVERSITY_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_UNIVERSITY</BuildingClassType>
		</Row>


		<!--  Prod  -->
		<Row>
			<BuildingType>BUILDING_WORKSHOP_UP</BuildingType>
			<BuildingClassType>BUILDINGCLASS_WORKSHOP</BuildingClassType>
		</Row>
	<!-- END -->
	</Building_ClassesNeededInCity>
	<Building_DomainFreeExperiences>
	<!-- BUILDING UPGRADE SYSTEM -->
	<!-- START -->
		<!--  Military  -->
		<Row>
			<BuildingType>BUILDING_BARRACKS_UP</BuildingType>
			<DomainType>DOMAIN_LAND</DomainType>
			<Experience>7</Experience>
		</Row>
		<Row>
			<BuildingType>BUILDING_BARRACKS_UP</BuildingType>
			<DomainType>DOMAIN_SEA</DomainType>
			<Experience>7</Experience>
		</Row>
		<Row>
			<BuildingType>BUILDING_BARRACKS_UP</BuildingType>
			<DomainType>DOMAIN_AIR</DomainType>
			<Experience>7</Experience>
		</Row>
			
		<Row>
			<BuildingType>BUILDING_ARMORY_UP</BuildingType>
			<DomainType>DOMAIN_LAND</DomainType>
			<Experience>7</Experience>
		</Row>
		<Row>
			<BuildingType>BUILDING_ARMORY_UP</BuildingType>
			<DomainType>DOMAIN_SEA</DomainType>
			<Experience>7</Experience>
		</Row>
		<Row>
			<BuildingType>BUILDING_ARMORY_UP</BuildingType>
			<DomainType>DOMAIN_AIR</DomainType>
			<Experience>7</Experience>
		</Row>
		<Row>
			<BuildingType>BUILDING_MILITARY_ACADEMY_UP</BuildingType>
			<DomainType>DOMAIN_LAND</DomainType>
			<Experience>7</Experience>
		</Row>
		<Row>
			<BuildingType>BUILDING_MILITARY_ACADEMY_UP</BuildingType>
			<DomainType>DOMAIN_SEA</DomainType>
			<Experience>7</Experience>
		</Row>
		<Row>
			<BuildingType>BUILDING_MILITARY_ACADEMY_UP</BuildingType>
			<DomainType>DOMAIN_AIR</DomainType>
			<Experience>7</Experience>
		</Row>
	<!-- END -->
	</Building_DomainFreeExperiences>
	<Building_Flavors>
	<!-- BUILDING UPGRADE SYSTEM -->
	<!-- START -->
		<!--  Cultural  -->
		<Row>
			<BuildingType>BUILDING_MONUMENT_UP</BuildingType>
			<FlavorType>FLAVOR_CULTURE</FlavorType>
			<Flavor>10</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_AMPHITHEATER_UP</BuildingType>
			<FlavorType>FLAVOR_CULTURE</FlavorType>
			<Flavor>20</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_OPERA_HOUSE_UP</BuildingType>
			<FlavorType>FLAVOR_CULTURE</FlavorType>
			<Flavor>35</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_MUSEUM_UP</BuildingType>
			<FlavorType>FLAVOR_CULTURE</FlavorType>
			<Flavor>40</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_BROADCAST_TOWER_UP</BuildingType>
			<FlavorType>FLAVOR_CULTURE</FlavorType>
			<Flavor>50</Flavor>
		</Row>


		<!--  Growth  -->
		<Row>
			<BuildingType>BUILDING_GRANARY_UP</BuildingType>
			<FlavorType>FLAVOR_GROWTH</FlavorType>
			<Flavor>18</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_AQUEDUCT_UP</BuildingType>
			<FlavorType>FLAVOR_GROWTH</FlavorType>
			<Flavor>40</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_AQUEDUCT_UP</BuildingType>
			<FlavorType>FLAVOR_SCIENCE</FlavorType>
			<Flavor>10</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_HOSPITAL_UP</BuildingType>
			<FlavorType>FLAVOR_GROWTH</FlavorType>
			<Flavor>35</Flavor>
		</Row>



		<!--  Military  -->
		<Row>
			<BuildingType>BUILDING_BARRACKS_UP</BuildingType>
			<FlavorType>FLAVOR_MILITARY_TRAINING</FlavorType>
			<Flavor>20</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_ARMORY_UP</BuildingType>
			<FlavorType>FLAVOR_MILITARY_TRAINING</FlavorType>
			<Flavor>20</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_MILITARY_ACADEMY_UP</BuildingType>
			<FlavorType>FLAVOR_MILITARY_TRAINING</FlavorType>
			<Flavor>20</Flavor>
		</Row>

		<!--  Faith  -->
		<Row>
			<BuildingType>BUILDING_SHRINE_UP</BuildingType>
			<FlavorType>FLAVOR_RELIGION</FlavorType>
			<Flavor>25</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_TEMPLE_UP</BuildingType>
			<FlavorType>FLAVOR_RELIGION</FlavorType>
			<Flavor>40</Flavor>
		</Row>

		<!--  City Def  -->
		<Row>
			<BuildingType>BUILDING_WALLS_UP</BuildingType>
			<FlavorType>FLAVOR_CITY_DEFENSE</FlavorType>
			<Flavor>20</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_CASTLE_UP</BuildingType>
			<FlavorType>FLAVOR_CITY_DEFENSE</FlavorType>
			<Flavor>25</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_ARSENAL_UP</BuildingType>
			<FlavorType>FLAVOR_CITY_DEFENSE</FlavorType>
			<Flavor>25</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_MILITARY_BASE_UP</BuildingType>
			<FlavorType>FLAVOR_CITY_DEFENSE</FlavorType>
			<Flavor>30</Flavor>
		</Row>

		<!--  Sciences  -->
		<Row>
			<BuildingType>BUILDING_LIBRARY_UP</BuildingType>
			<FlavorType>FLAVOR_SCIENCE</FlavorType>
			<Flavor>35</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_LIBRARY_UP</BuildingType>
			<FlavorType>FLAVOR_MILITARY_TRAINING</FlavorType>
			<Flavor>5</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_UNIVERSITY_UP</BuildingType>
			<FlavorType>FLAVOR_SCIENCE</FlavorType>
			<Flavor>35</Flavor>
		</Row>


		<!--  Prod  -->
		<Row>
			<BuildingType>BUILDING_WORKSHOP_UP</BuildingType>
			<FlavorType>FLAVOR_GROWTH</FlavorType>
			<Flavor>5</Flavor>
		</Row>
		<Row>
			<BuildingType>BUILDING_WORKSHOP_UP</BuildingType>
			<FlavorType>FLAVOR_PRODUCTION</FlavorType>
			<Flavor>30</Flavor>
		</Row>
	<!-- END -->
	</Building_Flavors>
	<Building_YieldChanges>
	<!-- BUILDING UPGRADE SYSTEM -->
	<!-- START -->
		<!--  Cultural  -->
		<Row>
			<BuildingType>BUILDING_MONUMENT_UP</BuildingType>
			<YieldType>YIELD_CULTURE</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<BuildingType>BUILDING_AMPHITHEATER_UP</BuildingType>
			<YieldType>YIELD_CULTURE</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<BuildingType>BUILDING_OPERA_HOUSE_UP</BuildingType>
			<YieldType>YIELD_CULTURE</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<BuildingType>BUILDING_MUSEUM_UP</BuildingType>
			<YieldType>YIELD_CULTURE</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<BuildingType>BUILDING_BROADCAST_TOWER_UP</BuildingType>
			<YieldType>YIELD_CULTURE</YieldType>
			<Yield>1</Yield>
		</Row>

		<!--  Growth  -->
		<Row>
			<BuildingType>BUILDING_GRANARY_UP</BuildingType>
			<YieldType>YIELD_FOOD</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<BuildingType>BUILDING_HOSPITAL_UP</BuildingType>
			<YieldType>YIELD_FOOD</YieldType>
			<Yield>2</Yield>
		</Row>

		<!--  Faith  -->
		<Row>
			<BuildingType>BUILDING_SHRINE_UP</BuildingType>
			<YieldType>YIELD_FAITH</YieldType>
			<Yield>1</Yield>
		</Row>
		<Row>
			<BuildingType>BUILDING_TEMPLE_UP</BuildingType>
			<YieldType>YIELD_FAITH</YieldType>
			<Yield>1</Yield>
		</Row>
	<!-- END -->
	</Building_YieldChanges>
	<Building_YieldChangesPerPop>
	<!-- BUILDING UPGRADE SYSTEM -->
	<!-- START -->
		<!--  Sciences  -->
		<Row>
			<BuildingType>BUILDING_LIBRARY_UP</BuildingType>
			<YieldType>YIELD_SCIENCE</YieldType>
			<Yield>25</Yield>
		</Row>
	<!-- END -->
	</Building_YieldChangesPerPop>
	<Building_YieldModifiers>
	<!-- BUILDING UPGRADE SYSTEM -->
	<!-- START -->
		<!--  Sciences  -->
		<Row>
			<BuildingType>BUILDING_UNIVERSITY_UP</BuildingType>
			<YieldType>YIELD_SCIENCE</YieldType>
			<Yield>17</Yield>
		</Row>

		<!--  Prod  -->
		<Row>
			<BuildingType>BUILDING_WORKSHOP_UP</BuildingType>
			<YieldType>YIELD_PRODUCTION</YieldType>
			<Yield>5</Yield>
		</Row>
	<!-- END -->
	</Building_YieldModifiers>
```
