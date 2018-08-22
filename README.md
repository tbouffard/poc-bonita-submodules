This repository allows to build the whole Bonita Platform. It is an attempt to simplify/replace the current [Bonita Community build script](https://github.com/Bonitasoft-Community/Build-Bonita)

It uses [Git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules) so to entirely clone this repository run `git clone --recurse-submodules https://github.com/tbouffard/poc-bonita-submodules`

To build the project, run `./mvnw install -DskipTests -Ptests,dev`

Note about profiles
* `dev`: for bonita-web, don't build all GWT permutations
* `tests`: for bonita-engine, build tests jar required by other modules
