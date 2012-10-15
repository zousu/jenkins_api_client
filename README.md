jenkins_api_client
==================

Client libraries for communicating with a Jenkins CI server

==== Sample Usage:

Install jenkins_api_client by `sudo gem install jenkins_api_client`

require 'jenkins_api_client'

client = JenkinsApi::Client.new(:server_ip => '0.0.0.0', :username => 'somename', :password => 'secret password')
# The following call will return all jobs matching 'Testjob'
puts client.job.list("^Testjob")