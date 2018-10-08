# **tagpro-comp-teams**

Team and Jersey definitions used by both [STATS userscript](https://github.com/Poeticalto/tagpro-comp-stats) and [tagpro.eu website](https://tagpro.eu/?teams).

teams.json holds information about each team and the corresponding abbreviation. It is formatted as a json object where each league is a property. Each league contains three arrays. The first array is the raw list. This is the list that will show up under the Red and Blue team names. The second array contains header labels. These labels help to distinguish teams based on some qualification like server or conference. The third array is the abbreviation list. This array should be the exact same size as the first array, where each position corresponds to the abbreviation of the team in the first array.

In addition, there is a Leagues property which contains the list of all leagues in the json. This is used to populate the autoscore league selector at the top of the group page.

jerseys.json holds the raw imgur IDs for the jerseys of each team. It is formatted as a json object where each team abbreviation is a property. Abbreviations are sorted alphabetically, with the exception of NLTP (with league identifiers A and B) because league rules mandate the same abbreviation for both teams. Each abbreviation contains a single array with two strings and four numbers corresponding to the raw imgur IDs of the jerseys and the transparency of each jersey. The first string is the red jersey and the second string is the blue jersey. The first number corresponds to the transparency of the actual ball with the red jersey and the second number corresponds to the transparency of the actual ball with the blue jersey. The third number corresponds to the transparency of the red jersey and the second number corresponds to the transparency of the blue jersey. 1 is the default value while 0 is fully transparent.

For examples on how to format each json, consult the teams.json and jerseys.json above.
