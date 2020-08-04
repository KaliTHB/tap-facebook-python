# tap-facebook
the facebook tapping source


config file variables

{"start_date":"2017-01-01T00:00:00Z",
"account_id":"*****************",
"adset_id":"*************",
"access_token":"*****************"}

properties file 

 The properties file will indicate what streams and fields to replicate from the Facebook Marketing API


state file 

 You can provide JSON file that contains a date for the streams to force the application to only fetch data newer than those dates. If you  omit the file it will fetch all data for the selected streams.

{"ads":"2017-01-01T00:00:00Z",
 "adcreative":"2017-01-01T00:00:00Z",
 "ads_insights":"2017-01-01T00:00:00Z"}


command:

tap-facebook -c config.json -p works/leads.json -s state.json
