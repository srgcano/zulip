# Design discussions

We discuss ideas for improving Zulip's user experience, interface, and visual
design in the [Zulip development
community](https://zulip.com/development-community/). The purpose of these
design discussions is to help us make smart, well-informed decisions about
design changes to the Zulip product. We want Zulip to work great for a diverse
array of users and organizations, and discussions in the development community
are an incredibly valuable source of insight and ideas. We welcome all
perspectives, respectfully shared.

Most design discussions take place in the [#design][design stream] stream in the
development community. Discussions about mobile app design happen in
[#mobile-team](https://chat.zulip.org/#narrow/stream/243-mobile-team), and
design of the terminal app is discussed in
[#zulip-terminal](https://chat.zulip.org/#narrow/stream/206-zulip-terminal).

## Guidelines for all participants

Everyone is encouraged to participate in design discussions! Your participation
greatly helps improve the product, especially when you focus your contributions
on supporting the productivity of the design team. The following guidelines
should put you on the right track:

- Always treat other participants in the discussion with respect, regardless of
  whether you agree with their ideas. Ad hominem attacks are never appropriate.

- Aim to present your feedback precisely, with reasoning, and in as objective a
  fashion as you can manage. E.g., “This button really jumps out at me in a way
  that’s distracting; maybe it’s because of the color has a higher contrast than
  the surrounding components?” is better than, “Can we make that color less
  dark?”.

- Clarify your feedback if there are follow-up questions or points of confusion.
  However, avoid simply repeating the same points, as it does not move us closer
  to making the best decisions we can.

- When relevant, highlight information you have beyond your personal opinion.
  E.g., “I moderate a community, and often have to answer questions about how
  this works,” is more helpful than, “This is confusing.”

- Think about corner cases and interactions with existing features that the
  design will need to handle, and bring up problems with them, especially if they
  are not obvious. (E.g., “This component also appears with a darker background
  in the Drafts UI,” with a screenshot).

- Present technical considerations _where appropriate_. “X requires
  some refactoring that would take me another hour,” is probably not
  worth bringing up if X would produce a better user
  experience. “Adding X might require removing feature Y,” or “X is
  incompatible with Zulip's security model,” is important to present
  early.

- If you disagree with someone on the design team, the best way to make progress
  is usually to state your opinions and reasoning clearly and respectfully, and
  then let the other design team members catch up on the conversation. Other
  project members may find your argument persuasive, and may have ideas that
  address your concerns.

- Don’t forget to express support and appreciation for aspects of
  ideas/work that you like, whether in messages or emoji reactions! It
  helps motivate folks working on Zulip’s design, creates a more
  positive atmosphere, and helps build consensus towards decisions.

## Guidelines for code contributors

When you are working on a PR that includes frontend changes, it may be helpful
to get interactive feedback on the design. The best way to do so is by posting a
message in the [#design][design stream] stream in the Zulip development
community. Some situations where this likely to be a good approach:

- The issue or a comment on your PR specifically asks you to get feedback in the
  [#design][design stream] stream.

- The issue you’re working on is not specific about some design point, and you
  would like advice.

- You’ve implemented an issue as described, but the UI doesn’t look good or
  seems awkward to use.

- You’re prototyping an idea that’s not fully fleshed out.

Here are some guidelines for requesting design feedback:

- Start a new topic, or use an existing one if there is a topic linked from the
  issue you’re working on. If you’re starting a new topic, appending the issue
  or PR number (e.g., `#1234`) to the topic name will turn it into a handy link.

- Summarize the feature you’re working on. You should provide enough
  context for readers to understand your question, and include links
  to any relevant issues or in-progress PRs for additional background.

- Post screenshots, and screen captures if there is an interaction that
  screenshots fail to show.

  - You may want to post a few screenshots of different options you’re
    considering.

  - Screenshots should show enough of the app to evaluate how the new feature
    looks in its context, but not so much that it’s hard to see the feature.

  - Screen captures should demonstrate the feature with a minimal amount of
    extraneous content.

  - See [here](../tutorials/screenshot-and-gif-software.md) for some
    recommended tools.

- Post a clear question or set of questions that you need help with. What
  specifically are you looking for feedback on?

- Since you’ve been working on this issue, you have likely gained some expertise
  in this area. Educate others by sharing any tradeoffs and relevant
  considerations you’re aware of.

Keep in mind that the Zulip community is distributed around the world, and you
should not expect to get realtime feedback. However, feel free to bump the
thread if you don’t see a response after a couple of business days.

## Guidelines for community moderators

### General guidelines

- We generally aim to discuss raw user feedback on the product’s design in
  [#feedback](https://chat.zulip.org/#narrow/stream/137-feedback).
  The [#design][design stream] should be reserved for design aspects that we’re
  actively (considering) working on. This lets the design team focus on
  discussions that are expected to result in actionable decisions.

- If a discussion that started in another stream has shifted into the design
  phase, moving the discussion to [#design][design stream] helps the design team
  follow the conversation.

- Discussion of implementation-related decisions should ideally happen in
  [#frontend](https://chat.zulip.org/#narrow/stream/6-frontend). The line can
  sometimes blur (and that’s OK), but we should aim to move (parts of) the
  thread if there is an extensive conversation that belongs in the other stream.

- [#design][design stream] is a very high traffic stream; don’t let it prevent
  you from doing your own work. It can be helpful to pick particular
  conversations to follow, where you feel that you have insight to share.

### Improving the quality of discussions

We should aim to make sure that design conversations are helpful to those who
are doing the work and/or making the decisions.

- If a design discussion seems to have been derailed by a tangent or argument,
  consider moving the tangent to another topic so that the conversation can
  refocus on the questions at hand.

- If the direction of the discussion seems unproductive, you can explicitly
  suggest circling back to a topic where additional discussion seems valuable.

- If folks seem confused, it can be helpful to educate discussion participants,
  e.g., by pointing them to earlier threads or help pages, or
  clarifying with screenshots.

- If someone is repeating the same points in a way that’s unhelpful, you can let
  them know that you understand what they are saying and appreciate their
  feedback, but at this point would find it helpful to hear feedback from other
  participants. People may sometimes repeat themselves because they are not feeling
  heard.

- That said, sometimes the best way to deal with questions or feedback that
  don’t move the discussion forward is to let them go by without comment, rather
  than potentially getting into a protracted back-and-forth that derails the
  thread. Examples of such feedback include unmotivated personal opinions,
  proposals that ignore counterarguments that have already been discussed, etc.

- It’s totally fine to let the conversation slow down or die, especially if it
  seems to be going off-track. If the decision makers feel that they do not have
  enough feedback yet, they can revive the conversation as needed, and the pause
  can serve as a good reset.

- If a conversation is going off-track and you are not sure how to fix it, ping
  the product team to intervene and help get the conversion into a better state.

## Guidelines for decision makers

### Managing the discussion

- Decision makers should aim to follow design threads closely and provide input
  early and often, so that conversations don’t get blocked waiting for their
  opinion.

- Decision makers should actively manage discussion threads when needed in order
  to seek the types of inputs that will help them. This may include outlining a
  set of alternatives to consider, posing questions to dig into someone’s
  feedback, asking for ideas to solve a specific design challenge, etc.

- Decision makers should explain the reasoning behind their proposed decisions,
  so that it’s possible to identify any gaps in their thinking, and in order to
  build a shared understanding in the community.

- That said, decision makers are not required to respond to every comment being
  made regarding a proposal, or to answer every question.

### From discussion to decision

There is a number of factors that affect when it’s time to move a thread from
discussion to a decision.

- For very small decisions, it may be enough to get a sanity-check from one or
  two well-informed community participants.

- For more significant decisions, one should generally allow at least 1-2 business
  days for discussion, to give core team members time to share their perspective
  if they have something to contribute.

- Beyond that minimum, the decision makers can move to the decision phase
  whenever they have enough input to make a well-informed decision. Here are
  some situations that would indicate that it’s time to move on:

  - There is general consensus on how to proceed. Or, there is consensus
    between the well-informed participants in the discussion.

  - For a relatively small decision, there is enough useful feedback to
    generate a solid proposal. Especially when the decision results in filing
    a non-urgent issue, it’s fine to write up the conclusions on GitHub, and
    update the issue if more ideas come in later on.

  - If the discussion is primarily rehashing old points, and doesn’t seem to
    be generating additional insights, it’s time to redirect the conversation
    or move on to a decision.

  - If the thread has died down, and the decision makers feel that they have
    enough information to go on. (If they don’t, the thread can be bumped.)

[design stream]: https://chat.zulip.org/#narrow/stream/101-design
