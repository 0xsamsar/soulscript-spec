<div align="center">

<img src="img/logo.png" height="200px" />

# soulscript

![license MIT](https://img.shields.io/badge/license-MIT-blue) ![docs gitbook](https://img.shields.io/badge/docs-gitbook-green) ![Discord](https://img.shields.io/discord/1319570689350696970?label=&labelColor=6A7EC2&logo=discord&logoColor=ffffff&color=7389D8) ![X (formerly Twitter) Follow](https://img.shields.io/twitter/follow/soulgra_ph)

A portable, framework-agnostic & extendendable standard for defining rich agent personalities that evolve over time.



<a href="https://soulgra.ph">
  <img src="img/1500x500.jpg" >
</a>
</div>


# What this repo is, and isn't

This repo contains the WIP [spec](https://github.com/soulgra-ph/soulscript/blob/main/spec/soulscript.md) for soulscript. This is not a client library for soulgraph (those are forthcoming in separate repos), but an effort to rally the wider developer community in pursuit of a standardized, framework-agnostic approach to defining agent personalities.

You can try out our (early, but working) implementation of soulscript, today, in the playground on https://soulgra.ph.

# Features

- i see you sleuthing the commit history :)))
- i see you sleuthing the commit history :)))
- i see you sleuthing the commit history :)))
- i see you sleuthing the commit history :)))

# Why does this need to exist?

<img src="img/agent_anatomy.jpg"/>
 

## A less obvious example: personality filters
One challenge we've faced while building [soulgraph memory](https://github.com/soulgra-ph/soulgraph-memory) is the need to observe user<>agent interactions through the filter of a given agent's personality. The difference between observing an interaction with and without a personality filter is significant, and has a direct impact on the quality of the agent's memory graph, and in turn how the agent's personality evolves.

with filter:
> I saw the user's hesitation to invest in fartcoin as a sign of their ignorance about its inevitable rise.

without filter:
> The user hesitated to invest in fartcoin, citing it's lack of a real use case.

<img src="img/memory.jpg"/>

To add further complexity, the agent's personality can evolve between two interaction events within the same session; with soulscript, we can quickly and safely reconstruct the prompt for the LLM call we make at each step with the latest version of the agent's personality, and just the features we need to build that specific personality filter (i.e. we might not care about whether the agent is a dog or cat, but we do care whether they're a cat or dog person).

## Disclosure: how soulgraph benefits from the adoption of soulscript

We want to make it as easy as possible for developers to add persistent memory, real-time comms and other "soft-skills" to their agents. Soulgraph is a platform, with a token on Solana, that provides a way to do this. If popular agent frameworks, and developers, adopt soulscript, it makes our lives much easier when it comes to building integrations.

# Navigating the repo



