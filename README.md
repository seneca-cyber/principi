# principi
Governance as Code - For Everyone. 

## Introduction

Welcome to principi, the Cyber Security industry’s first Governance as Code (GaC) platform.

## What is principi?

principi is derived from the Latin word `Principia`, which translates to "Principles" in English. It embodies the concept of Governance as Code, which involves using code to build, maintain, and audit business policies and their enforcement.

## Why principi?

Traditional governance tools are often expensive and fail to deliver on their promises. They usually excel in a few areas but lack comprehensive integration, leading to missed compliance points and user frustration.

## principi offers a fresh approach:

- **Evidence Generation:** Collects findings and policies and documents them as evidence in markdown and JSON, sent to a provider for internal and external auditors to review.
- **Flexibility:** Use any reasonable platform with an open and documented RESTful API as an evidence source.
- **Simplicity:** principi use straightforward declarative YAML syntax.
- **Integration:** Easily import evidence and policies into various tools and platforms, with EVERYTHING linked to it's control and framework correctly the first time.
- **Policy-Driven Automation:** Define and manage policies and their findings in YAML, and then publish to your Governance Platform.
- **Seamless Integration:** Works with existing provider modules or custom-built ones.

## Questions and Answers
### Q. Why do I need principi acting as a middle man between my various platforms? Can’t I just role my own API integration using curl and python?  
You are absolutely right. MIddlemen are really annoying. Until you have to change a relationship, like a new SIEM vendor, or a new Infrastructure toolset. Then you really want a simple middleman managing those relationships so you don't have to deal with that headache. Also, principi is declarative, and we already wrote many of those API integrations so you don’t have to. 

### Q. What if a module does not exist? 
If a module does not exist, you can roll your own, ask the community to roll the module, or pay us at Seneca Cyber to help you build it. 

### Q. How does principi Work? 
Simply run the command `principi --sync document.yml`, where document.yml is your principi governance as code file. Each principi file is made up of 3 primary components. 

1. **A Provider Definition** - Where are we collecting data from? Is it a finding or a policy? This information goes in here.

2. **A Receiver Definition** - Where is that data going?

3. **An Authentication definition** - What identity(s) are we using to access providers and receivers?

[Here is an example of a principi document](https://github.com/seneca-cyber/principi/blob/main/example.yml)

### Q. Is principi Idempotent? 
It absolutely is! It wouldn’t be a “X as Code” platform if it weren't! Findings will not be replicated or changed if they don’t need to be modified. As a caveat though, we are at the mercies of our providers and receivers and the strength of their APIs. principi Provider/Reciever Module documentation will provide notices if a module struggles with Idempotence. 

### Q. How much does principi cost? 
Nothing! Free for everyone. Free forever. It is open source and we are always looking for expert contributors to help us make this platform a common standard. 

### Q. Why should I use Seneca Cyber’s managed services instead of authoring my own Governance as Code environment with principi? 
One day, we would LOVE for people to have so much comfort with the platform that they feel confident enough to roll it themselves. But we kinda helped invent this Governance as Code space, and the rules are still being written for how it should be managed and ran. The team at Seneca Cyber is uniquely qualified to help organizations implement effective feedback loops around their governance practices in a fast and simple process that we’ve managed for other clients many times.


