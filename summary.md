# GitKon 2023 tl;dr

Better git practices drives better communication and collaboration. The purpose
is to make work more joyful.

"It is a strange fate that we should suffer so much fear and doubt over so small
a thing." - Boromir, LOTR

## Collaboration

Synchronous communication is not as valuable to team collaboration as
asynchronous. Focus on supporting asynchronous comm tools. But synchronous
communication is vital to the individual.

Often the most popular tools that gain traction outside of tech are tools built
by devs for devs. Power in asynch communication.

Work in teams much like you architect software, loose coupling. Work as
independently as possible, decouple dependencies between teams. Every team is
like an API.

Have developers discuss and review code as early as possible. By the time it
gets to review, it's too late. Shift left, have developers discuss during
ideation and during active development. Favor more pair programming so the PR is
more a formality. This also saves a lot of lost time from pipeline delays.

Commit frequently! The longer your code stays out of main, the more complicated
it gets. The more useless, wasteful the review. The less useful the history
becomes.

Lots of demos of GitKraken and GitLens features. All of the demos show the
immense value to developers when the commits are scoped small. Without these
kinds of commits, there is no value in the git history and not value can be
drawn using these tools.

If you commit multiple unrelated changes that aren't covered by your commit
message, split them apart.

Do not add commits that say "made changes." Don't be a Boromir.

Speed and value are derived from bringing more context to the developer. But
with more context comes greater complexity. Work on improving developer context
with better tools and workflows. Make collaboration _simpler_. If there is a
slow bottleneck in a workflow, make that your priority to solve. The goal is to
collaborate in simpler ways.

## Mental Health

Learn to identify your center, when you're feeling your best, most energetic,
most productive. Understand what your feel when you're there. Learn to identify
when your in a bad place, learn your emotions, your behaviors or habits, when
you're not centered. Learn to recognize when you're exhibiting your off
characteristics to help you identify your need to recenter. Work to learn how to
identify those points and move your self back to center.

No real work or value is accomplished if you're not challenged, and that always
comes at a cost. That's what wisdom is. It comes from navigating those
experiences. Whether successful or failure, it doesn't matter, wisdom comes from
the experience and journey. We are all on a journey gaining wisdom.

Burnout comes from when you're truly exhausted. If it comes in the interest of
something valuable to you, then it is an achievement. Just like a marathon
runner at the end of a race, you are burned out but have accomplished much.
Burnout doesn't always mean there's something wrong with you. Burnout resulting
in nothing that you value perhaps at the motivation of bad habit or the "what
have you done for me lately" feeling is destructive. You can't run from burnout,
so learn to recognize your motivations, be aware of your state, and adjust
accordingly.

## Monorepos

Monorepos are strongly preferred over a collection of multirepos. However, there
is an assumption that you have git tools and build tools appropriately in place
to accomplish all your various isolated builds and not do everything in one
monolithic project environment. That is considered counterproductive. Tooling
and pipelines are  essential, such as bazel, buck, pants, nix. Many
organizations are currently in a state of multiple monorepos, where they are
collecting everything around a given domain into a monorepo. There is a slow
ongoing migration happening to move everything eventually with time.

Monorepos support better, shared collaboration, explorability, forced
collaboration across shared dependencies and collective upgrade.

Remember git patches (if not look it up and read about it). It was the
predominant way shared, distributed development occurred before the GitHub model
changed everything. The problem with patches is the work needed to apply them
and view them, suggest or make edits, and apply them back to a repo. GitKraken
is working to bring back patches into modern workflow by providing patch
interactions, storage, sharing, viewing, editing, and merging, called cloud
patches.

## Generative AI

The future of generative AI is to create the software to solve the problem you
want instead of knowing how to use a software tool.

Generative AI will allow developers to work at a higher level of abstraction.

### Uses

For programming,

- Uses patterns and large sets of data (code) for AI models
- Reduces time consuming dev tasks
- Frees up devs for higher-level problem solving
- Emerging market of integrated AI dev tools right now

AI can be a team mate on your team

