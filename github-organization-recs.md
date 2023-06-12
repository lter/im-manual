# GitHub Organization Recommendations

## Rationale

[GitHub Organizations](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/about-organizations) are a great way of centralizing many individual GitHub repositories under a common umbrella. Access to these repositories is easily shared with organization members and limits to this access can be implemented smoothly as desired across groups of users simultaneously. Organizations also "own" repositories which lessens the risk of accidental deletion. Websites created by repositories owned by the same organization have a URL with a shared root which greatly simplifies navigation around the ecosystem of products produced by an organization.

The LTER Network recommends each LTER site create a GitHub organization for itself and then encourage site staff and visiting researchers to house their repositories there rather than in their own profiles. There are many benefits of GitHub Organizations (including those outlined above) and we hope that you share our excitement for this potential new direction!

The LTER Network has followed our own advice and has a GitHub Organization which you can see [here](https://github.com/lter)!

## Naming Convention

We recommend adopting a common organization naming convention so that visitors to one organization can easily find the organization of another LTER site. Six sites currently have organizations and the general naming convention is to use the three letter site abbreviation in all caps followed by a hyphen and "LTER" (e.g., "JRN-LTER").

Note that organization names can be changed as needed without breaking an individual user's code but the link to GitHub-hosted websites/etc. will be changed if the organization name changes.

## Organization Description & README

We also recommend adding a short description of your site to the organization page, so that visitors have a big-picture overview of your site. In addition, the organization page is a great place to link to your site's main website, your [Research Organization Registry (ROR)](https://ror.org/search?query=LTER), data catalog, or other platforms and build your online presence.

We also recommend that you create a README as a landing page for the Organization. To do this, create a public repository named ".github". Add a "profile" folder and put "README.md" in that folder. The content of the README will then appear on your organization's profile and will be the first thing visitors to the GitHub Organization will see.

## Administrators

Members of an organization can be designated "owners" and they will then have access to all possible settings for the organization (including inviting new members, changing the organization name, or deleting the organization among other functions). [GitHub recommends adding more than one owner](https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/maintaining-ownership-continuity-for-your-organization) because if only a single person has that power, access to the organization settings is entirely dependent on that person.

We recommend adding the following people as owners of a site organization:

- Site Primary Investigator
- Site Information Manager
- At least one representative of the LTER Network Office

Note that these people must all have a GitHub profile to be added as owners. Even if one of the prospective owners has no other need for a GitHub account, we feel it is worthwhile to have them create a GitHub profile for the sole purpose of allowing back-up access to the organization settings if that becomes necessary.

## Organization "Teams"

GitHub organizations control access to repositories in a slightly different way than repositories owned by individual users. In a user-owner repository, other profiles can be granted access and as each person is added, their level of access is decided by the profile that owns the repository. In an organization context however, access is controlled by [Organization Teams](https://docs.github.com/en/organizations/organizing-members-into-teams/about-teams). Instead of people being granted access to repositories, teams are granted access to repositories. Users are then added to team(s) as appropriate and their level of access is dictated by [the access of the team](https://docs.github.com/en/enterprise-server@3.7/organizations/managing-user-access-to-your-organizations-repositories/repository-roles-for-an-organization). Note that only organization owners have the power to create teams or modify the level of access granted to existing teams.

We recommend creating the following teams:

- **"Admin" team** including everyone at the LTER site that should have admin-level access to all repositories (i.e., can change repository-level settings)
- **"Maintain" team** including all lead researchers who need access to non-destructive actions in repositories (i.e., most repository-level settings)
- **"Write" team** including everyone who has any need to write any amount of code (i.e., no settings access but able to add/change code in a repository)

You may also want to create additional teams for active research or lab groups that have many repositories where a consistent set of profiles will need access to all of those repositories.

As new repositories are added to the organization, an organization owner will need to add teams to those repositories (so that people in each team have the correct level of access to that repository).

## Example Organization - BLE

The [Beaufort Lagoon Ecosystem GitHub Organization](https://github.com/BLE-LTER) is a phenomenal example of everything we just described above! Check out their organization for a nice example of how one site went about setting up an Organization for themselves.

## GitHub Organization vs. Other Platforms

If you are already using a comparable non-GitHub platform (e.g., [BitBucket](https://bitbucket.org/product), [GitLab](https://about.gitlab.com/), etc.) we still recommend creating a GitHub Organization! At the very least, an organization for your site will give site researchers who do use GitHub a place to store their code and interact with peers who also use GitHub–both at and outside of your site. You can also use the description field of your organization to direct visitors to the link of whichever alternate platform your site decides best fits your needs. Finally, if a majority of sites do create their own organizations, external users will be able to use the standard naming convention to navigate among sites even in cases where each site utilizes the organization at different levels of intensity.

