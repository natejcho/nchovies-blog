---
title: Writing Good Open Source
date: "2019-11-03T22:12:03.284Z"
description: "New Econmic System"
---

My company has a private git server, on which there's multiple public repository. I'm an admin on one and the biggest hurdle to growth is finding developers willing to contribute. Our repo has about 30 developers following but contributions are made by 2 people, one of them myself, on a regular basis. THere is a revolving door of enginneers submiting a PR when it comes to resolving an issue or adding a feature that supports there application, but interest is waning.

Such an experience is common among all open source projects. If you take a look at React repo, you'll see hundreds of issues with comments like "i'd like to take this on" or "please assign me this issue" but maybe only a dozen open MRs at a time. WHy is this?

Open source is a buzzword and I think most people love the idea of it, but when it comes to actually doing it or contributing, people are much less enthusiastic.

One issue is how intimidating it is. My repo suffers from having very bespoke PR contributing guidelines, and those guidelines aren't all held in one location. some are included in the PR template, like ensuring you bump the version, or add to the changelog. Some are included in the README.md, like how to start the application. Linting is part of our CI check, but besides the script in our package.json, there is no indication of such until your pipeline fails. Versioning is complicated, we have a nested project structure so it can be hard to find which package.json version to bump. and the instructions for which can only be found in the git wiki (not in the README or the PR template).

When you're a new developer on a team it can be really hard to pickup all the nuances or paradigms the team. Some teams prefer backtick for string logic, some prefer concatination. No matter how many articles you read on not taking code reviews personally, or how the code is a shared project, and that individual's contributions are not jsut theyre own and thus there is no blame or fault. Those kind of things can only be learned with time and experience, and even still yet. Something more experienced devs need to understand is that, as a new dev, getting a hundred comments on your PR is discouraging, and that's the last thing we want in good open source projects.

To maintain a good open source project, we need to streamline the onboard process

- All necessary info should go in the README.md it should be short organized yet exhaustive. there shouldn't be any doubt on where to learn how to develope, start or contribute to a repo, and it should be up to date
- First time contributers should be welcomed warmly. A DM does wonders, face to face is amazing if possible. Letting them know we're both warm squishy things trying to figure this out helps. and will be amazing for your reputation.
- loosen up on dogmatic principles. Linting is nice, but it should aid in developement. some people get crazy about standards and practice, and the overall net effect is that it discourages contribution. This is wher some pre commit/push hooks and a Strong CI/CL pipeline does wonders
- 'Good First Issues' - last point. Whenever I look at a new repo to contribute to I know the first thing I look at is Good First Issues, having such a label is a really soft entry point for most develoeprs. keeping these issues well groomed, exhaustive, and well responded It can do wonders for your project, if you can afford the overhead.
