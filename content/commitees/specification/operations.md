---
title: "Jakarta EE Specification Committee Operation"
---

This document describes the practices of the Jakarta EE Specification
Committee.

Changes to this document must be approved by a simple majority vote of
the Jakarta EE specification committee, conducted via the public Jakarta
EE Specification Committee (<jakarta.ee-spec@eclipse.org>) mailing list.

This is a public document.

## Specification Committee # {#specification_committee}

The Jakarta EE Specification Committee is responsible for implementing
the Eclipse Foundation Specification Process (EFSP) for all
Specification Projects (as that term is defined by the EFSP) under the
purview of the Jakarta EE Working Group. This includes the adaptation of
the EFSP for Jakarta which is referred to as the Jakarta EE
Specification Process (JESP).

The Specification Committee is ultimately responsible for ensuring that
the Final Specifications produced by the Working Group's Specification
Projects make sense. The definition of "makes sense" varies by
Specification Committee Participant, but is generally understood to mean
that the Specification can be implemented and that those aspects of the
Eclipse Intellectual Property Policy with regard to Essential Claims are
observed. In practical terms, Specification Committee Participants
wields power via the ballots that are required to approve key lifecycle
events per the EFSP.

The Specification Committee is responsible for producing, publishing and
maintaining operational guidance documentation for specification
projects. This includes the minimum requirements and process for
producing a Final Specification. It also includes operational guidance
for running a specifications TCK for the purpose of testing for
compatibility.

The Specification Chair (or their delegate) is responsible for
initiating ballots, tallying their results, disseminating them to the
community, and (when appropriate; e.g., in the case a release review
ballot) reporting them to the EMO.

The Specification Committee is also responsible for defining and
refining how they implement the EFSP/JESP for those Specification
Projects under their purview.

## Project Management Committee (PMC) # {#project_management_committee_pmc}

The primary role of the PMC is to ensure that project teams are
implementing the Eclipse Development Process. In particular, the PMC
monitors project activity to ensure that project teams are operating in
an open and transparent manner. The PMC reviews and approves (or vetos)
committer elections, first validating that candidate committers have
demonstrated sufficient merit.

The PMC is further responsible for ensuring that project teams abiding
by the Eclipse IP Policy and implementing the IP Due Diligence process.
In practical terms, the PMC approves intellectual property contributions
(CQs) and provides (limited) guidance to project teams regarding
intellectual property (deferring to the Eclipse IP Team as necessary).

The PMC is responsible for the structure of the Top Level Project and
the organization of the open source (software and Specification)
projects contained within.

The PMC is a link in the project leadership chain. As such, the PMC has
a role in the grievance handling process: they identify and document
project dysfunction (with the responsibility to remove/replace/add
disruptive committers).

The PMC provides other oversight regarding the operation of open source
projects. They review and approve release and progress review materials,
and facilitate cross-project communication within the Top-Level Project.

## Project Lead(s) Designation # {#project_leads_designation}

A specification project must designate one or more committers to serve
as the project lead. The lead is responsible for initiating reviews as
the project reaches the appropriate milestone.

## Specification Committee Votes # {#specification_committee_votes}

Specification committee approval votes connected to progress and release
reviews run for a minimum of 14 days; other votes run for a minimum of 7
days.

