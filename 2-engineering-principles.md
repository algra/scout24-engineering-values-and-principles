# Engineering principles

- [Agile software development](#agile-software-development)
- [Product first](#product-first)
- [Continuous integration and delivery](#continuous-integration-and-delivery)
- [Minimize technology variation](#minimize-technology-variation)
- [Embrace platform model](#embrace-platform-model)
- [Autonomous cross-functional teams](#autonomous-cross-functional-teams)
- [Automate](#automate)
- [Loosely coupled and highly cohesive services](#loosely-coupled-and-highly-cohesive-services)
- [Cleaning is part of work well done](#cleaning-is-part-of-work-well-done)
- [You build it, you run it](#you-build-it-you-run-it)
- [Eliminate accidental complexity](#eliminate-accidental-complexity)
- [Apply principle of least privileges](#apply-principle-of-least-privileges)
- [Data is a shared asset](#data-is-a-shared-asset)

We have expressed [what we value as a Scout24 engineering
community](1-engineering-values.md) and these values should guide us to good
engineering practices. In this document, we express the primary principles that
guide our work.

We expect all of the Scout24 engineering community to:

- use the following principles wisely by understanding their intention and
  evaluating their effect on what we try to achieve, rather than blindly
  following the offered solution

- review these principles regularly to maximize their value

- engage in conversations when there are questions about or disagreement with
  these principles instead of simply ignoring them, so that there is a shared
  understanding of how we work and these principles evolve to reflect how we
  actually work.

## Agile software development

We listen to user needs and release value often so we can learn from successes
and failures and adjust our approach quickly. To achieve this, we uphold the
[Manifesto for Agile Software Development](https://agilemanifesto.org/) and
follow appropriate eXtreme Programming, Scrum, Kanban and Lean software
development practices to keep maintenance and new feature cycle time under
control.

## Product first

We focus on the value we are delivering to our users, both internal and
external, and avoid expending time and money on technology for its own sake. To
achieve this, we incorporate the solutions that meet our needs which are already
used at Scout24, otherwise preferring existing solutions from AWS, our platform
teams and open and industry sources.

## Continuous integration and delivery

We, as team members, continuously integrate our software changes with those of
our teammates and push these changes to production automatically. To achieve
this, we use trunk based development to ease the resolution of conflicts that
result from people working in parallel, feature toggles to selectively provide
access to WIP and automated build pipelines to correctly deploy code or fail
fast. We have high confidence in the code we deploy and consider monitoring as
part of our safety net. We optimize for
[MTTR](https://en.wikipedia.org/wiki/Mean_time_to_recovery) over
[MTBF](https://en.wikipedia.org/wiki/Mean_time_between_failures).

## Minimize technology variation

We deliberately minimize the variety of technologies in our system to drive
efficiency, and, at the same time, have a managed program of innovation.
To achieve this, we monitor current technologies in use,
gravitate to those that most appropriately address the given challenges
and selectively experiment with new technologies
to find those that will improve our products.

## Embrace platform model

We make full use of our Scout24 platforms, and view platforms as a collaborative
effort between product and platform teams. To do this, we adopt these platforms
where ever applicable, and when there are issues adopting them, product and
platform engineering work together to address gaps.

## Autonomous cross-functional teams

We work in small teams completely responsible for taking product concepts to
visible customer value. To achieve this, we form trusted teams able to fulfill
the functions needed to take a product from ideation to a well maintained
running service. We provide the team with resources that support their efforts
without getting in their way.

## Automate

We automate repetitive activities to achieve better predictability, efficiency,
reproducibility, resiliency, and security. To achieve this, we look for
repetition and write production quality code to automate it, and we strive to
correct or enhance such automation to avoid further manual repetition.

## Loosely coupled and highly cohesive services

We strive to minimize the coupling of services and maximize their cohesion in
order to, among other things, limit failure propagation, reduce response times
and limit the scope of software changes. To achieve this, we model the domain of
the services to keep things that change together in a single service, and
between services, we do not share databases but instead use event and then API
oriented communication.

## Cleaning is part of work well done

We keep our products and their code clean to ensure a productive work
environment. To achieve this, we refactor to keep code easily readable and
aligned with its product domain, we remove unused or unneeded functionality when
it is identified, and we remove features and their implementation when they are
not relevant to our customers.

## You build it, you run it

We, as team members, ensure that the services our team create continue to run
reliably, which motivates us to create services that are intrinsically reliable.
To achieve this, we build appropriate reliability patterns into our services,
monitor their health, promptly bring them back to a healthy state when they fail
and update their code to prevent such failures from occurring again.

## Eliminate accidental complexity

We are diligently keeping complexity at a minimum. To achieve this, we focus on
addressing current needs, accept that we are poor at predicting future needs,
establish abstractions only after there are several concrete examples to work
from and actively reduce complexity that develops over time.

## Apply principle of least privileges

Security is important to us. 
We apply the principle of least privilege in order to reduce the blast radius of security incidents and to
demonstrate clear ownership and accountability.

## Data is a shared asset

We treat data as a shared asset to ensure all permitted staff have a complete
view of the company performance. Doing so allows Scout24 employees to generate
valuable data insights from listings, traffic and money that can create more
delightful experiences for our users and employees. To fulfill this concept we
follow the [Scout24 Data Landscape
Manifesto](https://medium.com/@seangustafson/f9816ea10af8).
