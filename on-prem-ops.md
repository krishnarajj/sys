# Introduction

With these instructions you should also receive logs from the services running in 
kubernetes cluster.

Requirements:

- Provide list of errors and commands used to debug the cluster
- Suggest improvements and possible fixes
- Sum up your findings in report document

We expect you to return a `.md` or `.pdf` file with your description and investigation report
together with ideas or additional thoughts that crossed your mind while solving the problem.

Keep in mind that the goal is to express familiarity with the topics, so your
answers will be evaluated based on the quality of the report you return.
By quality, we mean the information that you provide and the ways
that you are able to expand on the topics as well as rationalize your answers.
The layout of the document will not be evaluated - although the document
should, be easily legible.

You are free to use Google, Books or any other knowledge source 
at your disposal to verify your information and to expand on your answers.


# Background

It's day 175 and you starting to feel like "The Martian" on this mission, because
well you guessed it, welcome to the Mars.

"Be a pioneer", they said. "Space, the last frontier", they said. "It's gonna be
an adventure", they said... Yet, the last month has been really boring here.

To cheer you up, the folks from planet Earth gave you the *LARVIS*, their best
version of AI, that makes you think that ChatGPT would have been better option back then.
But anyway, with the jokes and all media content to consume (mostly videos of cats and dogs),
*LARVIS* plays an essential role to keep you alive. Some of the basic functionalities
of *LARVIS* include: supporting services, Messaging to HomePlanet (Telemetry) and MissionControl
(Most important service that keeps you alive).

One day you wake up to the strange noises:

> Beep...
> Beeep....
> BEEEEEEEEEEP....

> LARVIS: Wake up! Waaaake up! I dezected anomaliZeeees in SyyyyyyStem.

I know what you thinking, oh well, this technology. It keeps on giving.
That's true indeed. LARVIS is running on a small kubernetes cluster called alpha.


What? What's going on...? You go to your terminal and try to access the services
UI, only to notice it's gone! Ugh, must be a side effect of the last bootstrap.
Doing some quick tests, the Telemetry is also gone, but seems like the self-healing
properties of *LARVIS* kicked in, and produced... yeah, logs just bunch of logs.
You are an expert kubernetes engineer, this should be enough to get started solving the issue.

The time is ticking, your oxygen is running low, currently on 98%.

# Debug Alpha

On this cluster the are above mentioned services running on 4 Linux nodes (Ubuntu 25)
on top of the Kubernetes (1.24) cluster with 1 control node and 3 worker nodes.

You cannot destroy and recreate running system otherwise you would loose oxygen
and since you are a living creature unlike *LARVIS* you really do need to have that oxygen.
*LARVIS* does not allow any interaction of the internal cluster, you first need to provide reasoning
then you will be allowed to execute needed commands it is all due to security reasons.
Dont ask why, that is what we were told from Earth.

Damn! That oxygen, hurry up you don't have much time 75%.

Try to read the logs, spot errors and mistakes made in configurations also prepare
commands that you would run when you get access to fix the configuration and whole cluster.

# Write a report for *Alpha* cluster

In practice, this means suggesting improvements to the services and their configuration
and putting all that into single document which can be reviewed.
