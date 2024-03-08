Tn t
By default the alpine service replica was set to 1, meaning if that node goes down the service will not be available
To metigate that, we update the replica to 4. meaning if one node goes down the service will still be available
we also check the logs using the command docker service logs alpine to ensure it is pinging www.google.com
finally when we've checked all is fine, decided to roll it back to default setting.
