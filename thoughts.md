# thoughts about this project
## Naming convention:
In this document I'm referring to Tasker terms as <tasker_term> to prevent any confusion.

## rulesets
There are 2 types of rulesets: 
  1. actions, such as:
      * set ringvolume based on media volume
      * GamingMode
      * ...
  2. the (poorly-named) profiles, such as:
      * Home
      * Work
      * Meeting
      * Outdoor
      * Sleep
   

## general concept
### <1st Setup>
  - set "constants" (datatype doesn't exist in Tasker afaik but it makes development a lot easier)
  - set default values
  - check & load config json
  - generate vars based on config, fallback to default if necessary
  - check & load profile_rulesets json
  - generate action & trigger vars for rulesets
  - enable <tasks> based on trigger/action vars
  - enable <profiles> which are required by trigger vars
  - enable deamon(s)
