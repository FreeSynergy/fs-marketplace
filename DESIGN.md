# FreeSynergy Marketplace - design (draft)

Status: draft, no code. Everything here is a plan; what is not built says so.

## Place in the model (ADR 0076)
Offers, requests and catalogs. An offer names where the goods are (with checksum); the goods lie in a storage place. Every offer points to a procedure for obtaining it (fs-workflows).

## Standards
ValueFlows `Proposal`; schema.org `Offer`/`Demand`; ActivityStreams `Offer`; the catalog format of fs-catalog (AppStream-based, signed).

## Facets
Store (the shop window for programs, themes, icon sets and sound themes; today the program fs-store). Installing happens through fs-files, providers are groups (fs-groups).

## Rules that apply to every FreeSynergy program
- One program, one interface (ADR 0050); commands with `supported` (ADR 0066); capabilities (ADR 0068).
- One manifest (actions, objects, attributes) produces menus, workflow building blocks, REST (OpenAPI), MCP tools and the
  catalog entry (ADR 0076 section 2).
- Layers are separate (ADR 0074): the program delivers functions and data, a frontend arranges, a style styles; motion and
  sound are their own layers. No colors, spacing or fonts in the program.
- Every program ships a default frontend and has at least two frontends in the end.
- Own data stays in the person's own data folder; sync and storage follow fs-objects and fs-files.

## Related decisions
ADR 0076; ADR 0075 (marketplace); ADR 0068 (capabilities). All decisions: [fs-documentation](https://github.com/FreeSynergy/fs-documentation).

## Open
Everything: first design round, interface (Cap'n Proto) and manifest, first frontend (pictures first).
