# notification-service
A cloud notification service that allows users with premium subscription to receive edge event notifications via email , sms and other channels.

Currently ambianic users who are comfortable with YAML configuration files are able to configure their edge devices to send notifications via apprise. [Here is the documentation](https://docs.ambianic.ai/users/configure/#notification-settings) how to do it. This route requires users to obtain third party cloud notification service credentials (e.g. gmail app password) and enter them in ambianic edge `config.yaml`.

Alternatively, users can use a premium subscription option and skip the manual steps of third party service management and yaml configuration. Premium subscription covers the cost of managing and using thrid party cloud notification servies on their behalf.

The following diagram illustrates the high level architecture of the Ambianic notification service.

[![notification-flow](https://user-images.githubusercontent.com/2234901/112359136-f5b60400-8c9e-11eb-8489-4025fa76fe00.png)](https://drive.google.com/file/d/1VRykNIOxOAyraMdy13iRd-u-zPlCPbTT/view?usp=sharing)


The following flow illustrates how an Ambianic Edge device obtains authorization token to use the premium Ambianic notification service. Detailed explanation of the flow available [here](https://auth0.com/docs/flows/device-authorization-flow).

[![auth-sequence-device-auth](https://user-images.githubusercontent.com/2234901/112358395-4f69fe80-8c9e-11eb-949b-778dca839009.png)](https://auth0.com/docs/flows/device-authorization-flow)
