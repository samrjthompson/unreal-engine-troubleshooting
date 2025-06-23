# Red Imports

Red imports can be cause by the `.uproject` file having an additional plugin. To address this, see the default `.uproject`
file in `docs/default_uproject.txt` and ensure yours looks like that.

You can then delete the `Binaries`, `Intermediate`, `Saved`, `.idea`, `.vs`, and `.sln` file from root directory of your
project and generate visual studio project files again.