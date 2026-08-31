# Contributing to Awesome Microduck

Awesome Microduck is a manually curated list of independent projects around
Pollen Robotics' Microduck. The goal is signal: a short list of things someone
can inspect, run, build, or learn from today.

## Add one project

Use one line with a direct, canonical URL:

```markdown
- [Project Name](https://canonical-project-url) — One factual sentence about its Microduck-specific value.
```

Before opening a PR:

1. Confirm the link opens and lands on the named project.
2. Say if it is a fork, simulator-only, experimental, or your own work.
3. Put it in the narrowest fitting section and alphabetize it.
4. Run `git diff --check`.

## What belongs here

- Public software, apps, agents, simulators, training work, tools, CAD, parts,
  or creative projects with clear Microduck-specific value.
- Early work is welcome when the repository is real and inspectable; describe
  its current limits instead of implying hardware validation.
- A project appears once, with one link and one useful sentence.

## What does not belong here

- Pollen's official repositories, product pages, shipped behaviors, simulator
  features, documentation, or launch demos. Those belong in the README's
  upstream reference.
- Generic dependencies such as MuJoCo, `mjlab`, or actuator libraries unless
  they have a distinct Microduck project or integration to point at.
- Individual ONNX policies, task names, challenge prompts, product bundles, or
  a generic profile/invite link.
- A fork or mirror that does not add a meaningful Microduck-specific change.

Self-submissions are welcome. Keep the PR focused and explain the one reason
the project deserves a place on the list. If a link dies or a project stops
being relevant, open a cleanup PR or remove the line directly.
