## Bot Basics

## Enterprise Bot landscape

There are many types of Enterprise Bots.. Optimizers, One-trick Ponies, The Proactive, The Social, The Shield, The Chatty, The Super Bot.

## Bot Framework in the Enterprise

Cloud based abstraction layoer for poular and custom clients or "channels" that support chat

Makes channel-specif logic and nuances transparent to developers

Includes SDKs for Node and C#

Supports enterprise channels such as Skype for Business, Microsoft Teams, and Slack.

No real plans to make Bot Framework available on-premises. Custom implementation is possible, but not worth it.

## Bots and Office 365 (Clients and Data)

2 main parts - Enterprise Clients and Data

### Enterprise Clients

Microsoft Teams ---

>Pros
⋅⋅*Rich cards/ctrls, Future for MSFT, Extensibility platform 

>Cons
⋅⋅*1:1 vs Team deltas - different features in 1 on 1 vs team bots
⋅⋅*@ mention bot -- Can't have a bot that responds unless you explicitly mention it

Skype for Business --- 

>Pros
⋅⋅*Popular client
⋅⋅*New BF Support
⋅⋅*On-prem product

>Cons
⋅⋅*No rich cards/ctrls
⋅⋅*Questionable future - no more investment into the Skype for Business channel for Bot Framework


Slack ---

>Pros
⋅⋅*Mature client
⋅⋅*Mature bot platform
⋅⋅*Enterprise growth

>Cons
⋅⋅*Control/Compliance
⋅⋅*Data sovereignty 

EMail ---

>Pros
⋅⋅*Everyone has email
⋅⋅*Doesn't feel like a bot
⋅⋅*Small dev footprint

>Cons
⋅⋅*High latency
⋅⋅*Inconsistent UI/UX
⋅⋅*Spam feel


Custom Embed ---

>Pros
⋅⋅*Tailored to Scenario
⋅⋅*No client/distro
⋅⋅*Full UX control

>Cons
⋅⋅*Discovery
⋅⋅*Dev bot AND client

### Data