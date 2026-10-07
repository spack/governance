Spack AI Usage Policy

1. Extractive contributions

  AI tools lower the cost of producing plausible-looking contributions. At best, the maintainer cost to review these contributions is mostly unchanged. Without effort from the user, AI-generated contributions can be verbose and difficult for maintainers to review.

  A contribution is extractive when it demands more maintainer effort than the value of the contribution[1]. Common examples can be unreviewed AI-generated PRs, machine-generated issue reports, or changes the contributor cannot explain or defend. Extractive contributions are not unique to AI-assisted development, and avoiding AI use does not make extractive contributions acceptable.

  - You are responsible for everything you submit, however it was produced.
  - Understand every component of your contribution well enough to discuss and revise technical details.
  - Maintainers may close any PR or issue they judge to be extractive.
  - Contributors who repeatedly submit extractive contributions will be suspended or banned.

2. Authorship

  Every contribution must have a human author of record. AI tools may not be listed as authors or co-authors. Authors must disclose whether their PRs are AI-assisted.

  We define "AI-assisted" to mean an LLM or other AI tool wrote some portion of the characters/text of the contribution. Using AI to identify bugs or otherwise speed up development does not lead to an AI-assisted PR if the AI does not write on behalf of the user.

  - The human author's Signed-off-by: (DCO) certifies that they have the right to submit the work.
  - Do not use `Co-authored-by` for AI-assisted commits. Use `Assisted-by` if warranted. E.g. `Assisted-by: Claude Fable 5` or `Assisted-by: Claude`. `Assisted-by` is not required by the Spack project.
  - Disclosure of AI-assisted PRs is done by a checkbox template in the PR.

  Spack repositories will add an `AGENTS.md` file instructing AI agents to use `Assisted-by` and to follow the PR template when submitting PRs.

3. Human interaction

  Review comments and questions are addressed to you, not your tooling. You may use AI to help draft a reply, but a human must understand and post it.

  - Do not configure an agent to respond autonomously on PRs or issues.
  - Unattended agent responses will be treated as extractive under Section 1.


Notes:
[1] Credit for the term "Extractive Contribution" goes Nadia Eghbal in her book "Working in Public". Our definition paraphrases hers.
