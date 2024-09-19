# Governance of the Spack project

All information in this file is pursuant to the Spack Technical
Charter. In case of any conflict or difference in language, the Spack
Technical Charter takes priority over this document.

## Technical Steering Committee

### Role

The role of the Technical Steering Committee (TSC) is to provide
technical direction to the project. The TSC will vote on any matters
on which the community is unable to reach consensus.

### Membership

Members can be added to the TSC by a majority vote of the TSC. Members
may be removed from the TSC by a 2/3 vote of the TSC.

Current Membership:
- <fill in list>

### TSC Chair

The TSC will elect a chair. The TSC chair runs TSC meetings and may
make interim decisions on urgent matters on behalf of the TSC, which
may be reviewed by the TSC at its next meeting.

### Meetings

The TSC meets at 9am Pacific Time on the first Wednesday of every
month. These meetings are open to the public, and are held virtually.

## Public Spack fora

### Weekly Meetings

Public Spack meetings are held every Wednesday that is not a TSC
meeting, at 9am Pacific Time. These meetings are held virtually over
[webex](https://llnlfed.webex.com/llnlfed/j.php?MTID=m96de22e81d9a3218bb76dc416420c93a).

### Spack slack

The Spack project uses slack for day-to-day communication. Invitations
to the Spack slack instance are publically available from
[slack.spack.io](https://slack.spack.io).

### Spack Github

Spack [issues](https://github.com/spack/spack/issues),
[pull requests](https://github.com/spack/spack/pulls), and
[long term discussions](https://github.com/spack/spack/discussions)
are tracked on the
[Spack GitHub page](https://github.com/spack/spack). Upcoming
high-impact changes have their own
[pinned discussion](https://github.com/spack/spack/discussions/30634).

### Announcements

The [Spack mailing list](https://groups.google.com/d/forum/spack) is
an announcements-only list. Spack also has a twitter account
`@spackpm`.

## Teams in the Spack organization

### Administrative Access to the Github Repository

Only members of the TSC may have administrative access to the Spack
repository. TSC members will be given access as needed. This list is
not generally published for operational security reasons.

### Other teams within the Spack organization

There are other teams within the Spack github organization which
control access to various permissions on the repository. These teams
are:

- `tsc`: see above
- `spack-releasers`: can create a new release of Spack
- `merge-to-develop`: can merge an approved pull request to Spack
- `triage`: can triage pull requests and issues in the Spack repository
- `maintainers`: any user registered to be the maintainer for a package in Spack

See the relevant teams in the Spack github repository for membership
of these teams. Membership in these teams is controlled by the TSC.
