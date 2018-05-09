# WIP

# AWS Message broker

A message broker is a pub/sub service used to send and receive messages between devices and apps. 

Each message is published to a topic, and the message broker then delivers those messages to all of the topic's subscribers. An useful analogy is a Slack channel: Each Slack channel is like a topic, and members can send (publish) messages to other members of the channel (subscribers).

- diagram

The messaging protocol we will be using is MQTT, specifically version 3.1.1. In more detailed activities, you will use websockets to send and receive MQTT messages, but for now you'll will use the AWS dashboard to communicate with the "Makers" topic we've set up.


# Activity steps

1. Sign into AWS IoT cloud with your maker account (you should have received credentials via Slack, if not ask @nuclearnic or @dan for help)

2. Subscribe to the "makersPrep" topic and then publish a message to complete the activity
a) open the pub sub page
- Navigate to AWS IoT page
- Click "test" in the sidebar

b) subscribe
- Topic name: "makersPrep"
- Auto format JSON

c) publish
- Topic name: "makersPrep"
- Message: a JSON object with attributes "name" as your full name, "completed_prep" as true, and an optional "message" string.

d) If you did everything correctly, you will see your message appear in the topic message stream on the same page, and (something will happen in slack).

If you need help, contact a make master!


# Dan todo:
- Screenshots
- Slack bot for checking messages
- IAM user setup


# Extra resources
- https://docs.aws.amazon.com/iot/latest/developerguide/iot-message-broker.html

