# Score Definitions
## Setup
In order to have score in the game what you need is called Score definiiton.

**Here are the steps to setup a score definiiton:**
1. In project window, choose Create > Trophy > Score Definition
2. In the Score Definition inspector define a unique key
3. Go to trophy settings using Tools > Rocketshift Studio > Trophy > Settings
4. In the settings editor's score definitions array add a entry and assign the definition in there.

## Metadata & Format Properties
When it comes to showing scores to the user it requires some additional properties to do that. Here are information about the properties
![Metadata Section](../images/score-definitions/metadata-section.png)

| **Property** 	| **Description** 	|
|---	|---	|
| Name 	| The display name of the score which can be shown along with the score value when using {0} in format 	|
| Icon 	| A sprite which can be shown along with using the appropriate score icon element based on the use case 	|
| Default Format 	| The string format for the score text to use when displaying it to the user.<br><br>{0} Represents the name of the score<br>{1} Represents the value of the score<br>{2} Represents the type of the score<br><br>e.g. {2} {0}: {0:F2}<br>Result: Type Name: 0.00 	|
| Format "As Time" 	| Tells the definition to handle format string as time format<br>such as {1:mm\.ss} for 140 seconds will be shown as 02:20<br><br>For more information about time format please refer to [**Microsoft Documentation**](https://learn.microsoft.com/en-us/dotnet/standard/base-types/custom-timespan-format-strings) 	|


## Modifier Properties
Modifiers processes value before applying to the score. Here are information about the properties
![Modifiers Section](../images/score-definitions/modifiers-section.png)

| **Property** 	| **Description** 	|
|---	|---	|
| Limits Flags 	| Defines how the limit should effect the score value 	|
| Flow Restriction  | Defines which direction has to be restricted 	|
| Whole Value 	| On checked will round floating point values to nearest integer 	|
| Absolute Value    | On checked will convert negetive values to positive 	|


## Save/Load Properties
Defines score's saving and loading preferences
![Save/Load Section](../images/score-definitions/save-and-load-section.png)

| **Property** 	| **Description** 	|
|---	|---	|
| Best Calculation Type | How the best value will be calculated 	|
| Storage Flags  | Which storage will be used for save & load of values 	|

# Leaderboard Definitions

## Setup
In order to post scores to leaderboard what you need is called Leaderboard definiiton.

**Here are the steps to setup a leaderboard definiiton:**
1. In project window, choose Create > Trophy > Leaderoard Definition
2. In the Leaderoard Definition inspector set your leaderboard id. It should be same as the id you have setup in your server

Server View
![Leaderboard ID Cloud](../images/leaderboard-definitions/leaderboard-id-cloud.png)

Inspector View
![Leaderboard ID Definition](../images/leaderboard-definitions/leaderboard-id-definition.png)

3. In definition's score key property use the key of the target score
4. Select the source of value from value source
5. Go to trophy settings using Tools > Rocketshift Studio > Trophy > Settings
6. In the settings editor's leaderboards definitions array add a entry and assign the definition in there.
