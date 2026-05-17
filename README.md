<p align="center">
    <img src="assets/logo.svg" alt="Swift Concurrency Pro - Agent Skill for Claude Code, Codex, and Gemini" height="100" />
</p>

<h1 align="center">Swift Concurrency Agent Skill for AI Coding Assistants</h1>

<p align="center">
    <img src="https://img.shields.io/badge/iOS-26+-2980b9.svg" alt="Designed for iOS 26 and later." />
    <img src="https://img.shields.io/badge/swift-6.2+-8e44ad.svg" alt="Designed for Swift 6.2 and later." />
    <a href="https://twitter.com/twostraws">
        <img src="https://img.shields.io/badge/Contact-@twostraws-95a5a6.svg?style=flat" alt="Twitter: @twostraws" />
    </a>
</p>

An agent skill that helps AI coding assistants like Claude Code, Codex, Cursor, and Gemini write better Swift concurrency code. Covers `async`/`await`, actors, `Sendable`, task groups, `@concurrent`, structured concurrency, and more, targeting the mistakes LLMs actually make.

Also available:

- [SwiftUI Pro](https://github.com/twostraws/SwiftUI-Agent-Skill)
- [SwiftData Pro](https://github.com/twostraws/SwiftData-Agent-Skill)
- [Swift Testing Pro](https://github.com/twostraws/Swift-Testing-Agent-Skill)

Find more agent skills for Swift and Apple platform development at [Swift Agent Skills](https://github.com/twostraws/Swift-Agent-Skills).


## Installing Swift Concurrency Pro

### Claude Code

Add the Swift Concurrency Agent Skill marketplace, then install the plugin:

```
/plugin marketplace add twostraws/Swift-Concurrency-Agent-Skill
/plugin install swift-concurrency-pro@swift-concurrency-agent-skill
```

### Codex, Gemini, Cursor, and others

```bash
npx skills add https://github.com/twostraws/swift-concurrency-agent-skill --skill swift-concurrency-pro
```

If you get the error `npx: command not found`, it means you don’t currently have Node installed. You need to run this command to install Node through Homebrew:

```bash
brew install node
```

And if *that* fails it usually means you need to [install Homebrew](https://brew.sh) first.

When using `npx`, you can select exactly which agents you want to use during the installation. You can also select whether the skill should be installed just for one project, or whether it should be made available for all your projects.

Alternatively, you can clone this whole repository and install it however you want.

If you're using Xcode, watch the YouTube video on [How to Install and Use Agent Skills in Xcode](https://www.youtube.com/watch?v=nKVZBKoB6P4) for a walkthrough.


## Using Swift Concurrency Pro

The skill is called Swift Concurrency Pro, and can be triggered in various ways. For example, in Claude Code you would use this:

> /swift-concurrency-pro

And in Codex you would use this:

> $swift-concurrency-pro

In both cases you can provide specific instructions if you want only a partial review. For example, `/swift-concurrency-pro Make sure my project takes full advantage of Swift concurrency` on Claude, or `$swift-concurrency-pro Help me migrate this project to task groups` in Codex.

You can also trigger the skill using natural language:

> Use the Swift Concurrency Pro skill to look for potential concurrency problems in this project.


## Why Use an Agent Skill for Swift Concurrency?

I wrote a [book on Swift concurrency](https://www.hackingwithswift.com/quick-start/concurrency/), and update it regularly as new features are added. I’ve also written a comprehensive set of articles introducing what’s new in Swift (see [here](https://www.hackingwithswift.com/articles/277/whats-new-in-swift-6-2), [here](https://www.hackingwithswift.com/articles/276/whats-new-in-swift-6-1), and [here](https://www.hackingwithswift.com/articles/269/whats-new-in-swift-6) for examples), and so I’ve made it my business to understand the ins and outs of Swift concurrency.

This skill is the result of all that work. The rules contained here directly target common Swift concurrency mistakes made by LLMs, covering new features they aren’t trained on, older features they frequently make mistakes with, and patterns that help keep your code safe and efficient.

What this is *not* is just a dumping ground for all Swift concurrency advice ever. Agents already have a solid grounding of the fundamentals of `async`/`await`, actors, and structured concurrency, so skills that try to reteach them what they already know are just burning tokens.

*This skill focuses on what actually has an impact.*


## Contributing

I welcome all contributions, whether that's adding new checks, improving existing checks, or editing this README – everyone is welcome!

- Keep your Markdown concise. There is a token cost to using skills, particularly with SKILL.md, so please respect the token budgets of users.
- Do not repeat things that LLMs already know, because it burns tokens for no benefit. Focus on edge cases, surprises, soft deprecations, and similar.
- All work must be licensed under the MIT license so it can benefit the most people.

Please ensure you abide by the [Code of Conduct](CODE_OF_CONDUCT.md).


## License

Swift Concurrency Pro was originally created by [Paul Hudson](https://twitter.com/twostraws), who writes [free Swift tutorials over at Hacking with Swift](https://www.hackingwithswift.com). It’s available under the [MIT License](LICENSE), which permits commercial use, modification, distribution, and private use.


<p align="center">
    <a href="https://www.hackingwithswift.com/plus">
    <img src="https://www.hackingwithswift.com/img/hws-plus-banner@2x.jpg" alt="Hacking with Swift+ logo" style="max-width: 100%;" /></a>
</p>

<p align="center">&nbsp;</p>

<p align="center">
    <a href="https://www.hackingwithswift.com"><img src="https://www.hackingwithswift.com/img/hws-button@2x.png" alt="Hacking with Swift logo" width="66" height="75" /></a><br />
    A Hacking with Swift Project
</p>
