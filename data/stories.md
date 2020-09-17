## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot


## test
* greet
  - utter_greet
* test
  - test_custom_action

## book room1withnumber
* room_query{"book":"to book"}
  - utter_roomquery
* room_number{"room_number":"2 rooms"}
  - utter_roomtypequery
* simple
  - utter_simpleroom


## book room1
* room_query{"book":"to book","room_number":"a room"}
  - utter_roomtypequery
* simple
  - utter_simpleroom

## book room2withnumber
* room_query{"book":"to book"}
  - utter_roomquery
* room_number{"room_number":"2 rooms"}
  - utter_roomtypequery
* deluxe
  - utter_deluxeroom

## book room2
* room_query{"room_number":"a room","book":"to book"}
  - utter_roomtypequery
* deluxe
  - utter_deluxeroom

## clean now
* cleanroom_query
  - utter_cleantimequery
* clean_now
  - utter_cleannow

## clean later
* cleanroom_query
  - utter_cleantimequery
* clean_later
  - utter_cleanlater