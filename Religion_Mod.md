# Religion mod

## CIV5Beliefs

```xml
<!-- weak beliefs balanced -->
		<Row><!-- B2 -->
			<Type>BELIEF_GOD_WAR</Type>
			<MaxDistance>5</MaxDistance><!-- DEFAULT 4 -->
			<FaithFromKills>80</FaithFromKills><!-- DEFAULT 50 -->
		</Row>
		<Row><!-- B2 -->
			<Type>BELIEF_GODDESS_LOVE</Type>
			<MinPopulation>6</MinPopulation>
			<HappinessPerCity>2</HappinessPerCity><!-- DEFAULT 1 -->
		</Row>
		<Row><!-- B2 -->
			<Type>BELIEF_INITIATION_RITES</Type>
			<GoldPerFirstCityConversion>200</GoldPerFirstCityConversion><!-- DEFAULT 100 -->
		</Row>
		<Row><!-- B2 -->
			<Type>BELIEF_MISSIONARY_ZEAL</Type>
			<MissionaryStrengthModifier>50</MissionaryStrengthModifier><!-- DEFAULT 25 -->
		</Row>
		<Row>
			<Type>BELIEF_CEREMONIAL_BURIAL</Type>
			<HappinessPerFollowingCity>1</HappinessPerFollowingCity><!-- 0.5 FOR BNW -->
		</Row>
		<Row>
			<Type>BELIEF_CHURCH_PROPERTY</Type>
			<GoldPerFollowingCity>3</GoldPerFollowingCity><!-- DEFAULT 2 -->
		</Row>
		<Row>
			<Type>BELIEF_SACRED_WATERS</Type>
			<RiverHappiness>2</RiverHappiness><!-- DEFAULT 1 -->
		</Row>
		<Row>
			<Type>BELIEF_INTERFAITH_DIALOGUE</Type>
			<SciencePerOtherReligionFollower>25</SciencePerOtherReligionFollower><!-- DEFAULT 10 -->
		</Row>
		<Row>
			<Type>BELIEF_RELIQUARY</Type>
			<GreatPersonExpendedFaith>150</GreatPersonExpendedFaith><!-- DEFAULT 50 -->
		</Row>
		<Row>
			<Type>BELIEF_PEACE_LOVING</Type>
			<HappinessPerXPeacefulForeignFollowers>4</HappinessPerXPeacefulForeignFollowers><!-- DEFAULT 8 -->
		</Row>
		<Row>
			<Type>BELIEF_RELIGIOUS_SETTLEMENTS</Type>
			<PlotCultureCostModifier>-35</PlotCultureCostModifier><!-- DEFAULT -15 -->
		</Row>
	<Belief_BuildingClassYieldChanges>
		<Row>
			<BeliefType>BELIEF_ANCESTOR_WORSHIP</BeliefType>
			<YieldChange>2</YieldChange><!-- DEFAULT 1 -->
		</Row>
		<Row>
			<BeliefType>BELIEF_CHORAL_MUSIC</BeliefType>
			<BuildingClassType>BUILDINGCLASS_TEMPLE</BuildingClassType>
			<YieldType>YIELD_CULTURE</YieldType>
			<YieldChange>3</YieldChange><!-- DEFAULT 2 -->
		</Row>
		<Row>
			<BeliefType>BELIEF_LITURGICAL_DRAMA</BeliefType>
			<YieldChange>2</YieldChange><!-- DEFAULT 1 -->
		</Row>
	</Belief_BuildingClassYieldChanges>
	<Belief_CityYieldChanges>
		<Row>
			<BeliefType>BELIEF_GOD_CRAFTSMEN</BeliefType>
			<YieldType>YIELD_PRODUCTION</YieldType>
			<Yield>2</Yield><!-- DEFAULT 1 -->
		</Row>
	</Belief_CityYieldChanges>
	<Belief_TerrainYieldChanges>
		<Row>
			<BeliefType>BELIEF_DANCE_AURORA</BeliefType>
			<Yield>2</Yield><!-- DEFAULT 1 -->
		</Row>
	</Belief_TerrainYieldChanges>
	<Belief_YieldChangePerXForeignFollowers>
		<Row>
			<BeliefType>BELIEF_WORLD_CHURCH</BeliefType>
			<YieldType>YIELD_CULTURE</YieldType>
			<ForeignFollowers>4</ForeignFollowers><!-- DEFAULT 5 -->
		</Row>
	</Belief_YieldChangePerXForeignFollowers>
```