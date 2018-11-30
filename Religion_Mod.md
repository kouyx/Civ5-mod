# Religion mod

## Balance weak beliefs

Mod in *CIV5Beliefs*

```xml
<!-- weak beliefs balanced -->
		<Row><!-- B2 -->
			<Type>BELIEF_GOD_WAR</Type>
			<MaxDistance>5</MaxDistance><!-- 4 -->
			<FaithFromKills>80</FaithFromKills><!-- 50 -->
		</Row>
		<Row><!-- B2 -->
			<Type>BELIEF_GODDESS_LOVE</Type>
			<HappinessPerCity>2</HappinessPerCity><!-- 1 -->
		</Row>
		<Row><!-- B2 -->
			<Type>BELIEF_INITIATION_RITES</Type>
			<GoldPerFirstCityConversion>200</GoldPerFirstCityConversion><!-- 100 -->
		</Row>
		<Row><!-- B2 -->
			<Type>BELIEF_MISSIONARY_ZEAL</Type>
			<MissionaryStrengthModifier>50</MissionaryStrengthModifier><!-- 25 -->
		</Row>
		<Row>
			<Type>BELIEF_CEREMONIAL_BURIAL</Type>
			<HappinessPerFollowingCity>1</HappinessPerFollowingCity><!-- 0.5 FOR BNW -->
		</Row>
		<Row>
			<Type>BELIEF_CHURCH_PROPERTY</Type>
			<GoldPerFollowingCity>3</GoldPerFollowingCity><!-- 2 -->
		</Row>
		<Row>
			<Type>BELIEF_SACRED_WATERS</Type>
			<RiverHappiness>2</RiverHappiness><!-- 1 -->
		</Row>
		<Row>
			<Type>BELIEF_INTERFAITH_DIALOGUE</Type>
			<SciencePerOtherReligionFollower>25</SciencePerOtherReligionFollower><!-- 10 -->
		</Row>
		<Row>
			<Type>BELIEF_RELIQUARY</Type>
			<GreatPersonExpendedFaith>150</GreatPersonExpendedFaith><!-- 50 -->
		</Row>
		<Row>
			<Type>BELIEF_PEACE_LOVING</Type>
			<HappinessPerXPeacefulForeignFollowers>4</HappinessPerXPeacefulForeignFollowers><!-- 8 -->
		</Row>
		<Row>
			<Type>BELIEF_RELIGIOUS_SETTLEMENTS</Type>
			<PlotCultureCostModifier>-35</PlotCultureCostModifier><!-- -15 -->
		</Row>
	<Belief_BuildingClassYieldChanges>
		<Row>
			<BeliefType>BELIEF_ANCESTOR_WORSHIP</BeliefType>
			<YieldChange>2</YieldChange><!-- 1 -->
		</Row>
		<Row>
			<BeliefType>BELIEF_CHORAL_MUSIC</BeliefType>
			<BuildingClassType>BUILDINGCLASS_TEMPLE</BuildingClassType>
			<YieldType>YIELD_CULTURE</YieldType>
			<YieldChange>3</YieldChange><!-- 2 -->
		</Row>
		<Row>
			<BeliefType>BELIEF_LITURGICAL_DRAMA</BeliefType>
			<YieldChange>2</YieldChange><!-- 1 -->
		</Row>
	</Belief_BuildingClassYieldChanges>
	<Belief_CityYieldChanges>
		<Row>
			<BeliefType>BELIEF_GOD_CRAFTSMEN</BeliefType>
			<YieldType>YIELD_PRODUCTION</YieldType>
			<Yield>2</Yield><!-- 1 -->
		</Row>
	</Belief_CityYieldChanges>
	<Belief_TerrainYieldChanges>
		<Row>
			<BeliefType>BELIEF_DANCE_AURORA</BeliefType>
			<Yield>2</Yield><!-- 1 -->
		</Row>
	</Belief_TerrainYieldChanges>
	<Belief_YieldChangePerXForeignFollowers>
		<Row>
			<BeliefType>BELIEF_WORLD_CHURCH</BeliefType>
			<YieldType>YIELD_CULTURE</YieldType>
			<ForeignFollowers>4</ForeignFollowers><!-- 5 -->
		</Row>
	</Belief_YieldChangePerXForeignFollowers>
```
