# AI Policy

Large language models (LLMs) can greatly speed up the process of contributing to Spack. However, to ensure the quality and maintainability of our software and avoid maintainer burnout, we have to set some boundaries.

Note that this is a rapidly evolving landscape, and we may make frequent updates to this policy in order to keep up with new developments in generative AI.

## Policy

The following requirements apply to all interactions on GitHub, including discussions, issues, pull requests, code, documentation, and comments. While many of these requirements are designed with generative AI in mind, they also apply to human-authored contributions as well.

### Responsibility

You are ultimately responsible for your contributions. In particular, you must:

- understand every line of code or documentation that you contribute,
- ensure that you have permission (usually from your employer) to contribute, and
- take responsibility for any bugs you introduce.

Accidents happen, and everyone has introduced one or two security vulnerabilities before (right? right!?). The important thing is not that your code is perfect, but that you take responsibility for its quality and correctness. This includes apologizing for mistakes, fixing bugs, and reporting vulnerabilities.

Before tackling an issue or opening a PR with the assistance of AI, think about whether you could reasonably solve this problem or implement this feature without the use of AI. If not, it is unlikely that you will be able to fully grasp the AI implementation.

### Copyright

Fully autonomous or "agentic" AI contributions are not accepted as AI cannot hold copyright.[^1] You as a contributor are responsible for determining whether or not your contributions contain any code that is copied from a project under a different license. If you are not able to confirm whether or not your code is free from copyright issues, please do not open a PR. Instead, open an issue and ask someone else to contribute for you.

[^1]: [Thaler v. Perlmutter, 2025](https://media.cadc.uscourts.gov/opinions/docs/2025/03/23-5233.pdf)

### Communication

All communication with maintainers, including descriptions and comments on issues and PRs, should be made by humans. When you report an issue, we want to see you describe the issue in your own words to ensure you spent time debugging it. Similarly, when you open a PR, we want to see you summarize your implementation without AI assistance to guarantee you understand your own contribution. We may ask clarifying questions or suggest improvements to your PR. Please refrain from using AI to automatically respond to maintainer questions. It is fine to use AI for proofreading (typos/grammar) or translation, however.

### Conciseness

AI makes it easier than ever to quickly open a PR with minimal effort. However, without careful involvement of a human-in-the-loop, this can result in overly verbose PRs containing defensive coding and unnecessary testing. While this may save you time, human maintainers still have to review every line of code, unfairly shifting the burden and leading to "extractive contributions".[^2] Please keep all issues and PRs short and succinct. Avoid combining large refactors and new features in the same PR. While there are no hard requirements for word or line limits, if your PR could reasonably be split into many smaller PRs, we will likely ask you to do just that.

[^2]: [Eghbal, 2020, Working in Public: The Making and Maintenance of Open Source Software](https://press.stripe.com/working-in-public)

### Disclosure

All PRs must disclose to what extent AI was involved in writing the code using the following template:

- [ ] 🟢 **No AI usage**: written by humans, for humans
- [ ] 🟡 **AI-assisted**: AI helped with the coding, but I understand every line
- [ ] 🔴 **AI-generated**: AI did everything; I cannot explain all of the logic in this PR

## Enforcement

The above policy will be enforced at the discretion of the Technical Steering Committee based on the severity of the violation and likelihood of bot accounts. In all cases, a maintainer will point out exactly which part of the AI policy has been violated so that contributors can learn from their mistakes.

## References

This AI policy was not developed in a vacuum. While some of the above policies may seem strict, they are quite common among related libraries:

- [Linux](https://kernel.org/doc/html/next/process/coding-assistants.html): copyright, responsibility, disclosure
- [LLVM](https://llvm.org/docs//AIToolPolicy.html): responsibility, communication, disclosure, conciseness, copyright
- [Python](https://devguide.python.org/getting-started/generative-ai/): responsibility, conciseness, copyright
- [EasyBuild](https://docs.easybuild.io/policies/ai/): disclosure, responsibility
- [Homebrew](https://github.com/Homebrew/brew/blob/main/CONTRIBUTING.md#artificial-intelligencelarge-language-model-aillm-usage): disclosure, responsibility
- [pip](https://github.com/pypa/pip/blob/main/AI_POLICY.md): responsibility, copyright, communication, conciseness
- [Conda](https://docs.conda.io/projects/conda/en/latest/dev-guide/contributing.html#generative-ai): responsibility, copyright, communication, conciseness
- [uv](https://github.com/astral-sh/.github/blob/main/AI_POLICY.md): responsibility, communication, copyright
- [ruff](https://github.com/astral-sh/.github/blob/main/AI_POLICY.md): responsibility, communication, copyright
- [ty](https://github.com/astral-sh/.github/blob/main/AI_POLICY.md): responsibility, communication, copyright
- [Sphinx](https://github.com/sphinx-doc/sphinx/blob/master/doc/internals/ai-policy.rst): responsibility, disclosure, copyright, communication
- [Pytest](https://github.com/pytest-dev/pytest/blob/main/CONTRIBUTING.rst#aillm-assisted-contributions-policy): responsibility, communication, disclosure

In particular, our AI policy is most heavily influenced by LLVM, with the initial draft coming from TorchGeo!
