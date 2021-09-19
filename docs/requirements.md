# Requirements

Here, in English, are competency questions - requirements - for the GTKG. The Requirements are identified below and then described. 

## Implementation 
The SPARQL queries formulated to test that Requirements are met are stored in the folder `resources/queries/requirements/` of this repository. Each query there has an accompanying Python file that can be used to run the query against a loaded version of part of the GTKG.

## Reqs Summary

TE = Temporal Element

### Temporal Elements per Timescale

Req ID | Name | Description
--- | --- | ---
RTE01 | TE version | Return everything known about a given TE for a given Timescale version
RTE02 | TE date | Return everything known about a given TE for a given date
RTE03 | TE latest | Return everything known about a given TE as it is known currently
RTE04 | TE noselect | Return everything known about a given TE, no version/date given
RTE05 | TE 2006 next | Return everything known about a given TE from next Timescale following a given one
RTE06 | TE in which | Return a list of Timescales in which a given TE is present

### Temporal Elements Sequences

Req ID | Name | Description
--- | --- | ---
RSEQ01 | TE Order | Return all the TEs in temporal order by start time within a given Timescale TE Collection 
RSEQ02 | TE Order End | Return all the TEs in temporal order by end time within a given Timescale TE Collection

### Timescale Differences

Req ID | Name | Description
--- | --- | ---
RDIFF01 | TE Diff | Return the start/end time differences between to Timescale versions of a given TE
RDIFF02 | TE Same | Return all the Timescales for which a given TE has no changes from that given
