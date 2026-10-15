ForgeStack build helper (NOT A COMPILED PLUGIN)

1. Fork https://github.com/ForgePluginsMC/forge-stack on GitHub.
2. Copy build.gradle, settings.gradle and .github/workflows/build.yml
   from this package into the root of YOUR fork, maintaining paths.
3. Commit and push the files.
4. Open your fork's Actions tab and select 'Build ForgeStack JAR'.
   Run workflow, or use the automatically triggered push build.
5. If build succeeds, download the ForgeStack-1.0.0 Actions artifact.
   Extract it to find ForgeStack-1.0.0.jar.
6. On a test Paper 26.3 server using Java 25, put the JAR in plugins/
   and restart. Check logs for compatibility problems.

This is an untested helper: the repo was not reachable from the build
container, and no compile or runtime tests could be completed here.
The declared Paper dependency version might need adjusting to match
what Paper publishes. If Gradle reports dependency resolution errors,
check https://repo.papermc.io/ for a compatible API coordinate.

The original project states that no software license is selected.
Check with its author before redistributing binaries.
