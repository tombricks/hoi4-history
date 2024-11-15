# Localization Formatters

## Table of Content

* [advisor_desc](#advisor_desc)
* [building_state_modifier](#building_state_modifier)
* [character_name](#character_name)
* [country_culture](#country_culture)
* [idea_desc](#idea_desc)
* [idea_name](#idea_name)
* [tech_effect](#tech_effect)

## character_name
The character_name formatter gets the name of the character.

### Example:
```
custom_effect_tooltip = character_name|hjalmar_schacht
```


## country_culture
The country_culture formatter formats the string using the country's cultural override (`TAG_token`) if it exists,
otherwise the generic version (`token`).

### Localization Scope Object
The formatter requires the following Localization Scope Objets to be defined:
* `Country` - The country that the idea is associated with.

### Example
```
custom_effect_tooltip = country_culture|generic_tank_organisation
```


## idea_name
The idea_name formatter formats gets the name for the idea.

### Localization Scope Object
The formatter requires the following Localization Scope Objects to be defined:
* `Country` - The country that the idea is associated with.

### Example
```
custom_effect_tooltip = idea_name|canadian_pacific_railway
```


## advisor_desc
The advisor_desc formatter gets the description for the advisor.

### Localization Scope Object
The formatter requires the following Localization Scope Objets to be defined:
* `Country` - The country that the idea is associated with.

### Example
```
custom_effect_tooltip = advisor_desc|hjalmar_schacht
```


## tech_effect
The tech_effect formatter gets the effect of finishing a technology.

### Localization Scope Object
The formatter requires the following Localization Scope Objects to be defined:
* `Country` - The country that the tech is associated with.

### Example
```
custom_effect_tooltip = tech_effect|early_transport_plane
```


## idea_desc
The idea_desc formatter gets the description for the idea.

### Localization Scope Object
The formatter requires the following Localization Scope Objects to be defined:
* `Country` - The country that the idea is associated with.

### Example
```
custom_effect_tooltip = idea_desc|canadian_pacific_railway
```


## building_state_modifier
The building_state_modifier gets the state modifiers for the provided building template and the provided scope.

The formatter takes special care of the following parameters:
- INDENT: The indent to be added to all lines of the state modifier description (including header line).

### Example:
```
custom_effect_tooltip = building_state_modifier|dam
```


