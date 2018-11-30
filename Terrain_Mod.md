# Terrain Mod

## JEWELRY, PORCELAIN, MARBLE

Add in *CIV5Resources*

```xml
		<Row>
			<Type>RESOURCE_MARBLE</Type>
			<CivilizationType>CIVILIZATION_SIAM</CivilizationType><!-- MOD -->
		</Row>
		<Row>
			<Type>RESOURCE_IVORY</Type>
			<CivilizationType>CIVILIZATION_SIAM</CivilizationType><!-- MOD -->
		</Row>
```

Add in *CIV5Resources_Inherited_Expansion2*

```xml
    <InsertOrAbort>
      <Type>RESOURCE_JEWELRY</Type>
      <CivilizationType>CIVILIZATION_SIAM</CivilizationType><!-- MOD -->
    </InsertOrAbort>
    <InsertOrAbort>
      <Type>RESOURCE_PORCELAIN</Type>
      <CivilizationType>CIVILIZATION_SIAM</CivilizationType><!-- MOD -->
    </InsertOrAbort>
```

## Developable oasis and atoll

Mod in *CIV5Features*

```xml
	<Features>
		<Row>
			<Type>FEATURE_OASIS</Type>
			<NoImprovement>false</NoImprovement><!-- true -->
		</Row>
		<Row>
			<Type>FEATURE_ATOLL</Type>
			<NoImprovement>false</NoImprovement><!-- true -->
		</Row>
	</Features>
```

## REMOVE JUNGLE GRANT PRODUCTION

Mod in *CIV5Builds*

```xml
	<BuildFeatures>
			<FeatureType>FEATURE_JUNGLE</FeatureType>
			<Production>30</Production><!-- MOD -->
	</BuildFeatures>
```
