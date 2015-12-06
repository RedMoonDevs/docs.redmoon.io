Version
=======

## Command Name
`version`

## Usage 
The `version` command is used to check the version of the API. The current version is 0.1 (aka. Armadillo).

## Arguments
None.

## Components
Component | Type | Details
--- | --- | ---
`major` | int | Major Version (the `x` in `x.y`)
`minor` | int | Minor Version (the `y` in `x.y`)
`nameCode` | String | NameCode for the current version. 

## Example
```json
{
	"major": 1,
	"minor": 0,
	"nameCode": "Armadillo"
}```