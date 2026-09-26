# Preserved CoA `mod-playerbots` changes

This directory preserves the useful local CoA integration delta from the nested
`mod-playerbots` checkout without retaining that checkout as a second source
tree.

- Original repository: `https://github.com/Zyth45/mod-playerbots.git`
- Original base commit: `f112d520e33682e359871e787300dbef848eb721`
- Preserved patch: `coa-local-fixes.patch`
- Affected files:
  - `src/Ai/Class/Coa/CoaSpecialization.cpp`
  - `src/Bot/Factory/PlayerbotFactory.cpp`

The changes preserve same-faction recruitment when cross-faction group
interaction is disabled, and route low-level CoA playerbots through the
authoritative CoA starter-kit initializer instead of the generic starter
outfit path.

The nested repository's remote was not treated as user-controlled, so the
source delta is preserved here as a small Git patch on the CoA preservation
branch. The full nested checkout remains reproducible from its original base
commit and is not part of this preservation artifact.