- It's the most knowledgeable but least informed team member.
- Allow AI to crank out low level tasks
- Takes on dev-adjacent roles

AI is a rubber duck developer

- Sparks new ideas and approaches to problems
- Give it options and code snippets
- Conversational prompts help you practice explaining technical ideas and
  concepts clearly.
- Phind.com offers code suggestions - like ChatGPT just for devs

AI can be a reviewer

- Saves time flagging common problems.
- Will flag trivial, but also complex problems.
- Suggests improvements on best proactices, standards, and design patterns
- Codiga is static analysis and code review tool.
- Codium can suggest and write unit tests, plugin to IDE and writes for you.

AI can be a documenter

- Ensures code is will documented, easier to understand and share
- Provide analysis and explanation of 3rd party or legacy code. Feed it the code
  and ask it to explain it to you.
- Mintlify Doc Writer creates code documention

AI is a time saver

- Saves dev time
- Generate realistic data, content, and images for use in lower level
  environments
- ChatGPT create tables of fake content, gone are the days of lorem ipsum
- CodeWP used to scaffold wordpress plugins
- Bugasura tracks/manages bugs and issues

Considerations

- Only produces output that "looks" correct. Generated code may not be correct
- Always review, test and verify AI results
- Data provided might be used for further training, careful of this corner
- Be careful of the data you share, be aware of licensing and security before
  you submit your data
- AI content is not copyrighted (in the US) at this time
  - What does that do to your licensing for your projects?
  - Legal gray area right now

## Threat Modeling

Needs to be inherent in all software development.

## Equity in Tech

Equality is giving everyone the same opportunity. Equity is giving more to those
who need it more.

Changes like "master" to "main" are "well intentioned" but have little to no
impact on the actual problem.

More than 70% of teams are white. 39% of women felt voices unheard.

DEI roles are slowing disappearing. Industry is deprioritizing DEI in budgets.
(in US)

Containers are a way to provide equity in tech. They reduce the barrier to
entry, providing more access. They engender inclusivity and reduce stunted
growth.

## Tech Debt

All code is tech debt. Technology continually fades. Identify what tech debt is
worth paying.

Length complicated specifications are not often worth the cost. Documentation
for customers or consumers in critical. Documentation of internal functionality
or project not worth the cost.

Upgrading dependencies that are deprecated, security outdated, sunset features
are all tech debt that must be paid.

Reducing workflow bottlenecks, long waits for later stage failures, are valuable
tech debt to burn down.

Rewriting features in the newest language or framework may not be worth it. Is
it in the value of the customer or the developer?

To reduce tech debt, learn to say "no" at all phases of development.

Learn to say "no" to neat features. 80/20 rule applies. Customers will only use
80% of what you code. Try to avoid adding features that you think are great, and
deliver features that are requested.

Avoid different, special branches for each unique problem or special need. Avoid
special branches for different client or environment customizations. Focus
solely on rolling that change into the main line and ship a single release for
everyone.

## Jokes

Why couldn't the hobbit debug the code? Because it was in elvish script.

Why did the developer go broke? They lost all their cache.

There were many, many, more. 😑🫤🤭

## 🏆 Worst Talk

You should all quit your jobs and get side hustles on social media.

Domagoj Vidovic, @techwisdom, failed at several online tech businesses until he
found creating content. He has 750k followers and shared his "journey" with us.

He focused on creating social media content, quit his job, and makes more money
now than as a senior software engineer.

He moved out of the city and became a wandering tech nomad. Just look at all his
pictures of tropical locations in swim suits using a laptop!

He makes more money with social media than coding, and you can too! It's never
been easier and cheaper to start a side hustle. You can do social media, IG, YT,
TT. You can create blogs, vlogs, create courses. And you can teach others how to
do this too (uh, MLM)

Worst. Talk. Ever.

I think his content would have gone over better had he presented it as an option
for those interested in what he is doing. He presented his journey as if
everyone should want it and are wrong not to instead of being open to everyone's
journey in addition to his. He seemed very nice and personable, my snark is not
meant to demean him personally at all, only express my personal cynical disdain
for the "quit your job easy money" style of communication.
