# Cisco Sparky

Cisco Sparky is a Speech-enabled(optional) web chat application that utilizes several different Cisco Contact Center APIs. 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

```
To fully implement all the features of Sparky, you will need access to an AI facility (Google DialogFlow is the default), Cisco UCCE/PCCE ECE Chat and Email subsystem
and Cisco Remote Expert Mobile. All versioning should be at 11.6. 
```

### Installing

This project is a Javascript project and is embedded within the fictitious Cumulus Finance Company sample website. This project can be installed directly into the 
'webapps' folder on Tomcat or can be 'warified' (.war) and run on a webserver. 

You will need to 'Edit' certain parts of the .js files to insert your own configurations for ECE, DialogFlow and Remote Expert Mobile. The sections that
need configuration will be marked within comments.

## Testing

Simply navigate to the Cumulus (or any other website you have embedded this project into) website. To start the BOT, navigate to the 'about us' page which should
engage the chat and it will appear in the lower right portion of the screen.

### Commands in use

This project will use keywords that you have programmed into your AI application. The BOT in this example will key in on the following words to trigger interactions
with the Cisco ECE application:
- 'Loan', can i speak with a loan specialist... any phrase that has the 'loan' word in it. This will trigger a Chat session with an agent.
- 'Cobrowse', when this word is inputted, the system will launch the 'index_1.html' page to initiate a co-browse session.
- 'Goodbye', Typing this word will end the Chat session for the customer side. An agent can also terminate the session

### Web Chat Buttons

Within the application, there are 3 buttons located on the top of the Chat window. These buttons provide the following functionality:

- 'Up-Arrow', This button is used to transfer a file from the customer to the Agent
- 'Microphone', This button is used to trigger voice commands
- 'Video Play', This button will trigger an RE Mobile video call to the agent

## Distribution

This project will be distributed to DevNet and Github

## Authors

* **Frank Kicenko** - *Initial work* - [Cumulus Finance](https://github.com//fkicenko/CumulusFinance)

## License

This project is licensed under various licenses, see file for details

## Acknowledgments

* Hat tip to anyone who's code was used
* Inspiration
* etc

