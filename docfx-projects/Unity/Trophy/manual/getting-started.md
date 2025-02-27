# Getting Started
Here is complete guideline for onboarding with trophy score system.

## Setup the definitions
In order to have score in the game what we need is called Score definiiton.

**Here are the steps to setup a score definiiton:**
1. In project window, choose Create > Trophy > Score Definition
2. In the Score Definition inspector define unique key
3. Go to trophy settings using Tools > Rocketshift Studio > Trophy > Settings
4. In the settings editor's score definition array add a entry and assign the definition in there.

## Metadata & Format
When it comes to showing scores to the user it requires some additional properties to do that. Here are information about the properties
![Metadata Section](../images/getting-started/metadata-section.png)

| **Property** 	| **Description** 	|
|---	|---	|
| Name 	| The display name of the score which can be shown along with the score value when using {0} in format 	|
| Icon 	| A sprite which can be shown along with using the appropriate score icon element based on the use case 	|
| Default Format 	| The string format for the score text to use when displaying it to the user.<br><br>{0} Represents the name of the score<br>{1} Represents the value of the score<br>{2} Represents the type of the score<br><br>e.g. {2} {0}: {0:F2}<br>Result: Type Name: 0.00 	|
| Format "As Time" 	| Tells the definition to handle format string as time format<br>such as {1:mm\.ss} for 140 seconds will be shown as 02:20<br><br>For more information about time format please refer to [**Microsoft Documentation**](https://learn.microsoft.com/en-us/dotnet/standard/base-types/custom-timespan-format-strings) 	|


## Modifiers
Modifiers processes value before applying to the score. Here are information about the properties
![Modifiers Section](../images/getting-started/modifiers-section.png)

| **Property** 	| **Description** 	|
|---	|---	|
| Limits Flags 	| Defines how the limit should effect the score value 	|
| Flow Restriction  | Defines which direction has to be restricted 	|
| Whole Value 	| On checked will round floating point values to nearest integer 	|
| Absolute Value    | On checked will convert negetive values to positive 	|

