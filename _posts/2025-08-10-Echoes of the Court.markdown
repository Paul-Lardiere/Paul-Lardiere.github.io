---
layout: post
title: Echoes of the Court
date: 2025-08-10 15:01:35 +0300
image: echoes.png
tags: First-Person Narrative Exploration Adventure
---

Echoes of the Court is a first-person narrative exploration adventure set inside a detailed recreation of the Supreme Court of Canada. Players explore its public halls and hidden rooms, uncover stories connected to the Court's history, and use their discoveries to shape a novel written by the main character.

***

## Play the Game

- [Steam](https://store.steampowered.com/app/3960450/Echoes_of_the_Court/)
- [Google Play](https://play.google.com/store/apps/details?id=com.wildblueberrygames.Court)
- [App Store](https://apps.apple.com/fr/app/echoes-of-the-court/id6752741914)

***

## My Contribution

I joined the project after development had already begun and took responsibility for most of the remaining programming work.

My contribution covered a wide range of areas, including gameplay programming, mobile porting, designer-facing tools, performance optimization, debugging, platform integration, and release preparation.

Later in the project, I was also responsible for supervising an intern who assisted me with development tasks. I assigned and reviewed their work, helped them understand the existing architecture, and supported them while implementing and debugging features.

> **Role:** Gameplay and Mobile Porting Programmer  
> **Employer:** Wild Blueberry Games  
> **Platforms:** Windows, Android and iOS  
> **Responsibilities:** Gameplay, tools, mobile porting, optimization and technical supervision

***

## Gameplay Programming

A large part of my work focused on implementing and maintaining the game's core gameplay systems.

Because I joined an existing production, I first had to understand the architecture and systems that were already in place. I then expanded, refactored, and completed those systems while ensuring that new features remained compatible with the existing content.

My gameplay work included:

- Implementing new gameplay features
- Completing and improving existing systems
- Integrating narrative and exploration mechanics
- Supporting interactions with characters, objects, and the environment
- Debugging gameplay and progression issues
- Refactoring existing code where necessary
- Collaborating with designers to translate their requirements into reliable systems
- Maintaining consistent behavior across desktop and mobile platforms

***

## Designer Tools

I developed several tools to help the game designers create, configure, and test content without requiring constant programming support.

These tools were designed to make the production workflow faster and more accessible. They allowed designers to modify gameplay parameters, configure narrative content, place interactive elements, and validate their work directly inside the editor.

My tooling work included:

- Creating editor tools for configuring gameplay content
- Exposing useful parameters through clear designer-facing interfaces
- Automating repetitive content-production tasks
- Adding validation systems to detect configuration errors
- Developing debugging tools for gameplay and narrative systems
- Improving iteration times for designers
- Reducing the need for programmer intervention during content creation

Making the project more data-driven allowed the design team to iterate more independently while reducing the risk of introducing errors.

***

## Android and iOS Porting

I was responsible for adapting the project to run on both **Android** and **iOS**.

This involved more than producing mobile builds. The desktop version had to be adapted to account for different hardware capabilities, input methods, screen sizes, aspect ratios, operating-system behavior, and platform-specific requirements.

My mobile-porting work included:

- Configuring the project for Android and iOS
- Adapting gameplay systems for mobile devices
- Implementing and refining touch controls
- Supporting different screen resolutions and aspect ratios
- Adapting user interfaces for smaller screens
- Resolving Android-specific and iOS-specific issues
- Testing the game across different mobile devices
- Managing platform-specific build configurations
- Preparing builds for Google Play and the App Store
- Ensuring that the same project could be maintained across Windows, Android, and iOS
- Upgrading the project to a newer Unreal Engine version to comply with iOS requirements
- Migrating existing gameplay systems and content to the updated engine version
- Resolving deprecated APIs, compilation errors, and platform compatibility issues
- Validating the project across Windows, Android, and iOS after the engine upgrade

***

## Unreal Engine Upgrade

As part of the iOS port, I upgraded the project to a newer version of Unreal Engine to meet Apple's current iOS build and platform requirements.

This involved migrating the existing project and its systems to the updated engine version, resolving compilation errors and deprecated APIs, updating platform-specific integrations, and fixing compatibility issues introduced by the migration.

Because the game had already been in development for some time, the upgrade also required careful validation to ensure that existing gameplay features, tools, content, and platform-specific systems continued to function correctly.

After completing the migration, I validated the Windows, Android, and iOS versions to ensure that the upgrade did not introduce regressions across the supported platforms.

***

## Mobile Optimization

Performance optimization was a major part of bringing the game to mobile platforms.

The game contains a detailed 3D recreation of the Supreme Court of Canada, which required careful optimization to run reliably on devices with more limited CPU, GPU, and memory resources than a desktop computer.

I performed extensive profiling to identify the systems and assets that had the greatest impact on mobile performance.

My optimization work included:

- CPU and GPU profiling
- Memory profiling
- Investigating frame-time spikes
- Reducing expensive gameplay operations
- Optimizing systems that updated unnecessarily
- Identifying rendering bottlenecks
- Reducing memory usage where possible
- Investigating excessive allocations and memory-related issues
- Adjusting platform-specific scalability settings
- Testing performance on representative Android and iOS devices
- Balancing visual quality with performance and stability

The objective was to preserve the atmosphere and visual identity of the desktop version while ensuring that the game remained responsive and stable on mobile hardware.

***

## Cross-Platform Development

Maintaining the game across Windows, Android, and iOS required careful separation between shared gameplay code and platform-specific behavior.

Whenever possible, I kept features within a common codebase to reduce duplication and make future maintenance easier. Platform-specific implementations were introduced only when required by differences in input, hardware, operating-system behavior, build requirements, or store distribution.

This approach made it possible to maintain consistent gameplay and content across all three platforms while still supporting the specific needs of desktop and mobile devices.

***

## Intern Supervision

Later in development, I was placed in charge of an intern who joined the programming team to assist with the project.

My responsibilities included:

- Introducing them to the project's architecture and development workflow
- Selecting and assigning appropriate programming tasks
- Explaining the technical requirements of each task
- Reviewing their implementations
- Helping them investigate bugs and technical issues
- Ensuring that their work followed the project's existing conventions
- Integrating and validating their contributions
- Supporting their technical progression throughout the project

This gave me experience balancing my own development responsibilities with technical supervision, code review, and mentoring.

***

## Scope of My Work

Although the project was already in development when I joined, I completed most of the programming work required to bring it to release.

My main contributions included:

- Taking ownership of an existing codebase
- Completing and maintaining gameplay systems
- Developing tools for the design team
- Porting the game to Android and iOS
- Adapting controls and interfaces for mobile devices
- Upgrading Unreal Engine to comply with iOS platform requirements
- Migrating and validating the project after the engine upgrade
- Performing CPU, GPU, and memory profiling
- Optimizing the game for mobile hardware
- Resolving platform-specific issues
- Maintaining the Windows, Android, and iOS versions
- Supporting release preparation for Steam, Google Play, and the App Store
- Supervising and reviewing the work of an intern