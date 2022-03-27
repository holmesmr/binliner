# binliner
An expanded version of the Binary Ninja example inlining workflow, developed while
working on a project which makes heavy use of transferring condition flags across
function call boundaries

Current additional features:

* Persistent inlining of functions using Analysis database globals (requires the
  project be saved to a BNDB file).

* Ability to mark a function for inlining in all functions.

* Experimental aggressive rewriting of inlined basic blocks to allow correct
  propagation of conditions across inlined sections.

## Building

[Follow the build instructions supplied with official Vector35 C++ plugins][binja-plugin-armv7-build].


[binja-plugin-armv7-build]: https://github.com/Vector35/arch-armv7/blob/b45883e81fc656e2274e3ed48b9a8f3839b5e9b2/README.md#building