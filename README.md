# Structure
* Json Files
  * Competitions:
    * Holds every played match sorted by competition then time
  * Scores
    * Holds every team's score, and their score over time stored in a list
  * Teams
    * Stores every team, and every match they have played.

# Backlog

### Complete
* Create Json manager class
* Create competition class
* Create competition ID system
* Read and compile csvs into jsons
  * Have a json for comps and a json for teams
* Create scoring system
* Print a teams stats nicely
* Show scores over time

### In progress
* Display competitions nicely

### TODO
.
# Sprint Task List
* Implement skills

#### Complete
.
#### In progress
* Create comp class

#### TODO
* Use similar print format from the teams match printing
* Allow multiple comps to be shown at once
* Allow highlighting of certain teams
  * Also implement into the teams class

# Json format:

## Comps:
    {
      "CompName":{
        "Matches":[
          [
            "matchName",
            compId,
            [redScore, blueScore],
            [red1, red2],
            [blue1, blue2],
            "winner"
          ]
        ],
        "Skills": [
          [
            "TeamName",
            [autonScore, driverScore]
          ]
        ]
      }
    }
## Scores:

    {
      "teamNumber": [
        score1,
        score2,
        score3...
      ]
    }

## Teams:

    {
      "teamNumber": {
        "Matches: [
          "referenceToCompsJsonMatchIndex",
        ],
        "Skills": [

        ]
      }
    }


