---
title: "Natural Language Interaction for Dynamic Multi-Agent Secure Collaboration"
abbrev: "NLIP-DMSC"
category: info

docname: draft-natural-language-multiagent-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
number:
date:
consensus: true
v: 0
# area: AREA
# workgroup: WG Working Group
keyword:
 - dynamic systems
 - multi-agent systems
 - natural language 
venue: 
#  group: WG
#  type: Working Group
#  mail: WG@example.com
#  arch: https://example.com/WG
  github: "nlip-project/item-draft-dmsc"
  latest: "https://nlip-project.github.io/item-draft-dmsc/draft-natural-language-multiagent.html"

author:
 -
fullname: "Dinesh Verma"
organization: IBM
email: "dverma@us.ibm.com"

fullname: "Sean Hughes"
organization: "Service Now"
email: "shughes@thealliance.ai"

fullname: "Luyi Xing"
organization: "University of Illinois"
email: "lxing2@illinois.edu"

fullname: "Rasit Topaloglu"
organization: "Marist University"
email: "rasit.topaloglu@marist.edu"

fullname: "Elisa Bertino"
organization: "Purdue University"
email: "bertino@purdue.edu"

fullname: "Abhay Ratnaparkhi"
organization: "eBay"
email: "abhay.ratnaparkhi@gmail.com"

fullname: "Sanjay Aiyagari"
organization: "RedHat"
email: "saiyagar@redhat.com"

fullname: "Ted Ross"
organization: "IBM"
email: "teross@ibm.com"

informative:

...

--- abstract

When Distributed Agents have to be collaborate in order to perform a task, they need a variety of exchanges in order to complete the task successfully. The current approach in the industry is to define a set of APIs with rigid message formats to drive this collaboration. In this document, we discuss how these can be replaced with a single API which is based on a natural language exchange. The replacement of multiple APIs with a single API can deliver significant benefits in development, debugging and deployment of agents, and should be the preferred way for intelligent agents to interact.  

--- middle

# Introduction

Intelligent Agents are characterized by one key property, they have access to an AI model that can help them process information being sent to them. The capabilities of the agent may vary depending on the specific AI model the agent may be using. Access to an AI model that can process natural language allows an agent to interpret text passed to it in a natural language and interpret it appropriately. 

The prevalining tradition for software entities to interact with each other is to define an Application Programming Interface (API). The API defined an effective application-level protocol, where each exchange specifies a function name (or URI) and a data structure. All communicating entities are required to use the same format for data structure which is transferred between them using a structured representation such
as JSON. This design approach causes significant interoperability issues when the version
upgrade of any software causes a change in the format of data structure that needs to be exchanged.

If instead of exchanging specific APIs and a rigidly formatted data structure, we use a single API that can exchange natural language, using an AI model to translate from the natural lanuage format to an internal structured representation, one can decouple the structure of internal representation from the representation on the wire. This decopuling allows the different parties to evolve independently, and updating their internal structures as they deem fit without breaking the external communication mechanism. 

In essence, this approach is a re-application of the concept of the ubiquitous 'ntohs' and 'htons' macros that are used to decouple internal representation of a data structure at a machine with the representation of a data structure on the wire. This decoupling enables machines to maintain their own internal representations. 

The reapplication of this idea in the context of application level protocols and APIs can deliver significant benefits in the development, debugging and deployment of systems with distribtued agents. 


# Conventions and Definitions

{::boilerplate bcp14-tagged}


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
