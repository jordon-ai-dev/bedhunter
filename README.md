# bedhunter

A multi-source hospitality venue discovery engine. It collects venues from
multiple sources, reconciles them into a single golden-record database with
full provenance, and ranks them.

## Layers

- **Collectors** (Layer 1): pull raw venues from each external source, one module per source.
- **Resolver** (Layer 2): match and merge records that refer to the same real-world venue.
- **Store** (Layer 3): the golden-record schema and database access for the reconciled venues.
- **Scoring / Output** (Layer 4): rank and filter the golden records, then export or view the ranked list.

## Phase 1 scope

Google Places collection plus venue-website email enrichment, run on Franschhoek.
