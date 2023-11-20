# **Awesome Dioxus**
 
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A collection of awesome things regarding the Dioxus ecosystem.

This repository contains the list of awesome stuff that [Dioxus Awesome](https://dioxuslabs.com/awesome) uses.

# Contributing

To add your project, simply copy an existing entry and fill out all the values. It should be clear what most of them mean. There's some enums, so here are their values:

- `"type"`:
  - `"Awesome"`: Libraries/tools/or something else that helps developers with making Dioxus projects.
  - `"MadeWith"`: Real-world apps made with Dioxus. If the primary purpose of the app is aiding Dioxus developers, use `"Awesome"` instead.
- `"category"`:
  - `"Misc"`
  - `"Util"`
  - `"Logging"`
  - `"Components"`
  - `"Example"`
  - `"Styling"`
  - `"Deployment"`
  - `"Renderer"`
  - `"App"`: Generic category for `"MadeWith"` entries. Not actually displayed at the moment, because all `"MadeWith"` entries have this category.

```rust
struct Item {
    name: String,
    description: String,
    category: Category,
    
    /// Items won't display stars without this.
    github: Option<GithubInfo>,

    /// Replaces the auto-generated github link with an external link.
    link: Option<String>,
}

struct GithubInfo {
    username: String,
    repo: String,
}

enum Category {
    Util,
    Logging,
    Components,
    Example,
    Styling,
    Deployment,
    Renderer,
    Misc,
}
```
