<p align="center">
  <img src="https://www.debian.org/Pics/debian-logo-1024x576.png" alt="Debian logo" width="400">
</p>

# Contributing to Debian: A Practical Path

A practical path for new contributors, from easiest to most involved.

Debian is run by volunteers, so replies can be slow. A [2025 debian-devel thread](https://lists.debian.org/debian-devel/2025/06/msg00205.html) noted that finding maintainers with time for newcomers is hard, so persistence matters.

## Step 1: Set up your tools

```bash
sudo apt install how-can-i-help devscripts reportbug
```

- `how-can-i-help` hooks into APT and lists contribution opportunities, such as orphaned packages or newcomer-tagged bugs, for packages you have installed. Run `how-can-i-help -s newcomer` to see beginner-level bugs directly. This is useful because you'll work on software you already use. ([wiki](https://wiki.debian.org/how-can-i-help), [ostechnix](https://ostechnix.com/?p=10584))
- `devscripts` gives you the `bts` command for the bug tracker.
- `reportbug` is for filing new bugs.

## Step 2: Join the mailing list

Subscribe to [debian-mentors@lists.debian.org](mailto:debian-mentors@lists.debian.org).

[Debian Mentors](https://wiki.debian.org/DebianMentors) is a community of Debian Developers who help new contributors by answering questions and reviewing and uploading proposed packages. The list is open and explicitly meant for mentees to ask for help. Read it for a week or two before posting, and read the [Debian Mentors FAQ](https://wiki.debian.org/DebianMentorsFaq) first.

## Step 3: Fix a newcomer-tagged bug

1. Open the [list of newcomer bugs](https://bugs.debian.org/cgi-bin/pkgreport.cgi?tag=newcomer). The [newcomer tag](https://wiki.debian.org/BTS/NewcomerTag) marks bugs suitable for people new to Debian.
2. Pick a package or bug that interests you, ideally one in a language you know (C, C++, Python, shell).
3. Reproduce the bug first, ideally in a VM or container running Debian unstable.
4. Ask questions if you get stuck. Email the package maintainer or debian-mentors, mentioning the bug number and what you've tried.
5. When you have a patch, email it to the bug report at `NNNNNN@bugs.debian.org`. Replace `NNNNNN` with the bug number.

## Step 4: Triage bugs (no coding needed)

Open bugs often need someone to check whether they still happen on the current version, add logs, or ask the reporter for details. This is useful work and a good way to learn how maintainers think.

You can also file well-written new bugs with `reportbug` when you find real problems.

## Step 5: Package software (the bigger step)

If you've written your own tools, packaging them could be your path:

- Check WNPP (Work-Needing and Prospective Packages) for orphaned packages you could adopt.
- Follow the Debian New Maintainer's Guide and the Packaging Tutorial on the Debian wiki.
- As a new contributor you can't upload directly. You'll need a **sponsor**, a Debian Developer who reviews and uploads your package. You find one by posting a sponsorship request (an RFS bug) and asking on debian-mentors.

## Step 6: Translations and docs

Debian also needs translators and documentation writers. Look at the Debian l10n pages for your language's team and mailing list. Documentation work is also a gentle way to get to know a team.