The requirements for each are described in [Review
Requirements/Guidelines](#_review_requirementsguidelines).

The [standard release
process](https://www.eclipse.org/projects/handbook/#release) defined in
the Eclipse Foundation Project Handbook is followed and augmented with a
specification committee ballot. Additional detail for the various
reviews can be found in these sections:

-   [Creating a Release Plan](#_creating_a_release_plan)

-   [Creating a Final Specification](#_creating_a_final_specification)

The EMO initiates a specification committee ballot by sending an email
on the public Jakarta EE Specification Committee
(<jakarta.ee-spec@eclipse.org>) mailing list that describes the nature
of the vote (creation/progress/release) and includes pointers to the PR
request containing the proposed release content (e.g. release review
document, specification document, and technical artifacts).

A specification committee member votes by responding to the ballot
message on the public Jakarta EE Specification Committee mailing list,
using the usual +1/0/-1 voting notation.

If a specification committee member votes against a motion, they must
provide a comment that explains the reason for the negative vote and
suggest steps to mitigate the issue.

The specification committee chair (or their designate) tallies the
results of the vote, and aggregates the comments and presents them to
the community via the specification project page on jakarta.ee, a
summary email to <jakarta.ee-community@eclipse.org>, and a copies to
<jakarta.ee-spec@eclipse.org> and <emo@eclipse.org>, within one week of
the completion of the vote.

The specification committee may choose to extend the deadline for a vote
by simple majority vote on the public specification committee mailing
list (<jakarta.ee-spec@eclipse.org>).

In the event that a vote fails, the EMO will fail the corresponding
review, forward the comments from the vote to the specification team,
and invite them to resolve the issues and re-engage at a later date.

Note that the EMO schedules reviews to conclude on the first and third
Wednesday of the month; this will impact the timing of the start of a
specification committee vote and the timing of a project team
re-engaging following a failed vote. This means that specification
committee chair must start the vote at least 14 days prior to the first
and third Wednesday of the next month if they wish to minimize the time
for the review to complete. In the event that the specification
committee opts to extend a vote, the EMO will, at its discretion, either
bump the corresponding review to the next review slot or withhold
approval of the review until the results of the specification committee
vote are received.

## Participant Representative Appointments # {#participant_representative_appointments}

A Member Participant may send a note to <emo@eclipse.org> to designate
or remove their representative (a Member Participant's representative
must be covered by the Member Company's MCCA and WGPA) as the
Participant Representative (and Committer) for the Member Participant on
any specification project associated with the Jakarta EE Working Group.

The EMO will maintain a record of participant representatives on the
specification project's PMI \"Who's Involved\" page in a section titled
\"Participant Representatives\" (e.g. [Eclipse Project for Servlets
\"Who's
Involved\"](https://projects.eclipse.org/projects/ee4j.servlet/who)).

## Developing Specifications # {#developing_specifications}

Specification projects in active development must engage in a progress
or release review at least once per year as required by the JESP. In
practical terms, this means that the clock starts ticking when the plan
review that occurs at the beginning of the development cycle concludes
successfully, and is reset following a successful progress review.

The entire process is halted when either the specification project
engages in a successful release review (thereby concluding the
development cycle), or the specification team decides to abandon the
cycle.

## Creating a Release Plan # {#creating_a_release_plan}

Each specification project needs to engage in a Plan Review prior to any
extensive development effort in support of a new Specification Version.
A simple Release Plan may be defined via an [Eclipse release
record](https://www.eclipse.org/projects/handbook/#pmi-commands-release).
A more extensive Release Plan may be easier to define via an external
document. If an external document is created, it should be referenced in
the Eclipse release record. That is, an Eclipse release record is
required regardless of where the detail for the release is documented.

If an external Release Plan is developed, it needs to be made available
via the Specification Project's web pages. As an example, the Jakarta EE
9 Release Plan is housed on the [Platform Project's github
pages](https://eclipse-ee4j.github.io/jakartaee-platform/jakartaee9/JakartaEE9ReleasePlan).

The Release Plan should be reviewed with the Specification Committee
before continuing with the ballot stage.

## Recommended Specification Project Repository Structure # {#recommended_specification_project_repository_structure}

The current recommendation for structure of the specification project
repository is to have one \*-spec repository with an api and spec
subdirectory for the API and specification content, and a second \*-tck
repository for the TCK content.

## Distributing Specifications # {#distributing_specifications}

Each specification project has a location on the jakarta.ee website
under [Specifications](https://jakarta.ee/specifications/).

For each final specification:

-   Links to specification documentation and all related artifacts
    including the TCK and compatible implementations that will be
    updated as new implementation are certified;

-   Metadata, including version number and date of release

-   Results of all specification committee votes

## Creating a Final Specification # {#creating_a_final_specification}

A specification document that is marked \"Final\" cannot be made
generally available until after engaging in a successful release review
(with corresponding super-majority approval from the specification
committee). A release review will have validated that the specification
project has:

1.  Produced a staging release via OSSRH staging repository for the api,
    javadoc.

    -   Javadocs should include the [Eclipse Foundation Specification
        License](https://raw.githubusercontent.com/eclipse-ee4j/jakartaee-api/master/licenses/EFSL.html).

    -   Version in pom.xml should be increased by comparing to the
        previously released API artifact.

    -   Existing \"\@version ...​\" JavaDoc tags should be updated to
        match, or removed.

2.  The candidate final [EFTL](https://www.eclipse.org/legal/tck.php)
    licensed TCK archive should be uploaded to the project directory
    under <http://download.eclipse.org/ee4j>, e.g.,
    <http://download.eclipse.org/ee4j/bean-validation/beanvalidation-tck-dist-2.0.5.zip>
    .

3.  Generate standalone TCK results or platform TCK result as
    appropriate for the spec project.

    -   Information on running TCKs in the Jakarta CI infrastructure can
        be found
        [Build\_From\_Jakarta\_EE\_TCK\_Repo\_And\_Run](https://wiki.eclipse.org/TCK:Build_From_Jakarta_EE_TCK_Repo_And_Run#Jenkins_Pipelines).

4.  Create a compatibility certification request for the compatible
    implementation being used to validate the spec in the specification
    repository issue tracker. If the project does not already have a
    compatibility-certification-request template, you can use this one:
    [compatibility-certification-request.md](https://github.com/jakartaee/specification-committee/blob/master/compatibility-certification-request.md)

5.  After that TCK is passing, submit a ballot request by creating two
    [draft
    PRs](https://help.github.com/en/articles/about-pull-requests#draft-pull-requests)
    requests against the [Jakarta EE Specification Committee
    specifications](https://github.com/jakartaee/specifications)
    repository. The first PR provides everything requested in the [PR
    template](https://github.com/jakartaee/specification-committee/blob/master/spec_review_checklist.md)
    except the javadoc contents. The second PR includes only the apidocs
    directory with the javadoc contents.

    -   These PRs are intended to provide the items that are required to
        validate the release, and provide the jakarta.ee website content
        for the specification. The repo has a PR template that lists the
        expected content for the PR. It includes:

        -   A directory using the specification code as defined in
            Projects, Specifications, and Documents, e.g., wombat

        -   A subdirectory major.minor corresponding to the version of
            the spec, (e.g., 1.6), that contains:

            -   Specification Document from (2) above in both pdf and
                html formats, e.g., wombat\_1.6.pdf and wombat\_1.6.html

            -   Summary results of TCK run showing at least one
                compatible implementation

            -   Link to final TCK test bundle if the spec defines a TCK.
                This will be signed and uploaded to the official
                specification download area when the ballot passes.

            -   The URL of the OSSRH staging repository for the api,
                javadoc artifacts

            -   An apidocs directory containing the final JavaDocs from
                the api build in the second PR.

6.  Update the Jakarta EE API jar by submitting a PR to the
    [jakartaee-api](https://github.com/eclipse-ee4j/jakartaee-api)
    project that updates the version number of your API jar file.

7.  Update Eclipse GlassFish to use the new version of your API (and
    implementation, if applicable) by submitting a PR to
    [GlassFish](https://github.com/eclipse-ee4j/glassfish).

8.  For any release other than a service release, create a release
    record (if one doesn't already exist) as described in the [Eclipse
    Project
    Handbook](https://www.eclipse.org/projects/handbook/#pmi-commands-release)
    and then:

    -   Request approval for the release from the PMC by sending an
        email to <ee4j-pmc@eclipse.org> referencing the release record.

    -   Deliver an IP Log to the IP Team for their review as described
        in the [Eclipse Project
        Handbook](https://www.eclipse.org/projects/handbook/#pmi-commands-iplog).

    -   After the PRs are reviewed and approved, contact the EMO to
        initiate the official release review by sending an email to
        <emo@eclipse.org>.

9.  When the ballot request PRs are approved, release staged artifacts
    to Maven Central. Advice on this can be found
    [MavenReleaseScript](https://wiki.eclipse.org/MavenReleaseScript).

After the release review has completed successfully, the final release
needs to be promoted to maven central. The specification committee will
promote the specification project to jakarta.ee by merging the
associated PR into the Jakarta EE Specification Committee project
repository.

Links: <https://github.com/jakartaee/jakarta.ee>,
<https://gohugo.io/documentation/>

## Review Requirements/Guidelines # {#review_requirementsguidelines}

The EMO validates:

-   That the review material meets a minimum standard (meaningful
    description);

-   That the project repository includes the required legal
    documentation;

-   That the Eclipse Intellectual Property Due Diligence process has
    been followed.

The PMC validates:

-   That the Eclipse Development Process has been followed;

-   That the project is operating in an open and transparent manner;

-   That the specification document is consistent with established
    conventions;

-   That the project has no unreasonable barriers for participation;

-   That the submission material is complete.

The Specification Committee validates:

-   That the content presented for review is in scope;

-   That the website documentation adequately and consistently describes
    the specification(s);

-   That the specification document is consistent with established
    conventions and meets the necessary quality standards.

-   For a Plan Review, a sufficiently detailed and doable Release Plan
    has been created. In addition, an [Eclipse release
    record](https://www.eclipse.org/projects/handbook/#pmi-commands-release)
    exists that describes the content for the given release. This
    description could be a reference to an external plan document.

-   For a Progress Review, that sufficient progress has been made on a
    Compatible Implementation and TCK, to ensure that the spec is
    implementable and testable.

-   For a Release Review, that a Compatible Implementation is complete,
    passes the TCK, and that the TCK includes sufficient coverage of the
    specification. The TCK users guide MUST include the instructions to
    run the compatible implementations used to validate the release.
    Instructions MAY be by reference.

## Namespaces # {#namespaces}

### Maven # {#maven}

The maven group id, artifact id, and artifact names should follow the
rules described in the
<https://wiki.eclipse.org/JakartaEE_Maven_Versioning_Rules> document.

### Java Package # {#java_package}

All new classes, as well as modifications to `javax.` classes, are
created in the `jakarta.{abbreviation}.</emphasis>` package.

This also applies to OSGi bundles produced by the project.

### Exceptions # {#exceptions}

Petition the specification committee to request an exception to the
namespace rules above.

## Coding Conventions # {#coding_conventions}

Where feasible, all source content must include a valid copyright and
license header. Tools such as the `glassfish-copyright-maven-plugin` may
be useful in ensuring consistency.

## Specification Document Conventions (Currently under discussion) # {#specification_document_conventions_currently_under_discussion}

Written in the third person tense

TBD \"uses\" vs. \"includes\"

Recommended formats, in order of preference: asciidoc, markdown, text.

The first reference to other specifications must use the official full
name. Subsequent references may use a generally accepted abbreviation.

## Initial Migration Tasks # {#initial_migration_tasks}

The requirements for the initial migration from the legacy Java EE
projects and associated naming conventions to the Jakarta conventions is
outlined in these documents:

-   [Oracle/JCP Acronym
    Guidelines](https://jakarta.ee/legal/acronym_guidelines/)

-   [Project Names and Codes](names.xml)

Using these conventions, projects need to:

-   Change the specification name to that given in [Project Names and
    Codes](names.xml)

-   JavaDocs and text documents such as README files need to be updated
    to use these naming conventions.

-   Replace references to JCP process with references to [Eclipse
    JESP](https://jakarta.ee/about/jesp/)

-   Update references to other specifications to use name in [Project
    Names and Codes](names.xml)

-   Links to JCP JSR pages need to be replaced with a links of the form
    jakarta.ee/specifications/\<code\>/\<version\> where \<code\> is the
    specification code from [Project Names and Codes](names.xml), and
    \<version\> is the particular specification version.

-   Leave existing \"\@since XYZ 1.x\" uses alone. These refer to the
    old JCP version. Future additions should use the Jakarta project
    name.

Specification projects need issue templates and labels to support the
TCK challenge process, and the compatibility request process. Creating
an issue template is described in this GitHub doc:
<https://help.github.com/en/articles/creating-issue-templates-for-your-repository>.
Creating labels is described in this GitHub doc:
<https://help.github.com/en/articles/creating-a-label>.

The current TCK challenge and compatibility request process requires the
following issue labels, which should be defined in the issue tracker:

+-----------------------------------+-----------------------------------+
| Label                             | Description                       |
+===================================+===================================+
| challenge                         | TCK challenge                     |
+-----------------------------------+-----------------------------------+
| accepted                          | Accepted certification request    |
+-----------------------------------+-----------------------------------+
| challenge-appeal                  | Appeal a rejected TCK challenge   |
+-----------------------------------+-----------------------------------+
| appealed-challenge                | TCK challenge was appealed        |
+-----------------------------------+-----------------------------------+
| certification                     | Compatibility certification       |
|                                   | request                           |
+-----------------------------------+-----------------------------------+
| invalid                           | This doesn't seem right (label    |
|                                   | already exists)                   |
+-----------------------------------+-----------------------------------+
| enhancement                       | New feature or request (label     |
|                                   | already exists)                   |
+-----------------------------------+-----------------------------------+

Finally, follow [How to Prepare API Projects to Jakarta EE 8
Release](https://wiki.eclipse.org/How_to_Prepare_API_Projects_to_Jakarta_EE_8_Release)
to create an initial Jakarta EE 8 release.