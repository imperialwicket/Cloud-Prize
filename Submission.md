## Which Categories Best Fit Your Submission and Why?

Best Contribution to Operational Tools, Availability, and Manageability or Best Usability Enhancement

I aim to reduce entry barriers and ease initial setup for new users. If we can collectively enhance standards and establish best practices along the way, that is even better.

## Describe your Submission

I am generating AMIs that aim to be deploy-ready with minimal alterations by an end user. The idea is that someone should not need to ssh into the server to get a pre-built war installed and running. 

I plan to support these AMIs with puppet modules and potentially full manifests for generation. However, the core focus is currently puppet modules for the specific software solution and pre-baked AMIs.

I am also creating Hubot scripts for interfacing with Asgard APIs and launching Asgard (plus Asgard-complimenting) instances via Hubot.

## Provide Links to Github Repo's for your Submission

### Hubot-asgard

 - [Hubot-asgard intro post](http://imperialwicket.com/asgard-and-hubot-simplified-ami-deployment-to-aws)
 - [hubot-asgard (github)](https://github.com/imperialwicket/hubot-asgard)
 - [hubot-asgard (npm)](https://npmjs.org/package/hubot-asgard)

Hubot-asgard is a Hubot plugin for viewing status and managing standard Asgard tasks via Hubot. It is bundled with asgard-launcher which supports the launch, custom ami generation, security group controls, and terminate capabilities for an Asgard instance using the Amazon [aws-sdk-js](https://github.com/aws/aws-sdk-js).

Install hubot-asgard in an existing Hubot directory by updating package.json and running `npm install`; add 'hubot-asgard' to your external-scripts.json file and you're ready to go. After configuring AWS creds for Hubot, `asgard-launcher run` starts an Asgard instance for you. More details in the project readme.

### Hubot-edda

 - [hubot-edda (github)](https://github.com/imperialwicket/hubot-edda)

Hubot-edda is a Hubot plugin for interacting with the Edda api. Hubot-edda will not be polished prior to Cloud-Prize close, but I plan to wrap most of the api and support stored field selectors and user-specific queries so that it is easy for users to get quick access to this data via Hubot.

### AMIs and Puppet Modules

I plan to collect announcements at [imperialwicket.com](http://imperialwicket.com/tag/netflix). I will keep an updated list of the latest releases here, as well as information regarding related repositories.

[netflix-oss puppet manifest samples](https://github.com/imperialwicket/netflixoss-puppet-manifest-samples) - A collection of spartan manifests for using these puppet modules.

#### Asgard

[puppet-asgard](https://github.com/imperialwicket/puppet-asgard)

##### Asgard: Ubuntu 12.04LTS -
  - US-East (VA): ami-acadd2c5
  - US-East (VA): ami-11453178 (deprecated)
  - US-East (VA): ami-f7e28b9e (deprecated)
  - US-West (OR): ami-dd7be8ed
  - US-West (OR): ami-233fae13 (deprecated)
  - US-West (OR): ami-a5c25395 (deprecated)

##### Asgard: Amazon Linux - 
  - US-East (VA): ami-90add2f9
  - US-East (VA): ami-0347336a (deprecated)
  - US-East (VA): ami-17761e7e (deprecated)
  - US-West (OR): ami-c17be8f1
  - US-West (OR): ami-753fae45 (deprecated)
  - US-West (OR): ami-1bfe6f2b (deprecated)

